# Мой новый сайт на MkDocs  

Добро пожаловать! Это пример сайта, созданного в PyCharm.  

## Возможности  
- Поддержка Markdown  
- Автоматическое обновление  
- Простота настройки  
- 
![Описание изображения](/img/uploads/img1.jpg)
<img src="/img/uploads/img1.jpg" alt="Описание изображения" class="my-image">
[О проекте](about.md)  

## Последние посты

{% for page in pages if "posts/" in page.url %}
- [{{ page.meta.title }}]({{ page.url }})  
{% endfor %}

[Все посты →](blog/)

<div id="latest-posts"></div>
<script src="js/load-posts.js"></script>