---
layout: examples
title-list:  "read"
title:  "Potentiometer - read"
subtitle: "How to send potentiometer values through <i>Bluetooth</i>"
date:   2016-09-27 00:01:00
author: "José Juan Sánchez"
categories: [examples, potentiometer]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to read potentiometer values and send it through `Bluetooth`.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.potentiometer.read();
  board.bluetooth.println(value);
  delay(100);
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples