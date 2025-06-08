# Памятники и памятные места

<div class="cards-container">

<div class="card" onclick="this.classList.toggle('expanded')">
  <div class="card-header">
    <h3>Название памятника 1</h3>
  </div>
  <div class="card-content">
    <img src="images/monument1.jpg" alt="Памятник 1" style="max-width: 200px; float: left; margin-right: 15px;">
    <p><strong>Год установки:</strong> 1965</p>
    <p><strong>Автор:</strong> Иван Иванов</p>
    <p><strong>Адрес:</strong> г. Москва, ул. Примерная, 1</p>
    <div class="full-description">
      Полное описание памятника с историей его создания, значением и другими деталями.
      Можно добавить несколько абзацев текста.
    </div>
  </div>
</div>

<div class="card" onclick="this.classList.toggle('expanded')">
  <div class="card-header">
    <h3>Название памятника 2</h3>
  </div>
  <div class="card-content">
    <img src="images/monument2.jpg" alt="Памятник 2" style="max-width: 200px; float: left; margin-right: 15px;">
    <p><strong>Год установки:</strong> 1980</p>
    <p><strong>Автор:</strong> Петр Петров</p>
    <p><strong>Адрес:</strong> г. Москва, ул. Образцовая, 5</p>
    <div class="full-description">
      Подробное описание второго памятника с исторической справкой и интересными фактами.
    </div>
  </div>
</div>

</div>

<style>
.cards-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.card {
  border: 1px solid #ddd;
  border-radius: 8px;
  width: 300px;
  overflow: hidden;
  cursor: pointer;
  transition: all 0.3s ease;
}

.card-header {
  background-color: #f5f5f5;
  padding: 15px;
}

.card-content {
  padding: 15px;
  max-height: 200px;
  overflow: hidden;
  transition: max-height 0.3s ease;
}

.card.expanded .card-content {
  max-height: 1000px;
}

.full-description {
  margin-top: 15px;
  padding-top: 15px;
  border-top: 1px dashed #ccc;
}
</style>