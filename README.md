Modbus Master RTU/ASCII 
Supported Register
•	0x01: Read coil status
•	0x02: Read input status
•	0x03: Read holding registers
•	0x04: Read input registers
•	0x05: Force single coil
•	0x06: Preset single register
•	0x0f: Force multiple coils
•	0x10: Preset multiple registers
•	0x11: Report Slave ID.
•	0x16: Mask write register
•	0x17: Read/Write registers
C#
Int16[] Registers = new Int16[10];
ModbusRTU.Result Result;
Result = modbusRTUControl1.ReadHoldingRegisters(1, 0, 10, Registers);
Visual Basic
Dim Registers(10) As Short
Dim Result As ModbusRTU.Result
Result = modbusRTUControl1.ReadHoldingRegisters(1, 0, 10, Registers)
C++
array^ Registers = gcnew array(10);
ModbusRTU::Result Result;
Result = modbusRTUControl1->ReadHoldingRegisters(1, 0, 10, Registers);


