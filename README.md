# gRPC Group Chat Application

The gRPC Group Chat Application is a real-time, bidirectional streaming communication platform that enables users to participate in group discussions seamlessly. Built on the gRPC framework, this application leverages the power of bidirectional streaming to provide a highly efficient and responsive group chat experience.

## Key Features:

1. **Bidirectional Streaming:**
   The application employs gRPC's bidirectional streaming capabilities, allowing for efficient and instantaneous communication between the server and multiple clients. This bidirectional channel ensures that messages are delivered in real-time to all participants, creating a dynamic and interactive group chat environment.

2. **Scalability:**
   Built on gRPC, the group chat application is designed for scalability. It can easily handle a large number of participants concurrently engaging in conversations. The bidirectional streaming model ensures that the server can efficiently manage and distribute messages to all connected clients, making it suitable for both small teams and large communities.

3. **Secure Communication:**
   gRPC inherently provides secure communication through the use of Transport Layer Security (TLS). This ensures that all messages exchanged within the group chat are encrypted, safeguarding the confidentiality and integrity of the communication.

4. **Dynamic Membership:**
   Users can dynamically join or leave group conversations without disrupting the communication flow. The bidirectional streaming mechanism allows the server to push updates about user status changes, ensuring that all participants stay informed about the current group composition.

5. **Customization:**
   The application allows users to customize their profiles, including display names and avatars. This personalization enhances the user experience and facilitates easy identification of participants in the group chat.

6. **Robust Error Handling:**
   The gRPC Group Chat Application incorporates robust error handling mechanisms, ensuring the stability and reliability of the communication channel. In the event of connection issues or other disruptions, the application gracefully manages reconnections and continues the chat seamlessly.

## Code Dependencies:

```
python
from google.protobuf import descriptor as _descriptor
from google.protobuf import descriptor_pool as _descriptor_pool
from google.protobuf import symbol_database as _symbol_database
from google.protobuf.internal import builder as _builder
import grpc
import threading
from tkinter import *
from tkinter import simpledialog


Note: Ensure that you have the required dependencies installed, as specified in the `requirements.txt` file.

```
 plaintext
grpcio==1.9.0
grpcio-tools==1.9.0
protobuf==3.18.3
six==1.11.0


## Steps to Run the Application:

1. **Create `chat.proto`:**
   - Define the protocol buffer messages and service in a file named `chat.proto`.

2. **Run `generate-proto.bat`:**
   - Execute the batch file (`generate-proto.bat`) to generate the gRPC-related code from the `chat.proto` file.
   
3. **Run `server.py`:**
   - Start the server by running the `server.py` script. This initializes the server to handle incoming client connections.

4. **Run `client.py` (as many clients as you want):**
   - Execute the `client.py` script for each client you want to connect to the group chat. Multiple clients can join the conversation simultaneously.
