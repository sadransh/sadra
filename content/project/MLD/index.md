---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Magnetic Localization Device"
summary: "Muscle Movement Tracking through Implanted Magnet(s)"
authors: []
tags: [machinelearning,software]
categories: [optimization , LIS3MDL , ARM, STM32, Matlab, Genetic Algorithm, robotics,hardware, machinelearning]
date: 2020-07-11T00:54:32-05:00

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

Unfortunately, At the moment, I am not allowed to upload related information on the latest results. I will publish related photos as soon as I am allowed to do so.

## Background
------

The primary motivation for starting the project "Magnetic Localization Device" was implementing the novel idea of detecting muscle movements through implanted magnet(s). The final interface will be used as the control interface of [FUM-Bionic-Hand]({{< ref "/project/FUM-Bionic-Hand/index.md" >}}) III+ versions.

## My Contributions to Magnetic Localization projects
------


In February 2016, the first steps of the magnetic localization were taken. We started with low-cost Hall effect sensors called ugn3503. A 2D Bluetooth sensor array and a C# GUI designed for demonstration. As shown in the below pictures, the sensor array board is powered by STM32F103X microcontroller, 16 UGN3503 sensors connected, which are working with ADC on Direct Memory Access(DMA), and Uart Connection for wireless data transmission.


* Goal: first impression on sensors' sensitivity and other characteristics.
* 16 1-axis Hall-effect sensors ( UGN3503 )
* powered by 32-bit ARM microcontroller stm32f103X 
*	low pass analog filters(anti-aliasing) and digital low-pass filtering
* USB COM and UART Bluetooth communication
* C# GUI for demonstrating localization results.
* Using weighted average for estimating magnet's position based on SNR.

**Calibration:** 
* Precise sensors' location measured with Solidworks.
* Gain, Offset, and sensor's location calibrated.
* Logged sensor output in Matlab for further processing.

{{< gallery >}}
{{< figure link="BionicHand/MagnetLogger.png" caption="basic GUI for Magnet(1)" >}}
{{< figure link="BionicHand/MagnetLogger2.png" caption="basic GUI for Magnet(2)" >}}
<!-- {{< figure link="/img/arduino/test-setup.jpg" caption="Arduino test setup" >}} -->
{{< /gallery >}} {{< load-photoswipe >}}


{{< gallery >}}
{{< figure link="hw-designs/bionichand/v1/1.png" caption="Magnet Tracker design" >}}
{{< figure link="hw-designs/bionichand/v1/2.png" caption="Magnet Tracker 3d-front" >}}
{{< figure link="hw-designs/bionichand/v1/3.png" caption="Magnet Tracker 3d-back" >}}
{{< /gallery >}} {{< load-photoswipe >}}


During 2017 and 2018, other designs are performed: 





{{< gallery >}}
{{< figure link="hw-designs/bionichand/v2/1.png" caption="Magnet Tracker 24 sensors design" >}}
{{< figure link="hw-designs/bionichand/v2/2.png" caption="Magnet Tracker mainboard 24 sensors 3d" >}}
{{< figure link="hw-designs/bionichand/v2/3.png" caption="lis3mdl breakout 3d" >}}
{{< /gallery >}} {{< load-photoswipe >}}


Characteristics: 
* 32-bit STM32F4X series microcontroller. 
* SPI bus with 8 to 10 sensors on each bus. 
* Intrruped-based Data reading from each sensor with 1K Timer
* Using USB Communication for Data Transmission


{{< gallery >}}
{{< figure link="hw-designs/bionichand/v3/1.png" caption="Magnetic Tracker 30 sensors schematic" >}}
{{< figure link="hw-designs/bionichand/v3/2.png" caption="Magnetic Tracker design with 30 sensors 2d" >}}
{{< figure link="hw-designs/bionichand/v3/3.png" caption="Magnetic Tracker 3d" >}}
{{< figure link="hw-designs/bionichand/v3/4.png" caption="final board " >}}
{{< /gallery >}} {{< load-photoswipe >}}


* STM32F4X series microcontroller.
* Transfer data over Ethernet using WIZNET5500 for high-frequency data logging over **20 Mb/s** 
* Calibrating sensors data ( Gain, Offset, cross-axis Gain).
* Calibrating sensors' positions and orientations. 
* Implementing the mathematical model of the problem in Matlab.
* Simulation of the real problem in Matlab.
* Solving problem with LM, Fmincon, and other optimizations in Matlab.
* Processing of real data in Matlab.
* Localizing and tracking up to 2 magnets with minimum localization error.




Also, Test Setup Robot was used to move Magnets accurately, which has 3 stepper motors and works with Marlin Driver.
{{< gallery >}}
{{< figure link="project/mld/featured.jpg" caption="The TestSetup Robot" >}}
{{< /gallery >}} {{< load-photoswipe >}}

Results to the end I was working with the team are presented in papers links of which are in ending section of this page



This project is performed during my undergraduate studies in Advanced robotics Lab @ Ferdowsi University of Mashhad, Iran. Supervisors are Prof. Alireza Akbarzadeh tootoonchi, Dr. Mojtaba Izadi.


-----

Related links : 

* [Design and Implementation of a Multiple Magnet Tracking System]({{< ref "/publication/mld/index.md" >}})
* [Robust Real-time Magnetic-based Object Localization to Sensor’s Fault using Recurrent Neural Networks]({{< ref "/publication/8964748/index.md" >}})
