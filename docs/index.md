# Мой новый сайт на MkDocs  

Добро пожаловать! Это пример сайта, созданного в PyCharm.  

## Возможности  
- Поддержка Markdown  
- Автоматическое обновление  
- Простота настройки  

[О проекте](about.md)  

## Последние посты

{% for page in pages if "posts/" in page.url %}
- [{{ page.meta.title }}]({{ page.url }})  
{% endfor %}

[Все посты →](blog/)

<div id="latest-posts"></div>
<script src="js/load-posts.js"></script>