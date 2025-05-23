# Si-Time

Si-Time ensures that the timing requirements of the design are met. It analyzes the timing behavior of a digital circuit without considering its dynamic behavior or how it may change over time due to varying input conditions. The tool evaluates signal propagation delays, setup and hold times, clock skew, and other timing constraints to verify that the design operates reliably within specified timing margins. Si-Time helps designers identify and rectify timing violations early in the design process, reducing the risk of costly errors and ensuring that the final product meets performance requirements.

## How to Start
All the necessary files are packaged in a tarball. The user only needs to download and extract its contents to a preferred location, then run the setup script.
For further installation instructions, refer to the user manual in the doc folder or contact us at info@sihi-tech.com.

## Running SiTime with Docker

After saving the `INSTALL` directory inside the `data` directory of the `Docker_file`, follow these steps:

```bash
cd create_docker
make build-docker
make run

/* In Docker Environment */
cd data/INSTALL
./SiTime

/* Save/Load Docker Image */
cd create_docker
make save
cd use_docker
make load
