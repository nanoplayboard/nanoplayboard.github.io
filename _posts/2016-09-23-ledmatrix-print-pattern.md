---
layout: examples
title-list:  "print"
title:  "LED Matrix - print"
subtitle: "How to display a pattern on the LED matrix"
date:   2016-09-23 00:01:00
author: "José Juan Sánchez"
categories: [examples, ledmatrix]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to display a pattern on the LED dot matrix.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  byte pattern[5] = {16, 72, 8, 72, 16};
  board.ledmatrix.print(pattern);  
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples