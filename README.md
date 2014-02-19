# DMX/RDM Adapter / RS485 Hub

This is a board which allows you to:
- Interconnect any standard DMX plugs, which includes XLR 3 pin male+female, XLR 5 pin male+female and RJ45
- Flip the data lines for each port in case of wiring error
- Connect each plug to an internal RS485 hub (in "direct" mode, each Data+/Data- lines are connected to each other)
- Terminate each port and enable/disable RX (only if port is connected to the RS485 hub)
- Connect a logic probe to the RS485 hub or to the secondary data ports (useful for the OLA logic sniffer)
- Display RX/TX status (RS485 hub mode only)
- Powered via battery (9V) or US or USB)

# Applications

## Interconnect DMX plug formats directly


1. This mode works unpowered. You don't need to connect a battery or USB
2. Flip all switches from "TO HUB" to "DIRECT"
3. Connect exactly 2 plugs you wish to connect. If you connect more, data collisions can occur on the bus

## Interconnect DMX plug formats via the RS485 hub

1. This mode requires power. Connect a 9V battery or USB and flip the power switch to the specific "ON" position (either USB or BATTERY)
2. Flip the switches for all used ports from "DIRECT" to "HUB"
3. Connect as many plugs as you like
4. The LEDs should indicate RX/TX status

## Retrieve the data on the DMX bus via a logic analyzer

1. Set up as described in "Interconnect DMX plug formats via the RS485 hub"
2. Connect your logic probe to the GND and DATA pins on the bottom right

## Retrieve the data of the DMX secondary data lines

1. This mode works unpowered. However, you need an RS485 driver (like the SN75176) to convert the differential signal into logic levels
2. Connect your probe to the secondary data port


