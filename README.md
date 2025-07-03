This script is designed to decode message log files generated during communication between Electric Vehicle (EV) Chargers and Battery Management Systems (BMS), adhering to the GB/T 27930-2015 standard. The input files are .asc format log files exported from CANalyzer 12.0.

During initial analysis using CANalyzer, it was identified that the associated database file exhibited structural deficiencies, resulting in missing critical information. To address this, a comprehensive study of the GB/T 27930-2015 communication protocol was undertaken, leading to the development of this script. Its primary purpose is to facilitate the accurate extraction of essential charging-related data.

To utilize the script, export your .asc file from CANalyzer and execute `main.py`. The following key parameters will be exported:

*   Time
*   Requested Voltage (U_Req)
*   Requested Current (I_Req)
*   Charger Output Voltage (U_CCS)
*   Charger Output Current (I_CCS)
*   Battery Voltage (U_BCS)
*   Battery Current (I_BCS)
*   Maximum Temperature (Max_T \[°C\])
*   State of Charge (SOC)
*   Time Charged (Time_Charged \[min\])
