---
title: "SquareFox Documentation"
description: "Комплексная документация конфликтов и нарушений в игровом сообществе SquareFox"
date: 2025-12-17
aliases: ["/index", "/Главная"]
type: "index"
---

<style>
:root {
  --primary-bg: #1a1a1a;
  --secondary-bg: #2d2d2d;
  --text-primary: #e0e0e0;
  --text-secondary: #b0b0b0;
  --accent-color: #4a9eff;
  --warning-color: #ff6b6b;
  --success-color: #51cf66;
  --border-color: #404040;
  --card-bg: #252525;
  --shadow: rgba(0, 0, 0, 0.3);
}

[data-theme="light"] {
  --primary-bg: #ffffff;
  --secondary-bg: #f8f9fa;
  --text-primary: #212529;
  --text-secondary: #6c757d;
  --accent-color: #0d6efd;
  --warning-color: #dc3545;
  --success-color: #198754;
  --border-color: #dee2e6;
  --card-bg: #ffffff;
  --shadow: rgba(0, 0, 0, 0.1);
}

body {
  background-color: var(--primary-bg);
  color: var(--text-primary);
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  line-height: 1.6;
}

.index-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem;
}

.header {
  text-align: center;
  margin-bottom: 3rem;
  padding: 2rem;
  background: var(--card-bg);
  border-radius: 12px;
  box-shadow: 0 4px 20px var(--shadow);
}

.header h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  background: linear-gradient(135deg, var(--accent-color), #9c27b0);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.header p {
  font-size: 1.2rem;
  color: var(--text-secondary);
  margin-bottom: 1rem;
}

.quick-stats {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
  margin: 2rem 0;
}

.stat-card {
  background: var(--card-bg);
  padding: 1.5rem;
  border-radius: 8px;
  border-left: 4px solid var(--accent-color);
  box-shadow: 0 2px 10px var(--shadow);
}

.stat-number {
  font-size: 2rem;
  font-weight: bold;
  color: var(--accent-color);
}

.stat-label {
  color: var(--text-secondary);
  font-size: 0.9rem;
}

.table-of-contents {
  background: var(--card-bg);
  padding: 2rem;
  border-radius: 12px;
  margin-bottom: 2rem;
  box-shadow: 0 4px 20px var(--shadow);
}

.toc-tree {
  list-style: none;
  padding-left: 0;
}

.toc-tree li {
  margin: 0.5rem 0;
}

.toc-tree a {
  color: var(--accent-color);
  text-decoration: none;
  padding: 0.5rem 1rem;
  display: block;
  border-radius: 6px;
  transition: all 0.3s ease;
}

.toc-tree a:hover {
  background: var(--secondary-bg);
  transform: translateX(4px);
}

.category-section {
  margin: 3rem 0;
  background: var(--card-bg);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 20px var(--shadow);
}

.category-header {
  background: linear-gradient(135deg, var(--accent-color), #9c27b0);
  color: white;
  padding: 1.5rem 2rem;
  margin: 0;
}

.category-content {
  padding: 2rem;
}

.document-card {
  background: var(--secondary-bg);
  border: 1px solid var(--border-color);
  border-radius: 8px;
  padding: 1.5rem;
  margin: 1rem 0;
  transition: all 0.3s ease;
}

.document-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 25px var(--shadow);
}

.document-title {
  font-size: 1.3rem;
  font-weight: bold;
  color: var(--accent-color);
  margin-bottom: 0.5rem;
}

.document-meta {
  display: flex;
  gap: 1rem;
  margin-bottom: 1rem;
  font-size: 0.9rem;
  color: var(--text-secondary);
}

.document-description {
  color: var(--text-primary);
  margin-bottom: 1rem;
}

.document-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.tag {
  background: var(--accent-color);
  color: white;
  padding: 0.25rem 0.75rem;
  border-radius: 20px;
  font-size: 0.8rem;
  text-decoration: none;
  transition: all 0.3s ease;
}

.tag:hover {
  background: #3a8edd;
  transform: scale(1.05);
}

