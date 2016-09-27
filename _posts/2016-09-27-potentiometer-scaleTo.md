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

## scaleTo
This example shows how to read potentiometer values and scale it to another range.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {
  Serial.begin(9600);
}

void loop() {
  int value = board.potentiometer.read();
  Serial.println(value);
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