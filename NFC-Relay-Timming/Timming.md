# PN532Killer-PicoW-NFC-RELAY Timming

As we know, the NFC Relay based on PN532Killer&Raspberry Pi PicoW worked.

The system structure of NFC Relay is as follows:

![](https://github.com/NFC-funs/PN532Killer-PicoW-NFC-RELAY/blob/main/NFC-Relay-Timming/picture/PN532Killer-NFC-Relay-Schema.png)

If we want to emulate a "original" tag, we want the time from the reader sends command to the tag returns the data is shorter.


Fortunately, there are two test points in the PN532Killer.
The test point "DI" indicates the tag's data and "EI" indicates the reader's command.

![](https://github.com/NFC-funs/PN532Killer-PicoW-NFC-RELAY/blob/main/NFC-Relay-Timming/picture/PN532Killer-Data-Point.png)

If wen can capture the waveform of the "DI" and "EI", we will calculate the gap between the two.

The test results are as follows:

## The timming of read Ntag215's blocks

![](https://github.com/NFC-funs/PN532Killer-PicoW-NFC-RELAY/blob/main/NFC-Relay-Timming/picture/Ntag-Read-All-Block.png)

## Example 1 of the FDT -- 3ms

![](https://github.com/NFC-funs/PN532Killer-PicoW-NFC-RELAY/blob/main/NFC-Relay-Timming/picture/Ntag-Read-Block-3ms.png)

## Example 2 of the FDT -- 8ms

![](https://github.com/NFC-funs/PN532Killer-PicoW-NFC-RELAY/blob/main/NFC-Relay-Timming/picture/Ntag-Read-Block-8ms.png)
