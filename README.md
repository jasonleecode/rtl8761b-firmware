如果你的环境是ubuntu20.04及以上的，直接将这几个固件复制到/lib/firmware/rtl_bt/下，重新插拔适配器即可，然后dmesg看一下硬件挂载情况
```
[1385139.337770] usb 1-7: new full-speed USB device number 7 using xhci_hcd
[1385139.486549] usb 1-7: New USB device found, idVendor=0bda, idProduct=8771, bcdDevice= 2.00
[1385139.486559] usb 1-7: New USB device strings: Mfr=1, Product=2, SerialNumber=3
[1385139.486564] usb 1-7: Product: Bluetooth Radio
[1385139.486567] usb 1-7: Manufacturer: Realtek
[1385139.486570] usb 1-7: SerialNumber: 00E04C239987
[1385139.489444] Bluetooth: hci0: RTL: examining hci_ver=0a hci_rev=000b lmp_ver=0a lmp_subver=8761
[1385139.490529] Bluetooth: hci0: RTL: rom_version status=0 version=1
[1385139.490540] Bluetooth: hci0: RTL: loading rtl_bt/rtl8761bu_fw.bin
[1385139.490675] Bluetooth: hci0: RTL: loading rtl_bt/rtl8761bu_config.bin
[1385139.490735] Bluetooth: hci0: RTL: cfg_sz 6, total sz 27814
[1385139.630602] Bluetooth: hci0: RTL: fw version 0x09a98a6b
[1385139.714576] NET: Registered PF_ALG protocol family
[1385139.759420] Bluetooth: RFCOMM TTY layer initialized
[1385139.759430] Bluetooth: RFCOMM socket layer initialized
[1385139.759442] Bluetooth: RFCOMM ver 1.11

```

如果你的环境是ubuntu20.04以下，则需要修改的东西比较多，可以参考我的博客
https://blog.csdn.net/avatar1912/article/details/120851889
