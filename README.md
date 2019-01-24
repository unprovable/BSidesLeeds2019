# BSidesLeeds2019
Challenge firmware Repo for BSides Leeds 2019!

If you're seeing this, then you're here too early! Stuff will be uploaded on Thursday 24th ahead of the actual conference on 25th Jan...

http://bsidesleeds.co.uk/

To program, you need to make this command work:

`sudo python /root/.arduino15/packages/esp32/tools/esptool/2.3.1/esptool.py --chip esp32 --port /dev/ttyUSB0 --baud 921600 --before default_reset --after hard_reset write_flash -z --flash_mode dio --flash_freq 80m --flash_size detect 0xe000 boot_app0.bin 0x1000 bootloader_dio_80m.bin 0x10000 bsides-badge.ino.bin 0x8000 bsides-badge.ino.partitions.bin`
