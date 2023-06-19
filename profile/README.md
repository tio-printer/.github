# tio

A tinkerer-friendly device that prints messages via a thermal "receipt" printer. Tio stands for "Thermal I/O" or "Thermal In/Out." 

## Documentation

Read [the tio docs on GitBook](https://bpmct.gitbook.io/tio/) to learn more and see common use cases.

## Help & Feedback

Create or browse [GitHub issues](https://github.com/tio-printer/tio/issues) for support.

## Hardware

The tio client can run on single-board computers (e.g. Raspberry Pi) or microcontrollers (ESP32). It is expected for an ESC/POS compatible printer + 2 momentary buttons to be attached to the device.

## Architecture

- client: Application that connects to an ESC/POS thermal printer, accepts print jobs via MQTT, and communicates actions (button push) to the server 
- server: REST API that processes actions (e.g. "button press" and sends print jobs via MQTT)
- database: The server connects to a PostgreSQL database which stores user, devices, collections, etc.

## Roadmap

See [GitHub Projects](https://github.com/orgs/tio-printer/projects/2) for a basic roadmap.

## Contributing

Instructions coming soon
