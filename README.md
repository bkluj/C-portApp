# C-portApp -- Serial Port Communication Tool

C-portApp is a Windows Forms application written in C# for handling
serial communication via COM ports. It provides a user‑friendly
interface for configuring serial port parameters, sending and receiving
data, and monitoring communication in real time.

------------------------------------------------------------------------

## Features

### 🔌 Serial Port Configuration

-   Select COM port
-   BaudRate: 2400 / 4800 / 9600
-   Data Bits: 6 / 7 / 8
-   Stop Bits: One / Two
-   Parity: None / Odd / Even
-   Enable/disable DTR and RTS
-   Refresh available COM ports

------------------------------------------------------------------------

### 📤 Sending Data

Supports sending data using: - **Write** - **WriteLine**

Send modes: - Send button
- Automatically on **Enter** key
- Clear outgoing message
- Message length counter

------------------------------------------------------------------------

### 📥 Receiving Data

-   Displays received data in real time
-   Shows the length of incoming messages
-   Two display modes:
    -   **Always Update** (overwrite incoming data)
    -   **Add to Old Data** (append data)
-   Clear received data

------------------------------------------------------------------------

### 📊 Additional UI Features

-   Connection progress bar
-   Connection status: **ON/OFF**
-   Error handling for invalid COM settings

------------------------------------------------------------------------

## Installation

1.  Clone the repository:

```{=html}
<!-- -->
```
    git clone https://github.com/bkluj/C-portApp.git

2.  Open the project in **Visual Studio** (recommended: 2022).

3.  Ensure you have:

    -   .NET Framework compatible with the project
    -   `System.IO.Ports` available

4.  Start the application (F5).

------------------------------------------------------------------------

## Project Structure

    C-portApp/
    │
    ├── Form1.cs               # Main application logic
    ├── Form1.Designer.cs      # UI layout (auto-generated)
    ├── Program.cs             # Application entry point
    └── C-portApp.csproj       # Project configuration

------------------------------------------------------------------------

## Usage

1.  Connect your device via USB/RS-232.
2.  Launch the application.
3.  Choose a COM port and configure communication settings.
4.  Click **Open** to establish a connection.
5.  Send messages via button or Enter key.
6.  View received data in the reception window.

------------------------------------------------------------------------

## Known Limitations

-   No advanced protocol support (e.g., Modbus, CAN).
-   Text-only communication.
-   No built-in logging (can be added in future).

------------------------------------------------------------------------


## License

Distributed under the MIT License.
