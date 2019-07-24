Kendryte K210 SDK with FreeRTOS
======

This SDK is for Kendryte K210 which contains FreeRTOS support. <br> 
Ported from [Kendryte `kendryte-freertos-sdk`](https://github.com/kendryte/kendryte-freertos-sdk)

## Changes to make the SDK work better with MicroPython, but can be used as SDK for other applications to

_**The following files were modified:**_

* lib/bsp/
  * `printf.c`
  * device/
    * `rtc.cpp`
    * `uart.cpp`
    * `gpiohs.cpp`
* lib/arch/include/
  * `encoding.h`
* lib/drivers/src/storage/
  * `sdcard.cpp`
* lib/utils/include/
  * `syslog.h`
* lib/freertos/
  * include/
    * `task.h`
    * `devices.h`
    * `FreeRTOS.h`
    * `filesystem.h`
    * `portabe.h`
  * kernel/
    * `devices.cpp`
    * storage/
      * `filesystem.cpp`
  * conf/
    * `FreeRTOSConfig.h`
  * portable/
    * `port.c`
    * `portmacro.h`
    * `heap_4.c`
* third_party/
  * lwip/
    * src/
      * `Filelist.cmake`
      * include/
        * netif/
          * ppp/
            * `ppp_opts.h`
  * fatfs/
    * source/
      * `ffconf.h`

