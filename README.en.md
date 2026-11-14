# ZE1 Monitor

A vehicle monitor app (Android) for the 2nd-generation Nissan Leaf (ZE1, model years 2017–2025).
This is an unofficial app made by an individual. It is not affiliated with Nissan.

[日本語](README.md)

## Features

- Home: SOC, power (including regen), pack voltage, speed, range, battery temperature, 12 V battery, outside temperature, odometer
- Battery: SOH, capacity, the 96 cell voltages, battery temperatures, quick/normal charge counts, records and trends
- Charging view, trips, eco-driving challenge, milestones, threshold alerts
- Driving and charging records (CSV), demo mode, text size, Japanese and English

## Requirements

- A phone, tablet or car head unit with Android 8.0 or later
- An ELM327-compatible OBD2 adapter (Bluetooth, BLE or Wi-Fi)

## Install

1. Download `ze1monitor-0.1.0.apk` from [Releases](https://github.com/kojipa/ze1monitor-releases/releases).
2. Open the file and install it (allow installing from this source if Android asks).
3. Plug the adapter into the car's OBD2 port, choose it in the app and connect.

## Notes

- The app sends read commands only. It never sends commands that change the car's settings.
- Use at your own risk. Do not operate the app while driving.
- Quick charging and the 62 kWh (e+) are still being checked.
- The survey app (ZE1 Monitor Survey) is a separate app; both can be installed at the same time.

## References

How the values are read was based on these public sources (no code was copied):

- [OVMS v3](https://github.com/openvehicles/Open-Vehicle-Monitoring-System-3) (vehicle_nissanleaf, MIT License)
- [zerinrc/ze1tcu](https://github.com/zerinrc/ze1tcu) (MIT License)
- [dalathegreat/leaf_can_bus_messages](https://github.com/dalathegreat/leaf_can_bus_messages) (Nissan Leaf 2018 ECU polling)
