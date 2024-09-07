<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anime Slayer Clone</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <!-- رأس الموقع -->
    <header>
        <h1>Anime Slayer Clone</h1>
        <nav>
            <ul>
                <li><a href="#latest">آخر الحلقات</a></li>
                <li><a href="#genres">التصنيفات</a></li>
                <li><a href="#popular">الأكثر شهرة</a></li>
                <li><a href="#search">بحث</a></li>
            </ul>
        </nav>
    </header>

    <!-- قسم البحث -->
    <section id="search">
        <h2>ابحث عن أنمي</h2>
        <input type="text" id="searchBar" placeholder="أدخل اسم الأنمي...">
        <button onclick="searchAnime()">بحث</button>
    </section>

    <!-- قسم آخر الحلقات -->
    <section id="latest">
        <h2>آخر الحلقات</h2>
        <div class="anime-list">
            <div class="anime-item">
                <img src="anime1.jpg" alt="Anime 1">
                <h3>اسم الأنمي 1</h3>
                <a href="episode1.html">مشاهدة الآن</a>
            </div>
            <div class="anime-item">
                <img src="anime2.jpg" alt="Anime 2">
                <h3>اسم الأنمي 2</h3>
                <a href="episode2.html">مشاهدة الآن</a>
            </div>
            <!-- تكرار المزيد من الأنميات -->
        </div>
    </section>

    <!-- قسم التصنيفات -->
    <section id="genres">
        <h2>التصنيفات</h2>
        <ul>
            <li><a href="#">أكشن</a></li>
            <li><a href="#">رومانسي</a></li>
            <li><a href="#">كوميدي</a></li>
            <li><a href="#">خيال علمي</a></li>
        </ul>
    </section>

    <!-- قسم الأكثر شهرة -->
    <section id="popular">
        <h2>الأكثر شهرة</h2>
        <div class="anime-list">
            <div class="anime-item">
                <img src="anime3.jpg" alt="Anime 3">
                <h3>اسم الأنمي 3</h3>
                <a href="episode3.html">مشاهدة الآن</a>
            </div>
            <div class="anime-item">
                <img src="anime4.jpg" alt="Anime 4">
                <h3>اسم الأنمي 4</h3>
                <a href="episode4.html">مشاهدة الآن</a>
            </div>
        </div>
    </section>

    <!-- التذييل -->
    <footer>
        <p>&copy; 2024 Anime Slayer Clone</p>
    </footer>

    <script src="scripts.js"></script>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    background-color: #f5f5f5;
    margin: 0;
    padding: 0;
    direction: rtl;
}

header {
    background-color: #2c3e50;
    color: white;
    padding: 20px;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin-right: 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

section {
    margin: 20px;
}

.anime-list {
    display: flex;
    flex-wrap: wrap;
}

.anime-item {
    width: 200px;
    margin: 10px;
}

.anime-item img {
    width: 100%;
    height: auto;
}

.anime-item h3 {
    font-size: 18px;
    margin: 10px 0;
}

footer {
    background-color: #2c3e50;
    color: white;
    text-align: center;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}

// دالة بسيطة للبحث عن أنمي
function searchAnime() {
    const searchQuery = document.getElementById('searchBar').value.toLowerCase();
    alert('بحث عن: ' + searchQuery);
}
