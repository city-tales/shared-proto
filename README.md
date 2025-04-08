# shared-proto

This repository contains **Protocol Buffers** (`.proto`) files used across multiple microservices in the architecture. These Protobuf files define the **gRPC services** and **message types** that are shared across services.

By centralizing these Proto files, we ensure **consistent communication protocols** across all services, enabling efficient and scalable communication.

## Repository Structure
The files name should be present under the particular folder and the folders will be present in their respective microservices folder.

### **Proto Files Overview**

- **`microservice/folder/file`**: Each folder defines the service dependency on the microservice and each file would describe the use cases of the folder.

## Usage

Integration of Proto files in microservices and API Gateway:

### **Option 1: Using Git Submodules**

1. The **`shared-proto`** repo will be a **Git submodule** in microservices:

   ```bash
   git submodule add https://github.com/city-tales/shared-proto.git /path/to/shared-proto

2. If it does not work try with commands
   ```
   git submodule init     
   git submodule update     
   ```
### Error Handling and Logging
Standardized error handling and logging definitions is implemented to ensure consistency across all services.

### License
This project is licensed under the MIT License.

## Contributing
Contributions to the project are welcome! If you encounter any bugs, have suggestions for improvements, or would like to add new features, please open an issue or submit a pull request.

When contributing, please adhere to the existing code style, follow best practices, and ensure thorough testing of your changes.