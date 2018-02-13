The original firmware and eeprom blobs are saved here as:

  stock-ctc-gt2560-eeprom.raw
  stock-ctc-gt2560-flash.raw

They may each be restored to the printer using the respective line or lines:

$ avrdude -c wiring -P /dev/ttyUSB0 -p m2560 -b 57600 -D -U flash:w:flash.raw:r
$ avrdude -c wiring -P /dev/ttyUSB0 -p m2560 -b 57600 -D -U eeprom:w:eeprom.raw:r
