---
layout: examples
title-list:  "scaleTo"
title:  "LDR - scaleTo"
subtitle: "How to scale LDR values"
date:   2016-09-26 00:02:00
author: "José Juan Sánchez"
categories: [examples, ldr]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to read LDR values and scale it to another range.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.ldr.scaleTo(0, 99);
  board.ledmatrix.printInLandscape(value);
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples