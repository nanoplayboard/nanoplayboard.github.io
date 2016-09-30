---
layout: articles
title:  "How to calibrate a continous servo using NanoPlayBoard"
subtitle: ""
date:   2016-09-30 00:00:00
author: "José Juan Sánchez"
categories: articles
header-img: "resources/images/header-bg.png"
---

## Sketch
You'll find this post in your `_posts` directory - edit this post and re-build (or run with the `-w` switch) to see your changes!
To add new posts, simply add a file in the `_posts` directory that follows the convention: YYYY-MM-DD-name-of-post.ext.

Jekyll also offers powerful support for code snippets:

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

The source code of this sketch is [available on GiHub][1].

## Header 2
<p>Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center — an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.</p>

<a href="#">
    <img class="img-responsive" src="{{ site.baseurl }}/resources/images/bluetooth_beach.jpg" alt="Post Sample Image">
</a>

<p>Science cuts two ways, of course; its products can be used for both good and evil. But there's no turning back from science. The early warnings about technological dangers also come from science.</p>

### Header 3
<p>What was most significant about the lunar voyage was not that man set foot on the Moon but that they set eye on the earth.</p>

<p>A Chinese tale tells of some men sent to harm a young girl who, upon seeing her beauty, become her protectors rather than her violators. That's how I felt seeing the Earth for the first time. I could not help but love and cherish her.</p>


[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library