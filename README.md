# PN532Killer-PicoW-NFC-RELAY
NFC Relay Based on PN532Killer&amp;Raspberry Pi PicoW

###Project ideas

PN532Killer can be used as a NFC reader or a tag emulator.

If the one act as a reader, and the other emulate a tag, the data between the reader an tag can be transimtted over WIFI, BLE ,LORA, etc.

Raspberry Pi PicoW built in WIFI&BLE, so it is ideal for data transfer.

Data flow:
PN532Killer1(reader) <--uart--> PicoW1 <--    wifi    --> PicoW2 <--uart--> PN532Killer2(tag emulator)

###Devices:

![NFC Realy Reader-Tag-Half](https://github.com/user-attachments/assets/d9af2d87-4cbf-48e2-94da-98c631ce651d)


###Demo video(Phone read Ntag215, App TagInfo):



https://github.com/user-attachments/assets/feacffe3-3a49-4efc-8bcb-78e733e99a6b



###Performance:

The yellow line indicates the PN532Killer tag emulator uart tx.
The purple line indicates the PN532Killer tag emulator uart rx.
The FDT is about 5-7ms.

![NFC Relay FDT](https://github.com/user-attachments/assets/8385b77c-8824-4429-8d64-7ab47a677f41)
