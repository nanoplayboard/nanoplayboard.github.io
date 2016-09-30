---
layout: examples
title-list:  "print"
title:  "LED Matrix - print"
subtitle: "How to display a scrolling text message on the LED matrix"
date:   2016-09-23 00:00:00
author: "José Juan Sánchez"
categories: [examples, ledmatrix]
header-img: "resources/images/header-bg.png"
---

## Example 1
This example shows how to display a scrolling text message on the LED dot matrix.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  board.ledmatrix.print("H o l a  m u n d o!");
}
```

## Example 2
The `setScrollSpeed`method allows you to control the scroll speed that is used to display the text on the LED dot matrix.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {
  board.ledmatrix.setScrollSpeed(10);
}

void loop() {
  board.ledmatrix.print("H o l a  m u n d o!");
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