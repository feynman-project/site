---
name: 'Initial Plan'
date: 2022-01-25
---

<script>
    import Log from '../../../components/Log.svelte'
</script>

<Log name={name} rawDate={date}>

## Elevator Pitch

Help students learn about the relationship between resistance, current, voltage, and capacitance. This is done by creating physical circuits that allow students to change the inputs (e.g. voltage or amount of resistance) and see the change in the outputs (current, voltage drops, equivalent resistance, etc).

## Main Parts

### PDM (Probe Display Module)

The PDM is a simple system for allowing the user to select a predetermined point in the circuit and have the current and resistance be displayed at that point on the LCD display. This is a generic system that can plug into any circuit and can be expanded to work with more points. This means that I only need to make the board once. The module consists of 3 core parts:

- LCD -> The display that will show the current and voltage drop at the given point.
- Microcontroller -> Device that will run the code to display and measure the current and voltage drops.
- Buttons -> Buttons that allow a user to select which point to display and measure.

### UC (User Circuits)

A basic circuit that has sockets for placing resistors and capacitors in the circuit to see how they affect the current and voltage drops. This system contains at least one set of power supply ports and two sockets for attaching through hole components (e.g. resistors, capacitors, and LEDs).

## Example Circuit

![Basic Board](/images/basic-board.svg)

## Main Problems

There are a number of things I need to figure out before I have the PCBs made:

- Apparently, it is impossible to record voltages over 3.3 volts on the microcontroller without doing ratio-based estimation or using a dedicated voltage recording board. I need to figure out a way to record the voltages.
- Can I write the code in rust? There is a HAL for AVR but it seems complicated flashing the binary to the board. It is also possible that there isn't libraries for rust that I might need to accomplish this project.
- What CAD software should I use to create the PCBs? KiCad looks promising and is open-source. I'll have to try out a few.
- Who should I order the boards from? I've heard that PCBWay is a good manufacturer and should be very cheap (~$10) for 4 boards.

</Log>
