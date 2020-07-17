---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Altium Designs"
summary: "A demo of electronic Boards I have designed for several projects"
authors: []
tags: [hardware, Altium, Embedded System, ARM, STM32]
categories: []
date: 2020-07-11T18:16:49-05:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Here are the samples of boards I have designed for different projects : 

1. I Designed this board as an assistant for the Robotics principles course. The student will then try to balance Inverted Pendulum Robot:
Specifications
* STM32F103X
* I2C, PWM, SPI, External Interrupt, Timers, UART.


{{< gallery >}}
{{< figure link="hw-designs/ipr/iprrobot-schem.png" caption="Inversed pendulum robot schematic" >}}
{{< figure link="hw-designs/ipr/iprrobot2d.png" caption="Inversed pendulum robot design" >}}
{{< figure link="hw-designs/ipr/iprrobot3d.png" caption="Inversed pendulum robot 3d" >}}
{{< /gallery >}} {{< load-photoswipe >}}

2. basic Magnetic Tracker Test Board : 

* STM32F4X
* LIS3MDL, USB, UART, SPI, etc.

{{< gallery >}}
{{< figure link="hw-designs/bionichand/v1/1.png" caption="Magnet Tracker design" >}}
{{< figure link="hw-designs/bionichand/v1/2.png" caption="Magnet Tracker 3d-front" >}}
{{< figure link="hw-designs/bionichand/v1/3.png" caption="Magnet Tracker 3d-back" >}}
{{< /gallery >}} {{< load-photoswipe >}}

3. Mainboard and sensor board designs for magnetic localization. This design used to test different 3d sensor arrangements  

* STM32F4X
* WIZNET5500
* USB, UART, SPI,etc.

{{< gallery >}}
{{< figure link="hw-designs/bionichand/v2/1.png" caption="Magnet Tracker 24 sensors design" >}}
{{< figure link="hw-designs/bionichand/v2/2.png" caption="Magnet Tracker mainboard 24 sensors 3d" >}}
{{< figure link="hw-designs/bionichand/v2/3.png" caption="lis3mdl breakout 3d" >}}
{{< /gallery >}} {{< load-photoswipe >}}


4. Mainboard for static sensor design for Magnetic Localization Project  

{{< gallery >}}
{{< figure link="hw-designs/bionichand/v3/1.png" caption="Magnet Tracker 24 sensors design" >}}
{{< figure link="hw-designs/bionichand/v3/2.png" caption="Magnet Tracker mainboard 24 sensors 3d" >}}
{{< figure link="hw-designs/bionichand/v3/3.png" caption="lis3mdl breakout 3d" >}}
{{< /gallery >}} {{< load-photoswipe >}}


4. Other Designs For Bionic Hand :  

{{< gallery >}}
{{< figure link="hw-designs/bionichand/v4/1.jpg" caption="This board was designed to test Magnet Localization after implanting Magnet inside Person's Hand." >}}
{{< figure link="hw-designs/bionichand/v4/2.jpg" caption="This board was designed to test Magnet Localization after implanting Magnet inside Person's Hand - feedback through LEDs" >}}
{{< figure link="hw-designs/bionichand/v4/3.jpg" caption="initial Modular board designs for attaching around Handicaped Person(Test designs)" >}}
{{< figure link="hw-designs/bionichand/v4/4.jpg" caption="initial Modular board designs for attaching around Handicaped Person(Test designs)" >}}
{{< figure link="hw-designs/bionichand/v4/5.jpg" caption="initial Modular board designs for attaching around Handicaped Person(Test designs)" >}}
{{< /gallery >}} {{< load-photoswipe >}}

5. Other Designs :

{{< gallery dir="hw-designs/other" caption-effect="fade" hover-effect="grow" />}} {{< load-photoswipe >}}

