# linux-configuration
Some scripts and files to get my laptop running

# ASUS T100HA
The device is a cherry trail 2-in-1 which runs nearly flawlessly with the new 4.19 Kernel in Manjaro Linux
It needs a monitor.conf to have correct display rotation (autoration is also possible, but not interesting for me, so not configured).
The HCD is the firmware required to use Bluetooth, just copy to `/lib/firmware/brcm` There also needs to be a second file there:
```shell
sudo cp /sys/firmware/efi/efivars/nvram-74b00bd9-805a-4d61-b51f-43268123d113 /lib/firmware/brcm/brcmfmac43340-sdio.txt
```
