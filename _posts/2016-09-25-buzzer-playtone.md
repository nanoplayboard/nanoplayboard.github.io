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

void loop() {
  int value = board.potentiometer.read();
  board.buzzer.playTone(value);
  delay(100); 
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