---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Coral Image Segmentation"
summary: "a deep learning project for coral segmentation"
authors: []
tags: [software, deep-learning, segmentation, OpenCV, Tensorflow, Keras, Python]
categories: []
date: 2020-07-12T23:31:12-05:00

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


During the Spring of 2020, I utilized deep learning segmentation to do coral segmentation. I used a dataset of ~ 150 images of corals, which contains eight different categories.
* Pre-processed images using PIL and OpenCV and annotated. I used different techniques, including but not limited to, histogram equalization, white balance, color balance.
* I have done data augmentation because of the small size of the dataset. Methods used: cropping, rotation, mirror and etc.
* Dataset annotated carefully using labelme.
* Used different ResNet, U-Net, FCN, Vanilla CNN, and etc.
* Hyperparameter tuning.
* Segmented images of 8-different categories of corals with the accuracy of mIoU 60.1 %, considering the size of the dataset and the time I had, It's a good one. 