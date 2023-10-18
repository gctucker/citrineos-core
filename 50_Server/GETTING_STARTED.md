# Welcome to CitrineOS

CitrineOS is an open-source project aimed at providing a modular server runtime for managing Electric Vehicle (EV) charging infrastructure. This README will guide you through the process of installing and running CitrineOS.
This project is TypeScript-based and OCPP 2.0.1 compliant.

## Getting Started

### Prerequisites

Before you begin, make sure you have the following installed on your system:

- Node.js (v16 or higher): [Download Node.js](https://nodejs.org/)
- npm (Node Package Manager): [Download npm](https://www.npmjs.com/get-npm)

### Installation

1. Clone the CitrineOS repository to your local machine:

   ```shell
   git clone https://github.com/s44-energy/CitrineOS.git
   ```

2. Navigate to the CitrineOS directory:

   ```shell
   cd CitrineOS
   ```

3. Install project dependencies:

   ```shell
   npm install
   ```

### Configuration

CitrineOS requires configuration to allow your OCPP 2.0.1 compliant charging stations to connect. You can configure the server by editing the config.json file in the root directory.

   ```json
    {
        "ocpp": {
            "version": "2.0.1",
            "port": 9220, // Change to your desired port
            "endpoint": "/ocpp"
        }
    }
   ```

### Starting the Server

To start the CitrineOS server, run the following command:

   ```shell
   npm run start:dev
   ```

This will launch the CitrineOS server with the specified configuration.

### Usage

You can now connect your OCPP 2.0.1 compliant charging stations to the CitrineOS server. Make sure to configure the charging stations to point to the server's IP address and port as specified in the config.json file.

### Contributing

We welcome contributions from the community. If you would like to contribute to CitrineOS, please follow our contribution guidelines.

### License

CitrineOS and its subprojects are licensed under the Apache License, Version 2.0. See LICENSE for the full license text.

### Support and Contact

If you have any questions or need assistance, feel free to reach out to us on our community forum or create an issue on the GitHub repository.

### Roadmap

- Support for Kafka Streams
- Support for OCPP 2.0.1 Core Profile