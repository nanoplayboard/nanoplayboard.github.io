---
layout: examples
title-list:  "toggle"
title:  "RGB - toggle"
subtitle: "How to toggle the current state of the LED"
date:   2016-09-27 00:04:00
author: "José Juan Sánchez"
categories: [examples, rgb]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to toggle the current state of the LED.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  board.rgb.toggle();
  delay(1000);
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples