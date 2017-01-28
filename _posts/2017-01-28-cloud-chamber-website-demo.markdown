---
layout: post
title:  "Cloud Chamber Website Demo"
date:   2017-01-28 21:42:21 +0100
categories:
---
This is a demo post, to showcase features.

Demo python code:

{% highlight python  %}
import cv2

# read demo image
img = cv2.imread('/home/bence/cc2.jpg', 0)

# erosion -> dilation
median = cv2.medianBlur(img, 5)
# binary thresholding
ret, thresh1 = cv2.threshold(median, 200, 255, cv2.THRESH_BINARY)

# save file
cv2.imwrite('binarycc2.jpg', thresh1)
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
