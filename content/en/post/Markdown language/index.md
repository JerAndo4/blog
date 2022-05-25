---
title: Markdown language
subtitle: Today we will talk about Markdown language

# Link this post with a project
projects: []

# Date published
date: '2022-05-08T00:00:00Z'

# Date updated
lastmod: '2022-05-08T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [https://3dnews.ru](https://3dnews.ru/944343/vishlo-krupneyshee-obnovlenie-dota-2-s-novim-geroem-monkey-king)'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - 2 week

categories:
  - post 2

---


*Markdown is a markup language for texts. Such texts are easy to write and read. They can be easily converted to HTML. Most programmers prefer Markdown for writing documentation, describing their projects, writing blogs, and so on.*

## **What does it mean?**

The "markup language" is just a set of conventions, rules.

Let's say that you communicate with a friend by SMS. You can't make the text bold or slanted in them. You agree with a friend: if I write * something* so between the asterisks, then consider it an oblique text. And if I write ** something ** between two asterisks, then consider it a bold text. You came up with the rules.

Markdown is a set of similar rules.

## **Why is this necessary?**

1. To add markup to places where real markup is not possible. For example, in a simple text file or in the same SMS, where it is impossible to highlight bold, create titles, highlight quotes, etc.

2. For more convenient writing of texts for subsequent conversion to HTML or other formats.

## **Markdown syntax**

This is a quick reference of the basic elements of the Markdown syntax. There is no single standard and different versions of Markdown may differ in details. But the basic elements from the list below are supported in all standards.

#### **Text Selection**

  **This text will be slanted (italics)*  * 

_ _This text will be slanted (italics)_ _

  ** **This text will be bold** **

__ __This text will be bold__ __

_ _It is possible to ** **insert** ** one type into another_ _


#### **Headings**

	#This is the largest header, it turns into a <h1> tag

	##<h2>

	###<h3>

	####<h4>

	#####<h5>
	
	######<h6>

#### **Links**
https://github.com — the text of a simple link will become a clickable link automatically

Any text can be made a link:

[This is a link to GitHub](https://github.com )

#### **Quote**

> (>)This is a wise quote

> (>)A wise man.

Write without brackets!!!

#### **Lists**
An unnumbered list:

* Item (*)

* One more point (*)

	* Sub-item (Tab + *)

	* One more sub-item (Tab + *)

Write without brackets and before paragraphs!!!

For sub-items, use TAB

#### **Numbered list:**

1. Item

1. One more point

	1. Sub-item

	1. One more sub-item
	
For sub-items, use TAB

You can use any numbers in the numbered list — it doesn't matter. When converted to HTML or another format, the numbers will become correct and consistent (1, 2, 3, etc.).
















