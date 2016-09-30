---
layout: articles
title:  "How to calibrate a continous rotation servo using NanoPlayBoard"
subtitle: ""
date:   2016-09-30 00:00:00
author: "José Juan Sánchez"
categories: articles
header-img: "resources/images/header-bg.png"
---

## Inventory

<a href="#">
    <img class="img-responsive" src="{{ site.baseurl }}/resources/images/bluetooth_beach.jpg" alt="Post Sample Image">
</a>

* NanoPlayBoard.
* 9v battery.
* Continous rotation servo.
* Screwdriver.

## Sketch
Upload this sketch on the NanoPlayBoard:

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.potentiometer.scaleTo(0, 180);
  board.ledmatrix.printInLandscape(value);
  board.servo[1].to(value);
}
```

The source code of this sketch is [available on GitHub][1].

## Set up connections



[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library