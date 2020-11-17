---
date: 2020-11-14 12:26:40
layout: post
title: Afraid of SQL Injections
subtitle: Eye4AnEye
description: A system to detect cataracts using image processing.
image: /assets/img/teams/sql.png
optimized_image: /assets/img/teams/sql.png
category:
tags:
  - 4th place
author: fchacks
---
Problem

Living in a country which has the second highest population of senior citizens and having close ophthalmologist relatives I know the struggles our country is experiencing when talking about vision problems, and especially nowadays with the corona virus lurking among us it is quite difficult for senior citizens to resolve their vision problems. Thus I made this easy-to-use app in order to facilitate procedures regarding the ophthalmology sector and further improve the current healthcare state.

Algorithm

Eye4AnEye uses two libraries for image recognition, opencv-python and numpy. For cataract detection the image is firstly resized and then it is converted from the common BGR colour scheme into HSV colour scheme as it is easier to apply a mask which covers any unwanted pixels. It is later converted back into BGR as it is easier to process colour data  through iteration. Through iteration we detect all the pixels that their BGR values are included in a specified range. Finally we divide the pixels by the total amount of pixels contained in our image and we multiply that function by 1000 to get the ‰. If that ‰ is above a certain threshold we can come to the conclusion that this person has cataract. Our Blood presence algorithm works in a similar way just without the conversions as red is not a very light or sensitive colour.

Possible Improvements

More features can be added, for instance glaucoma or pterygium support can be added. Additionally the algorithm can become way more accurate by using artificial intelligence and neural networks (such as NEAT). And last but not least live feed and instant share support can be added to avoid complications with our output file.

Conclusion
Eye4AnEye uses an image recognition algorithm to detect cataract or extreme blood presence in our eyes. Consequently we have reduced and automated the diagnosis process for such vision problems while simultaneously reducing the need for special equipment.

<a href="https://github.com/DonaldDuck780/Eye4AnEye">Code File</a><br>
<a href="https://youtu.be/xwnpviH2yRY">Project Video</a>

Creator: Evangelopoulos (Greece)
