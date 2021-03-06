---
layout: examples
title-list:  "setIntensity"
title:  "RGB - setIntensity"
subtitle: "How to set the brightness of the LED"
date:   2016-09-27 00:03:00
author: "José Juan Sánchez"
categories: [examples, rgb]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to set the brightness of the LED.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {
  board.rgb.setColor("FF0000");
}

void loop() {
  int intensity = board.potentiometer.scaleTo(0, 99);
  board.rgb.setIntensity(intensity);
  board.ledmatrix.printInLandscape(intensity);
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples