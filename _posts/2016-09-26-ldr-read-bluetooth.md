---
layout: examples
title-list:  "read"
title:  "LDR - read"
subtitle: "How to send LDR values through Bluetooth"
date:   2016-09-26 00:01:00
author: "José Juan Sánchez"
categories: [examples, ldr]
header-img: "resources/images/header-bg.png"
---

## read
This example shows how to read potentiometer values and send it through `Bluetooth`.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void loop() {
  int value = board.ldr.read();
  board.bluetooth.println(value);
  delay(100);
}
```

The source code of this example is [available on GiHub][1].

## Image
<a href="#">
    <img class="img-responsive" src="{{ site.baseurl }}/resources/images/bluetooth_beach.jpg" alt="Post Sample Image">
</a>

## Video
<iframe width="750" height="423"  src="https://www.youtube.com/embed/NiuZJAB38TI" frameborder="0" allowfullscreen></iframe>

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples