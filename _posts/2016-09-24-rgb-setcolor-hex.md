---
layout: examples
title-list:  "setColor"
title:  "RGB - setColor"
subtitle: "How to set the LED color using a HEX value"
date:   2016-09-27 00:01:00
author: "José Juan Sánchez"
categories: [examples, rgb]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to set the LED color using a HEX value.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  board.rgb.setColor("#FF0000");
  delay(1000);
  board.rgb.setColor("#00FF00");
  delay(1000);
  board.rgb.setColor("#0000FF");
  delay(1000);
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples