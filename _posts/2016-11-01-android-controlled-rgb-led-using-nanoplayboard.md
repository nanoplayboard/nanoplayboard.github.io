---
layout: articles
title:  "Android controlled RGB LED using NanoPlayBoard and Bluetooth"
subtitle: ""
date:   2016-11-01 00:00:00
author: "José Juan Sánchez"
categories: articles
header-img: "resources/images/header-bg.png"
---

This article shows you how to control an RGB LED using an Android device, **NanoPlayBoard** and HC-05 Bluetooth module.

## Inventory

<a href="#">
    <img class="img-responsive" src="{{ site.baseurl }}/resources/articles/android-controlled-rgb-led/img-00.jpg" alt="Inventory">
</a>

* NanoPlayBoard.
* 9v battery.
* HC-05 Bluetooth module.
* Android device.
* Paper box (made with an A4 paper).

## Sketch
Upload the sketch: [firmaware_bluetooth.ino][1] on the **NanoPlayBoard**:

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {
  btSerial.begin(9600);
}

void loop() {
  btSerialEvent();
  doMessageAction();
}

...
```

```c++
void doMessageAction() {
  switch(message_id) {
    ...
    case ID_RGB_SET_COLOR:
      rgbSetColor();
      break;
    ...
  }
}
```

```c++
void rgbSetColor() {
  if (json.length() <= 0) return;

  StaticJsonBuffer<200> json_buffer;
  JsonObject& root = json_buffer.parseObject(json);

  if (!root.success()) {
    btSerial.println("{\"error\": \"Error parsing json message\"}");
    return;
  }

  int r = root["r"];
  int g = root["g"];
  int b = root["b"];

  board.rgb.setColor(r, g, b);
}
```

The source code of this sketch is [available on GitHub][1].

## Android App

### UI

<img class="img-responsive" src="{{ site.baseurl }}/resources/articles/android-controlled-rgb-led/img-01.jpg" alt="Inventory">

## Video
<iframe width="100%" height="423" src="https://www.youtube.com/embed/5EVmYEs8DxE" frameborder="0" allowfullscreen></iframe>

## Resources
* [NanoPlayBoard Arduino Library][2].
* [NanoPlayBoard Android App][3].

[1]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library/blob/master/examples/13.android/firmware_bluetooth/firmware_bluetooth.ino
[2]: https://github.com/josejuansanchez/NanoPlayBoard-Arduino-Library
[3]: https://github.com/josejuansanchez/NanoPlayBoard-Android-App