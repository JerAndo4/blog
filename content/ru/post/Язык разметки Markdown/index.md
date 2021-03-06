---
title: Язык разметки Markdown
subtitle: Сегодня мы поговорим о языке разметки Markdown

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

*Markdown - это язык разметки текстов. Такие тексты легко писать и читать. Они могут быть легко преобразованы в HTML. Большинство программистов предпочитают Markdown для написания документации, описания своих проектов, ведения блогов и так далее.*

## **Что это значит?**

"Язык разметки" - это всего лишь набор соглашений, правил.

Допустим, вы общаетесь с другом по SMS. Вы не можете сделать текст в них жирным или наклонным. Вы согласны с другом: если я напишу *что-то* так между звездочками, то считайте это наклонным текстом. И если я напишу ** что-то ** между двумя звездочками, то считайте это жирным шрифтом. Ты придумал правила.

Markdown - это набор аналогичных правил.

## **Почему это необходимо?**

1. Добавить разметку в тех местах, где реальная разметка невозможна. Например, в простом текстовом файле или в том же SMS, где невозможно выделить жирным шрифтом, создать заголовки, выделить кавычки и т.д.

2. Для более удобного написания текстов для последующего преобразования в HTML или другие форматы.

## **Синтаксис Markdown**

Это краткое описание основных элементов синтаксиса Markdown. Единого стандарта не существует, и разные версии Markdown могут отличаться в деталях. Но основные элементы из приведенного ниже списка поддерживаются во всех стандартах.

#### **Выделение текста**

  **Этот текст будет выделен наклонным шрифтом (курсивом).*  * 

_ _Этот текст будет выделен наклонным шрифтом (курсивом)_ _

  ** **Этот текст будет выделен жирным шрифтом** **

__ __This text will be bold__ __

_ _Можно  ** **вставить** ** один тип в другой_ _


#### **Заголовки**
	#Это самый большой заголовок, он превращается в тег <h1>

	##<h2>

	###<h3>

	####<h4>

	#####<h5>
	
	######<h6>

#### **Ссылки**
https://github.com — текст простой ссылки автоматически станет кликабельной ссылкой

Любой текст можно сделать ссылкой:

[Это ссылка на GitHub](https://github.com )

#### **Цитата**

> (>)Это мудрая цитата

> (>)Мудрый человек.

Пишите без скобок!!!

#### **Списки**
Ненумерованный список:

* Пункт (*)

* Еще один пункт (*)

	* Подпункт  (Tab + *)

	* Еще один подпункт (Tab + *)

Пишите без скобок и перед абзацами!!!

Для подпунктов используйте TAB

#### **Нумерованный список:**

1. Пункт

1. Еще один момент

	1. Подпункт

	1. Еще один подпункт
	
Для подпунктов используйте TAB

Вы можете использовать любые цифры в нумерованном списке — это не имеет значения. При преобразовании в HTML или другой формат числа станут правильными и последовательными (1, 2, 3 и т.д.).















