# I2C OLED 128x64 with added polish fonts (beta)

makecode I2C OLED 128x64 extension for micro:bit.  
Origin code from https://github.com/makecode-extensions/OLED12864_I2C 
Part of the drive base on fizban99's microbit OLED driver:  
https://github.com/fizban99/microbit_ssd1306  

## Basic usage

```
let item = 0
OLED12864_I2C.init(120)
OLED12864_I2C.rect(0, 0, 60, 30, 1)
OLED12864_I2C.showString(0, 0, "Hello!", 1)
OLED12864_I2C.showString(0, 1, "1234567890", 0)
item = 0
basic.forever(() => {
    OLED12864_I2C.showNumber(0, 3, item, 1)
    item += 1
    basic.pause(1000)
}) 
```

## License

MIT

Copyright (c) 2018, microbit/micropython Chinese community  

## Supported targets

* for PXT/microbit

[Origin from microbit/micropython Chinese community](http://www.micropython.org.cn)
