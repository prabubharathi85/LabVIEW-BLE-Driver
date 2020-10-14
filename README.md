Products and Environment

Hardware RF|Wireless

Software LabVIEW

Driver NI RF Device Drivers

Operating System Windows 10

Programming Language .NET C Sharp LabVIEW 2020

Description This example demonstrate on how to use the windows 10 BLE native library to communicate with BLE devices (Smart watch, bulb or any device which support BLE). This does not need any BLE dongle to communicate with BLE devices. It uses the windows 10 bluetooth stack and its native library to communicate with BLE devices.

Developed the DLL to interact with windows 10 BLE library in C# platform and integrated the dll into LabVIEW by using .Net constructor node.

Here demonstrates usage of the Bluetooth Generic Attribute (GATT) Client APIs for Universal Windows Platform (UWP), along with sample code for common GATT client tasks:

Query for nearby devices Connect to device Enumerate the supported services and characteristics of the device Read and write to a characteristic Subscribe for notifications when characteristic value change

How to Use Following are the methods available in BLE library:

Methods:

BLE_Initialize.vi - Initialize the DLL BLE_StartWatcher.vi - listening advertisement of near by BLE devices BLE_Get_WatcherResponse.vi - Gets the manufacture data, BLE address from BLE advertisement BLE_Get_WatcherReceivedData.vi - Decodes the watcher response BLE_StopWatcher.vi - Stop getting advertisement from near by BLE devices BLE_Request_Connect.vi - Initiates the connection to BLE device and returns with response of connection status and GATT Services list from BLE device BLE_Get_ServicesUUIDs_Property.vi - Gets the GATT service UUIDs and Property UUIDS from BLE device BLE_Notify.vi - Initiate the BLE notification of UUIDs from BLE device BLE_Notify_Listener.vi - Gets the notification of UUIDs from BLE device BLE_Read_Characteristic.vi - Reads the UUIDs of BLE device BLE_Read_CharacteristicArray.vi - Reads the array of UUIDs of BLE device BLE_Request_ServiceUUIDs.vi - Get the Service UUIDs BLE_Write.vi - Write the UUIDs of BLE device BLE_Write_Without_Response.vi - Write the without response UUIDs of BLE device and not return response

Additional Information When setting the debug logs to true, C# library created the BLE log files under C drive

Development Environment: LabVIEW 2020 32 Bit OS: Win 10 64 bit

Added the Example code in HLD where user has to change the BLE address before run. The BLE address can be get after running the watcher.