.search-container {
  background: var(--card-bg);
  padding: 2rem;
  border-radius: 12px;
  margin: 2rem 0;
  box-shadow: 0 4px 20px var(--shadow);
}

.search-input {
  width: 100%;
  padding: 1rem;
  border: 2px solid var(--border-color);
  border-radius: 8px;
  background: var(--secondary-bg);
  color: var(--text-primary);
  font-size: 1rem;
}

.search-input:focus {
  outline: none;
  border-color: var(--accent-color);
}

.filter-tabs {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-top: 1rem;
}

.filter-tab {
  background: var(--secondary-bg);
  color: var(--text-primary);
  border: 1px solid var(--border-color);
  padding: 0.5rem 1rem;
  border-radius: 20px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.filter-tab.active,
.filter-tab:hover {
  background: var(--accent-color);
  color: white;
  border-color: var(--accent-color);
}

.theme-toggle {
  position: fixed;
  top: 20px;
  right: 20px;
  background: var(--card-bg);
  border: 1px solid var(--border-color);
  border-radius: 50%;
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  box-shadow: 0 4px 15px var(--shadow);
  transition: all 0.3s ease;
}

.theme-toggle:hover {
  transform: scale(1.1);
}

@media (max-width: 768px) {
  .index-container {
    padding: 1rem;
  }
  
  .header h1 {
    font-size: 2rem;
  }
  
  .quick-stats {
    grid-template-columns: 1fr;
  }
  
  .filter-tabs {
    justify-content: center;
  }
  
  .theme-toggle {
    top: 10px;
    right: 10px;
    width: 40px;
    height: 40px;
  }
}

.backlinks-section {
  background: var(--card-bg);
  padding: 2rem;
  border-radius: 12px;
  margin: 2rem 0;
  box-shadow: 0 4px 20px var(--shadow);
}

.graph-view-placeholder {
  background: var(--secondary-bg);
  border: 2px dashed var(--border-color);
  border-radius: 8px;
  padding: 3rem;
  text-align: center;
  color: var(--text-secondary);
  margin: 2rem 0;
}

.highlight {
  background: var(--accent-color);
  color: white;
  padding: 0.2rem 0.4rem;
  border-radius: 4px;
}
</style>


  <div class="header">
    <h1>Разоблачения SquareFox</h1>
    <p>Полная документация конфликтов и нарушений в игровом сообществе</p>
    <p><strong>Создано:</strong> 29 ноября 2025 | <strong>Обновлено:</strong> 17 декабря 2025</p>
  </div>



  <div class="table-of-contents">
    <h2>📋 Содержание</h2>
    <ul class="toc-tree">
      <li><a href="#main-story">📖 История Арбуза</a></li>
      <li><a href="#serious-allegations">⚠️ Серьёзные обвинения</a></li>
      <li><a href="#admin-conflicts">👥 Конфликты с администрацией</a>
        <ul>
          <li><a href="#moderator-conflict">Конфликт с модератором</a></li>
          <li><a href="#milavi-conflict">Конфликт с Милави</a></li>
        </ul>
      </li>
      <li><a href="#ban-incidents">🚫 Бан инциденты</a>
        <ul>
          <li><a href="#mass-ban">Забаненная семёрка</a></li>
          <li><a href="#personal-ban">Личный бан Арбуза</a></li>
        </ul>
      </li>
      <li><a href="#financial-issues">💰 Лор за деньги</a></li>
      <li><a href="#moderation-issues">🛡️ Проблемы модерации</a></li>
      <li><a href="#timeline">📅 Хронология событий</a></li>
    </ul>
  </div>

  <div class="category-section" id="main-story">
    <h2 class="category-header">📖 История Арбуза</h2>
    <div class="category-content">
      <div class="document-card">
        <h3 class="document-title"><a href="Главная/Привет, я Арбуз.md">Привет, я Арбуз</a></h3>
        <div class="document-meta">
          <span>📅 Сентябрь - Декабрь 2025</span>
        </div>
        <p class="document-description">
          Полная хронология работы технического помощника в проекте SquareFox. 
          Документирует все этапы от принятия на работу до конфликтов и бана.
        </p>
      </div>
    </div>
  </div>

  <div class="category-section" id="serious-allegations">
    <h2 class="category-header">⚠️ Серьёзные Обвинения</h2>
    <div class="category-content">
      <div class="document-card">
        <h3 class="document-title"><a href="Главная/Семья с педофилами.md">Семья с педофилами</a></h3>
        <div class="document-meta">
          <span>📅 Ноябрь 2025</span>
        </div>
        <p class="document-description">
          Документирование неподходящих отношений между администраторами\модераторами проекта.
        </p>
      </div>
    </div>
  </div>

  <div class="category-section" id="admin-conflicts">
    <h2 class="category-header">👥 Конфликты с Администрацией</h2>
    <div class="category-content">
      <div class="document-card" id="moderator-conflict">
        <h3 class="document-title"><a href="Главная/Конфликт с Модером.md">Конфликт с Модером</a></h3>
        <div class="document-meta">
          <span>📅 29 ноября 2025</span>
        </div>
        <p class="document-description">
          Подробное описание конфликта с модератором Scromnik19, включая 
          оскорбления, угрозы и злоупотребление модераторскими правами.
        </p>
        </div>
      </div>
  <div> 
      <div class="document-card" id="milavi-conflict">
        <h3 class="document-title"><a href="Главная/Конфликт с Милави.md">Конфликт с Милави</a></h3>
        <div class="document-meta">
          <span>📅 29 ноября 2025</span>
        </div>
        <p class="document-description">
          Переписка и конфликт с главным администратором Милави, демонстрирующая 
          предвзятость и нежелание решать проблемы объективно.
        </p>
        </div>
      </div>
      <div class="document-card">
        <h3 class="document-title"><a href="Главная/Конфликт с Мостом.md">Конфликт с Мостом</a></h3>
        <div class="document-meta">
          <span>📅 Декабрь 2025</span>
        </div>
        <p class="document-description">
          Принуждение к признанию и давление со стороны администрации в 
          ситуации с разрушением постройки.
        </p>
        </div>
      </div>
    </div>
  </div>

  <div class="category-section" id="ban-incidents">
    <h2 class="category-header">🚫 Бан Инциденты</h2>
    <div class="category-content">
      <div class="document-card" id="mass-ban">
        <h3 class="document-title"><a href="Главная/Забаненная семёрка.md">Забаненная семёрка</a></h3>
        <div class="document-meta">
          <span>📅 11 декабря 2025, 14:31 МСК</span>
        </div>
        <p class="document-description">
          Детальное описание массового бана 7 игроков по надуманным причинам, 
          включая переписку забаненных и реакцию сообщества.
        </p>
        </div>
      </div>
      <div> 
      <div class="document-card" id="personal-ban">
        <h3 class="document-title"><a href="Главная/МОЙ БАНан.md">МОЙ БАНан</a></h3>
        <div class="document-meta">
          <span>📅 29 ноября 2025</span>
        </div>
        <p class="document-description">
          Причины личного бана технического помощника, включая предъявляемые 
          обвинения и контекст конфликта.
        </p>
        </div>
      </div>
      <div> 
      <div class="document-card">
        <h3 class="document-title"><a href="Главная/Дополнение к БАНану.md">Дополнение к БАНану</a></h3>
        <div class="document-meta">
          <span>📅 После 29 ноября 2025</span>
        </div>
        <p class="document-description">
          Дополнительная информация и факты, касающиеся ситуации с баном 
          и реакции сообщества.
        </p>
        </div>
      </div>
    </div>
  </div>

  <div class="category-section" id="financial-issues">
    <h2 class="category-header">💰 Лор за деньги?</h2>
    <div class="category-content">
      <div class="document-card">
        <h3 class="document-title"><a href="Главная/Мерзость.md">Мерзость</a></h3>
        <div class="document-meta">
          <span>📅 16 декабря 2025</span>
        </div>
        <p class="document-description">
          Случай с игроком МиМаксом, которому администрация взяла деньги за 
          услуги, которые не были выполнены, а затем забанила его.
        </p>
        </div>
      </div>
    </div>
  </div>

  <div class="category-section" id="moderation-issues">
    <h2 class="category-header">🛡️ Проблемы Модерации</h2>
    <div class="category-content">
      <div class="document-card">
        <h3 class="document-title"><a href="Главная/Отношение модератора к комьюнити.md">Отношение модератора к комьюнити</a></h3>
        <div class="document-meta">
          <span>📅 Декабрь 2025</span>
        </div>
        <p class="document-description">
          Документирование токсичного поведения модератора Ris$he4ka по отношению 
          к участникам сообщества.
        </p>\
        </div>
      </div>
    </div>
  </div>

  <div class="category-section" id="timeline">
    <h2 class="category-header">📅 Хронология Событий</h2>
    <div class="category-content">
      <div class="document-card">
        <h3 class="document-title">Временная линия конфликтов</h3>
        <div class="document-meta">
          <span>📅 Сентябрь 2025 - Декабрь 2025</span>
        </div>
        <div class="document-description">
          <strong>Сентябрь 2025:</strong> Принятие на работу технического помощника<br>
          <strong>2 ноября:</strong> Потеря доверия администрации<br>
          <strong>15 ноября:</strong> Конфликт Тикса и админ состава<br>
          <strong>15-17 ноября:</strong> Закрытие СФА<br>
          <strong>27 ноября:</strong> Конфликт со Скромником<br>
          <strong>29 ноября:</strong> Бан Тикса + личный бан Арбуза<br>
          <strong>11 декабря:</strong> Массовый бан 7 игроков<br>
          <strong>16 декабря:</strong> Случай с МиМаксом
        </div>
      </div>
    </div>
  </div>

  <div class="backlinks-section">
    <h2>🔗 Связанные документы и ссылки</h2>
    <p>Эти документы связаны между собой и содержат перекрёстные ссылки:</p>
    <ul>
      <li><strong>Конфликт с Модером</strong> → <a href="Главная/Конфликт с Милави.md">Конфликт с Милави</a> (продолжение)</li>
      <li><strong>МОЙ БАНан</strong> → <a href="Главная/Дополнение к БАНану.md">Дополнение к БАНану</a> (дополнительные факты)</li>
      <li><strong>Забаненная семёрка</strong> → упоминает <a href="Главная/Семья с педофилами.md">предыдущие конфликты</a></li>
      <li><strong>Все конфликты</strong> → связаны с <a href="Главная/Привет, я Арбуз.md">основной историей</a></li>
    </ul>
  </div>


<script>
// Theme toggle functionality
function toggleTheme() {
  const body = document.body;
  const currentTheme = body.getAttribute('data-theme') || 'dark';
  const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
  
  body.setAttribute('data-theme', newTheme);
  localStorage.setItem('theme', newTheme);
  
  const toggle = document.querySelector('.theme-toggle');
  toggle.textContent = newTheme === 'dark' ? '🌙' : '☀️';
}

// Load saved theme
document.addEventListener('DOMContentLoaded', function() {
  const savedTheme = localStorage.getItem('theme') || 'dark';
  document.body.setAttribute('data-theme', savedTheme);
  document.querySelector('.theme-toggle').textContent = savedTheme === 'dark' ? '🌙' : '☀️';
});

// Search functionality
document.getElementById('searchInput').addEventListener('input', function(e) {
  const searchTerm = e.target.value.toLowerCase();
  const documentCards = document.querySelectorAll('.document-card');
  
  documentCards.forEach(card => {
    const title = card.querySelector('.document-title').textContent.toLowerCase();
    const description = card.querySelector('.document-description').textContent.toLowerCase();
    const tags = Array.from(card.querySelectorAll('.tag')).map(tag => tag.textContent.toLowerCase());
    
    const matches = title.includes(searchTerm) || 
                   description.includes(searchTerm) || 
                   tags.some(tag => tag.includes(searchTerm));
    
    if (matches || searchTerm === '') {
      card.style.display = 'block';
    } else {
      card.style.display = 'none';
    }
  });
});

// Filter functionality
function filterContent(category) {
  const documentCards = document.querySelectorAll('.document-card');
  const filterTabs = document.querySelectorAll('.filter-tab');
  
  // Update active tab
  filterTabs.forEach(tab => tab.classList.remove('active'));
  event.target.classList.add('active');
  
  documentCards.forEach(card => {
    if (category === 'all') {
      card.style.display = 'block';
    } else {
      const tags = Array.from(card.querySelectorAll('.tag')).map(tag => tag.textContent.toLowerCase());
      const title = card.querySelector('.document-title').textContent.toLowerCase();
      
      let shouldShow = false;
      
      switch(category) {
        case 'conflicts':
          shouldShow = tags.some(tag => ['конфликт', 'скромник', 'милави', 'администратор'].includes(tag)) ||
                      title.includes('конфликт');
          break;
        case 'bans':
          shouldShow = tags.some(tag => ['бан', 'массовый бан', 'забаненный'].includes(tag)) ||
                      title.includes('бан');
          break;
        case 'admin':
          shouldShow = tags.some(tag => ['администрация', 'администратор', 'модерация'].includes(tag)) ||
                      title.includes('администрация') || title.includes('модератор');
          break;
        case 'serious':
          shouldShow = tags.some(tag => ['обвинения', 'серьёзные'].includes(tag)) ||
                      title.includes('педофил');
          break;
      }
      
      card.style.display = shouldShow ? 'block' : 'none';
    }
  });
}

// Smooth scrolling for anchor links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function (e) {
    e.preventDefault();
    const target = document.querySelector(this.getAttribute('href'));
    if (target) {
      target.scrollIntoView({
        behavior: 'smooth',
        block: 'start'
      });
    }
  });
});

// Highlight search results
function highlightSearchResults() {
  const searchInput = document.getElementById('searchInput');
  const searchTerm = searchInput.value;
  
  if (searchTerm.length > 2) {
    const documentCards = document.querySelectorAll('.document-card');
    
    documentCards.forEach(card => {
      const titleElement = card.querySelector('.document-title');
      const descElement = card.querySelector('.document-description');
      
      // Remove previous highlights
      titleElement.innerHTML = titleElement.textContent;
      descElement.innerHTML = descElement.textContent;
      
      // Add new highlights
      const titleText = titleElement.textContent;
      const descText = descElement.textContent;
      
      if (titleText.toLowerCase().includes(searchTerm.toLowerCase())) {
        const regex = new RegExp(`(${searchTerm})`, 'gi');
        titleElement.innerHTML = titleText.replace(regex, '<span class="highlight">$1</span>');
      }
      
      if (descText.toLowerCase().includes(searchTerm.toLowerCase())) {
        const regex = new RegExp(`(${searchTerm})`, 'gi');
        descElement.innerHTML = descText.replace(regex, '<span class="highlight">$1</span>');
      }
    });
  }
}

// Update search functionality to include highlighting
document.getElementById('searchInput').addEventListener('input', function(e) {
  const searchTerm = e.target.value.toLowerCase();
  const documentCards = document.querySelectorAll('.document-card');
  
  documentCards.forEach(card => {
    const title = card.querySelector('.document-title').textContent.toLowerCase();
    const description = card.querySelector('.document-description').textContent.toLowerCase();
    const tags = Array.from(card.querySelectorAll('.tag')).map(tag => tag.textContent.toLowerCase());
    
    const matches = title.includes(searchTerm) || 
                   description.includes(searchTerm) || 
                   tags.some(tag => tag.includes(searchTerm));
    
    if (matches || searchTerm === '') {
      card.style.display = 'block';
    } else {
      card.style.display = 'none';
    }
  });
  
  highlightSearchResults();
});
</script>

---

## Теги и категории


### Временные метки
- `сентябрь 2025` - Начало работы
- `октябрь 2025` - Первые конфликты
- `ноябрь 2025` - Эскалация конфликтов
- `декабрь 2025` - Критические события

### Участники
- `Арбуз` - Технический помощник
- `Милави` - Главный администратор
- `Нерз` - Лорный администратор
- `Скромник` - Модератор
- `Ris$he4ka` - Модератор
- `tix45` - Жертва админстрации

---
