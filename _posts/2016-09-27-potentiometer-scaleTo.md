---
layout: examples
title-list:  "scaleTo"
title:  "Potentiometer - scaleTo"
subtitle: "How to scale potentiometer values"
date:   2016-09-27 00:02:00
author: "José Juan Sánchez"
categories: [examples, potentiometer]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to read potentiometer values and scale it to another range.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.potentiometer.scaleTo(0, 99);
  board.ledmatrix.printInLandscape(value);
  delay(100);
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples