---
layout: examples
title-list:  "read"
title:  "Potentiometer - read"
subtitle: "How to send potentiometer values through <i>serial port</i>"
date:   2016-09-27 00:00:00
author: "José Juan Sánchez"
categories: [examples, potentiometer]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to read potentiometer values and send it through the Arduino serial port, using the `Serial` class.

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

The source code of this example is [available on GitHub][1].

## Image
<a href="#">
    <img class="img-responsive" src="{{ site.baseurl }}/resources/images/bluetooth_beach.jpg" alt="Post Sample Image">
</a>

## Video
<iframe width="100%" height="423" src="https://www.youtube.com/embed/NiuZJAB38TI" frameborder="0" allowfullscreen></iframe>

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples