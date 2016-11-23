---
layout: examples
title-list:  "playTone"
title:  "Buzzer - playTone"
subtitle: "How to play tones on the buzzer"
date:   2016-09-26 00:02:00
author: "José Juan Sánchez"
categories: [examples, buzzer]
header-img: "resources/images/header-bg.png"
---

## Example
This example shows how to play tones on the buzzer.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.potentiometer.read();
  board.buzzer.playTone(value);
  delay(100); 
}
```

The source code of this example is [available on GitHub][1].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/tree/master/examples