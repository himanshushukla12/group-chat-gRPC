Certainly! Here's an updated version of the README markdown file with the additional instructions:

```markdown
# Project Name

Brief project description here.

## Installation

To run this project, make sure you have the following dependencies installed:

1. **grpcio** - Version 1.9.0
   ```bash
   pip install grpcio==1.9.0
   ```

2. **grpcio-tools** - Version 1.9.0
   ```bash
   pip install grpcio-tools==1.9.0
   ```

3. **protobuf** - Version 3.18.3
   ```bash
   pip install protobuf==3.18.3
   ```

4. **six** - Version 1.11.0
   ```bash
   pip install six==1.11.0
   ```

5. **tkinter** - (Usually included in standard Python installations)
   - For Python 3.x: `sudo apt-get install python3-tk` (on Debian/Ubuntu)
   - For Python 2.x: `sudo apt-get install python-tk` (on Debian/Ubuntu)

## Running the Project

Follow these steps to run the project:

1. Create `chat.proto` - Define your gRPC service in the Protocol Buffers file.

2. Run `generate-proto.bat` - Execute the batch file to generate gRPC service code from the `chat.proto` file.

3. Run `server.py` - Start the gRPC server.

4. Run `client.py` - Execute the client script to interact with the server. You can run multiple instances of `client.py` for multiple clients.

## Additional Notes

Include any additional notes or information about the project here.

```

Replace "Project Name" with the actual name of your project and update the brief project description and running instructions accordingly. Make sure to provide clear and concise instructions for users to follow.
