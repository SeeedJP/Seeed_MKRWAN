# Firmware Update

1. Generate **fw.h** from **cmwx1zzabz_0xx.bin**.

    ```
    mv cmwx1zzabz_0xx.bin mlm32l07x01.bin
    echo -n "const " > fw.h && xxd -i mlm32l07x01.bin >> fw.h
    ```

1. Open **MKRWANFWUpdate_standalone.ino** in Arduino IDE.

1. Compile and Upload in Arduino IDE.

1. Open Serial Monitor.
