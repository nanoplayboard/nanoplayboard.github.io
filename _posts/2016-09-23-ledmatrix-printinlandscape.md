---
layout: examples
title-list:  "printInLandscape"
title:  "LED Matrix - printInLandscape"
subtitle: "How to display a number in landscape mode"
date:   2016-09-23 00:02:00
author: "José Juan Sánchez"
categories: [examples, ledmatrix]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to display a number on the LED dot matrix in landscape mode.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int number = board.potentiometer.scaleTo(0, 99);
  board.ledmatrix.printInLandscape(number);
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples