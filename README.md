# Adafruit Fingerprint Sensor Library for STM32F4

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)
![Platform](https://img.shields.io/badge/platform-STM32F4-orange.svg)

This repository contains a library for interfacing the [Adafruit Fingerprint Sensor](https://www.adafruit.com/product/4690) with an STM32F4 microcontroller. This library was developed as part of a project for the Embedded System Design course at the University of Colorado Boulder.

![image](https://github.com/kiranj26/Adafruit_Fingerprint_STM32F4/assets/111842372/6010a094-1db7-4dd5-8c19-a0baab9a4497)


## Features

- **Easy Integration**: Simple and straightforward API for interfacing with the fingerprint sensor.
- **Real-Time Performance**: Optimized for real-time applications using the STM32F4 microcontroller.
- **Comprehensive Documentation**: Detailed setup guide and usage examples included.

## Getting Started

### Prerequisites

- STM32F4 microcontroller board
- [Adafruit Fingerprint Sensor](https://www.adafruit.com/product/4690)
- STM32CubeMX and STM32CubeIDE
- (Other tools or libraries)

### Installation

1. Clone the repository and open it in STM32CubeIDE.
2. Configure the microcontroller settings in STM32CubeMX.
3. Add the source files from the `src` directory to your project.

### Usage

This library provides functions for:

- Initializing the UART interface for the fingerprint sensor.
- Verifying the password for sensor access.
- Capturing fingerprint images.
- Converting images to fingerprint templates.
- Creating and storing fingerprint models.
- Searching for fingerprint IDs.
- Managing the fingerprint database (enrollment, deletion, and clearing).
- Controlling the LED indicators on the sensor.

Refer to the [setup guide](docs/setup_guide.md) for detailed instructions on integrating the library into your project.

### Observed Data and Functionality

The following data and functionality are supported by the library:

- **Return Codes**: The library defines various return codes such as `FINGERPRINT_OK`, `FINGERPRINT_NOFINGER`, `FINGERPRINT_IMAGEFAIL`, etc., to indicate the status of fingerprint operations.
- **Commands**: The library uses several commands to interact with the sensor, including `FINGERPRINT_GETIMAGE`, `FINGERPRINT_IMAGE2TZ`, `FINGERPRINT_REGMODEL`, `FINGERPRINT_STORE`, and more.
- **Packet Handling**: The library handles communication packets between the STM32F4 microcontroller and the fingerprint sensor, ensuring reliable data transfer.
- **LED Control**: The library includes functions to control the onboard LED of the fingerprint sensor, allowing users to turn it on or off, and set colors if supported.

### Example Usage

Although we have not included specific example code in this repository, you can refer to the [usage examples](docs/usage_examples.md) documentation for guidance on how to implement the various functionalities provided by the library.

## Documentation

Detailed documentation is available in the [docs](docs) directory, including:

- [Setup Guide](docs/setup_guide.md)
- [Usage Examples](docs/usage_examples.md)

## Contributing

Contributions are welcome! If you have any improvements or suggestions, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project was developed as part of the Embedded System Design course at the University of Colorado Boulder.
- Special thanks to the professors and peers who provided guidance and support.
