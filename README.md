# OpenOCD config for clone STM32F103C8T8 microcontoler CS32F103C8T6 (CKSF103C8T6)

## English note
If you purchased a clone of the stm32f103c8t8 microcontroller such as CS32F103C8T6 (CKSF103C8T6) (https://aliexpress.ru/item/32525208361.html), when trying to work with them through OpenOCD, an error may appear when trying to fill in the code or debugging (SWD).

```
An : UNEXPECTED rcode: 0x2ba01477
Error: expected 1 of 1: 0x1ba01477
in procedure 'program'
** OpenOCD init failed **
shutdown command invoked
```

This is fixed by specifying the correct configuration file for OpenOCD.
This repository contains configuration files for this type of microcontroller.

To ensure correct operation, you must copy the files from the repository to the directory with OpenOCD installed and correctly specify the desired configuration file (cs32f103c8_blue_pill(stlink).cfg). After that, everything works correctly.

## Russian note
Если вы приобрели клон микроконтроллера STM32F103C8T8 такие как CS32F103C8T6 (CKSF103C8T6) (https://aliexpress.ru/item/32525208361.html), то при попытке работы с ними через OpenOCD может появляться ошибка при попытке заливки кода или отладке (SWD).

```
Warn : UNEXPECTED idcode: 0x2ba01477
Error: expected 1 of 1: 0x1ba01477
in procedure 'program'
** OpenOCD init failed **
shutdown command invoked
```

Исправляется это путем указания правильного конфигурационного файла для OpenOCD.
В данном репозитарии расположены конфигурационные файлы для данного типа микроконтроллера.

Для обеспечения корректной работы необходимо скопировать файлы из репозитория в директорию с установленным OpenOCD и правильно указать нужный конфигурационный файл (cs32f103c8_blue_pill(stlink).cfg). После этого все работает корректно.
