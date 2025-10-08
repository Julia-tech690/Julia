<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Портфолио педагога</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            color: #333;
            font-size: 16px;
        }
        header {
            background-color: #2c3e50;
            color: white;
            padding: 1.5em 1em;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #34495e;
            position: sticky;
            top: 0;
            z-index: 100;
            flex-wrap: wrap;
        }
        nav a {
            color: white;
            padding: 0.8em 1em;
            text-decoration: none;
            transition: background-color 0.3s;
            font-size: 0.9em;
        }
        nav a:hover {
            background-color: #16a085;
        }
        section {
            padding: 2em 1em;
            max-width: 1000px;
            margin: 0 auto;
        }
        .section-title {
            color: #2c3e50;
            border-bottom: 2px solid #16a085;
            padding-bottom: 0.5em;
            margin-bottom: 1.5em;
            font-size: 1.5em;
        }
        .project-gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 1em;
        }
        .project-card {
            width: 100%;
            margin-bottom: 1.5em;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            border-radius: 5px;
            overflow: hidden;
            transition: transform 0.3s;
        }
        .project-card:hover {
            transform: translateY(-5px);
        }
        .project-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }
        .project-card h3 {
            padding: 0.5em 1em;
            margin: 0;
            background-color: #f8f9fa;
            font-size: 1.1em;
        }
        .project-card p {
            padding: 0 1em 1em;
            margin: 0;
            font-size: 0.9em;
        }
        form input, form textarea {
            width: 100%;
            padding: 0.8em;
            margin-top: 1em;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 1em;
        }
        form button {
            background-color: #16a085;
            color: white;
            border: none;
            padding: 0.8em 2em;
            margin-top: 1em;
            cursor: pointer;
            border-radius: 4px;
            transition: background-color 0.3s;
            font-size: 1em;
            width: 100%;
        }
        form button:hover {
            background-color: #1abc9c;
        }
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 1.5em 1em;
            margin-top: 2em;
            font-size: 0.9em;
        }
        .qualifications {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5em;
        }
        .qualification-item {
            background-color: #f8f9fa;
            padding: 1.2em;
            border-radius: 5px;
        }
        .qualification-item h3 {
            font-size: 1.2em;
            margin-top: 0;
        }
        .qualification-item ul {
            padding-left: 1.2em;
        }
        .qualification-item li {
            margin-bottom: 0.5em;
            font-size: 0.9em;
        }
        
        /* Стили для блока "О педагоге" */
        .about-container {
            display: flex;
            flex-direction: column;
            gap: 1.5em;
        }
        .about-container img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            margin: 0 auto;
            display: block;
        }
        .about-info h3 {
            margin-top: 0;
            font-size: 1.3em;
        }
        .about-info p {
            margin-bottom: 0.8em;
            font-size: 0.95em;
        }
        
        /* Стили для контактов */
        .contact-container {
            display: flex;
            flex-direction: column;
            gap: 2em;
        }
        .contact-info h3, .contact-form h3 {
            font-size: 1.2em;
            margin-top: 0;
        }
        .contact-info p {
            margin-bottom: 0.8em;
            font-size: 0.95em;
        }
        
        @media (min-width: 480px) {
            nav a {
                padding: 0.8em 1.2em;
                font-size: 1em;
            }
            .about-container {
                flex-direction: row;
                align-items: center;
            }
            .about-container img {
                margin: 0;
            }
        }
        
        @media (min-width: 600px) {
            .project-card {
                width: 48%;
            }
            .qualifications {
                grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            }
            .contact-container {
                flex-direction: row;
            }
        }
        
        @media (min-width: 768px) {
            body {
                font-size: 17px;
            }
            .project-card {
                width: 30%;
            }
            nav a {
                padding: 1em 2em;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Портфолио педагога</h1>
    <p>Современные образовательные технологии и методики преподавания</p>
</header>

<nav>
    <a href="#about">О педагоге</a>
    <a href="#qualifications">Квалификация</a>
    <a href="#projects">Методические разработки</a>
    <a href="#achievements">Достижения</a>
    <a href="#contact">Контакты</a>
</nav>

<section id="about">
    <h2 class="section-title">О педагоге</h2>
    <div class="about-container">
        <img src="https://github.com/Julia-tech690/-/blob/main/640360как%20бы%20я11.png?raw=true" alt="Фото педагога">
        <div class="about-info">
            <h3>Иванова Мария Петровна</h3>
            <p>Учитель истории и обществознания высшей квалификационной категории</p>
            <p>Стаж работы: 15 лет</p>
            <p>Специализация: учитель истории, искусственный интеллект в обучении</p>
        </div>
    </div>
</section>

<section id="qualifications">
    <h2 class="section-title">Квалификация</h2>
    <div class="qualifications">
        <div class="qualification-item">
            <h3>Образование</h3>
            <p>Кузбасская государственная педагогическая академия, 2008</p>
            <p>Специальность: "История"</p>
        </div>
        <div class="qualification-item">
            <h3>Повышение квалификации</h3>
            <ul>
                <li>Цифровые технологии в образовании (2023)</li>
                <li>Искусственный интеллект в школе (2024)</li>
                <li>Разработка интерактивных учебных материалов (2022)</li>
            </ul>
        </div>
        <div class="qualification-item">
            <h3>Профессиональные навыки</h3>
            <ul>
                <li>Разработка электронных образовательных ресурсов</li>
                <li>Создание интерактивных уроков</li>
                <li>Использование LMS систем (Moodle, Google Classroom)</li>
                <li>Программирование на Python, JavaScript</li>
            </ul>
        </div>
    </div>
</section>

<section id="projects">
    <h2 class="section-title">Методические разработки</h2>
    <div class="project-gallery">
        <div class="project-card">
            <img src="https://via.placeholder.com/300x200" alt="Методическая разработка">
            <h3>ИИ в школьной программе</h3>
            <p>Методическое пособие по программированию на Python</p>
        </div>
        <div class="project-card">
            <img src="https://via.placeholder.com/300x200" alt="Методическая разработка">
            <h3>Интерактивный курс Python</h3>
            <p>Серия интерактивных уроков по программированию для начинающих</p>
        </div>
        <div class="project-card">
            <img src="https://via.placeholder.com/300x200" alt="Методическая разработка">
            <h3>Цифровая грамотность</h3>
            <p>Рабочая тетрадь по развитию цифровых навыков у учащихся 5-7 классов</p>
        </div>
    </div>
</section>

<section id="achievements">
    <h2 class="section-title">Достижения</h2>
    <div class="qualifications">
        <div class="qualification-item">
            <h3>Награды</h3>
            <ul>
                <li>Победитель конкурса "Цифровая компетентность современного педагога" (2025)</li>
            </ul>
        </div>
        <div class="qualification-item">
            <h3>Публикации</h3>
            <ul>
                <li>Статья "ИИ в образовании: перспективы и риски" (2024)</li>
                <li>Методическое пособие "Gamification в обучении" (2023)</li>
            </ul>
        </div>
        <div class="qualification-item">
            <h3>Ученические достижения</h3>
            <ul>
                <li>5 победителей олимпиад по истории и обществознанию</li>
                <li>3 призера конкурса проектных работ</li>
            </ul>
        </div>
    </div>
</section>

<section id="contact">
    <h2 class="section-title">Контакты</h2>
    <div class="contact-container">
        <div class="contact-info">
            <h3>Контактная информация</h3>
            <p>Email: teacher@example.com</p>
            <p>Телефон: +7 (123) 456-78-90</p>
            <p>Школа: МБОУ "Красулинская ООШ", Новокузнецкий МО</p>
        </div>
        <div class="contact-form">
            <form onsubmit="event.preventDefault(); alert('Сообщение отправлено! Спасибо за обратную связь.'); this.reset();">
                <input type="text" name="name" placeholder="Ваше имя" required>
                <input type="email" name="email" placeholder="Ваш email" required>
                <textarea name="message" rows="5" placeholder="Ваше сообщение" required></textarea>
                <button type="submit">Отправить сообщение</button>
            </form>
        </div>
    </div>
</section>

<footer>
    <p>&copy; 2025 Портфолио педагога Ивановой М.П.</p>
    <p>Все методические материалы защищены авторским правом</p>
</footer>

</body>
</html>
