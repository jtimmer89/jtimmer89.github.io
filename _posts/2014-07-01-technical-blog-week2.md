---
layout: post
title: "Technical Blog: CSS Spacing"
quote: Trying to wrap my mind around CSS spacing.
image: /media/technical-blogs/AutumnLake_14.jpg
video: false
---

#CSS spacing is easier than it looks

##Margin

{% include image.html url="/media/technical-blogs/cssbox.gif" width="60%" description="CSS guide for spacing" %}

Starting from the outermost of an html element, you have a css feature that will affect the positioning of other elements. This all makes sense when you realize that all elements in html are blocks. I have read that before but never understood it. It seemed so simple, but sometimes it takes a couple times before it clicks with wen development ideas. When you give some text header tags in html, it turns the white space around the text into a block. You can position this block and in turn the text with positioning as well as margin, borders, and padding. If you think of the outermost edge of the block as the border, you can add space between an element’s border and another element using margin. Let me illustrate.

{% include image.html url="/media/technical-blogs/websitenomargin.png" width="100%" description="No margin for header" %}

{% include image.html url="/media/technical-blogs/websitewithmargin.png" width="100%" description="Then I added 10px of margin, and you can see the space around the left and top edge" %}

##Border

The border principle is pretty straightforward. As we learned, each html element is a box, and we can add and play with the border around that box. Also, You can play with the size, color, and add the line feature (solid, dotted, dashed, double, groove, ridge, inset, outset). The following code would create a 10 pixel solid black line around the paragraphs in the html document:

```
  p { border: 10px solid black; }
```

##Padding

If we refer back up to the first picture, we can see that padding is the space around our content. If we added a large amount of padding, then added a border, that actual border box would ended up being far from the text or image. Padding and margin can be optimized with 4 characteristics: top, bottom, left, and right. There are two ways that you can adjust padding and margins. Let’s look at the different syntax for padding.

```
  padding-top: #px;
  padding-right: #px;
  padding-bottom: #px;
  padding-left: #px;
```

versus

```
  padding: #px #px #px #px;
```

###Well, that about covers it. Thanks for reading!