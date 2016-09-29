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

The source code of this example is [available on GiHub][1].

## Image
<a href="#">
    <img class="img-responsive" src="{{ site.baseurl }}/resources/images/bluetooth_beach.jpg" alt="Post Sample Image">
</a>

## Video
<iframe width="100%" height="423" src="https://www.youtube.com/embed/NiuZJAB38TI" frameborder="0" allowfullscreen></iframe>

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples