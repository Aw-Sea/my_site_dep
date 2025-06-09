# Жить! Помнить! Знать!

<div style="text-align: center; margin-bottom: 40px;">
  <img src="static/img/logo.jpg" alt="Логотип" style="max-width: 200px;">
  <p style="font-size: 1.2em; color: #d32f2f;">Сохранение памяти о героях Великой Отечественной войны и Специальной военной операции</p>
</div>

<div class="grid cards" style="margin-bottom: 30px;">
  <div class="grid-item">
    <h2>О проекте</h2>
    <p>Наш проект посвящен сохранению исторической памяти о подвиге советского народа в Великой Отечественной войне 1941-1945 гг. и героях современной Специальной военной операции.</p>
    <p>Мы собираем, систематизируем и публикуем материалы о:</p>
    <ul>
      <li>Памятниках и мемориалах</li>
      <li>Воинских захоронениях</li>
      <li>Героях прошлого и настоящего</li>
      <li>Исторических маршрутах</li>
    </ul>
  </div>
  <div class="grid-item">
    <img src="static/img/rodina.jpg" alt="Родина-мать" style="border-radius: 8px; max-width: 100%;">
  </div>
</div>

## Основные разделы

<div class="grid cards" style="margin-top: 20px;">
  <div class="grid-item" onclick="location.href='blog';" style="cursor: pointer;">
    <h3><i class="fas fa-newspaper"></i> Новости</h3>
    <p>Актуальные события, мероприятия и публикации</p>
  </div>

  <div class="grid-item" onclick="location.href='monuments';" style="cursor: pointer;">
    <h3><i class="fas fa-landmark"></i> Памятники и памятные места</h3>
    <p>Мемориалы Великой Отечественной войны и СВО с описанием и фотографиями</p>
  </div>

  <div class="grid-item" onclick="location.href='wargraves';" style="cursor: pointer;">
    <h3><i class="fas fa-cross"></i> Военные захоронения</h3>
    <p>База данных мест захоронений воинов с возможностью поиска</p>
  </div>

  <div class="grid-item" onclick="location.href='facesofvictory';" style="cursor: pointer;">
    <h3><i class="fas fa-star"></i> Лица Победы</h3>
    <p>Истории ветеранов Великой Отечественной войны</p>
  </div>

  <div class="grid-item" onclick="location.href='heroes';" style="cursor: pointer;">
    <h3><i class="fas fa-medal"></i> Герои СВО</h3>
    <p>Подвиги участников Специальной военной операции</p>
  </div>

  <div class="grid-item" onclick="location.href='map';" style="cursor: pointer;">
    <h3><i class="fas fa-route"></i> Туристический маршрут "Пенза"</h3>
    <p>Интерактивная карта памятных мест Пензенской области</p>
  </div>

  <div class="grid-item" onclick="location.href='videohistory';" style="cursor: pointer;">
    <h3><i class="fas fa-video"></i> Видеоистория</h3>
    <p>Документальные фильмы и интервью с ветеранами</p>
  </div>

  <div class="grid-item" onclick="location.href='about';" style="cursor: pointer;">
    <h3><i class="fas fa-users"></i> Наша команда</h3>
    <p>Организаторы проекта и волонтеры</p>
  </div>
</div>

## Цифры памяти

<div class="grid cards" style="text-align: center;">
  <div class="grid-item">
    <h1>27 млн</h1>
    <p>погибших в Великой Отечественной войне</p>
  </div>
  <div class="grid-item">
    <h1>34 тыс</h1>
    <p>памятников и мемориалов в России</p>
  </div>
  <div class="grid-item">
    <h1>500+</h1>
    <p>героев Специальной военной операции</p>
  </div>
</div>

<style>
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
}

.grid-item {
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  padding: 20px;
  transition: transform 0.3s, box-shadow 0.3s;
}

.grid-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0,0,0,0.1);
}

.cards h3 i {
  margin-right: 10px;
  color: #d32f2f;
}
</style>
## Последние посты

{% for page in pages if "posts/" in page.url %}
- [{{ page.meta.title }}]({{ page.url }})  
{% endfor %}

[Все посты →](blog/)

<div id="latest-posts"></div>
<script src="js/load-posts.js"></script>