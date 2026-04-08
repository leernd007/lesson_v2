 **Розміщення сайту в інтернеті**
    - Використайте сервіс [GitHub Pages](https://pages.github.com/)
    - Отримайте посилання на свій сайт.

## Хід роботи
1. Зареєструватись на github.com
2. Створити нову публічну репозиторію (імя має бути <user>.github.io)
   <img width="870" height="743" alt="image" src="https://github.com/user-attachments/assets/92dcbe2f-140b-46e0-b6f8-fd1dfffb2a0c" />
3. Створити там наступні файли
<img width="1167" height="195" alt="image" src="https://github.com/user-attachments/assets/2821fad7-dcdf-418e-a31e-9cf6dc93d63c" />

      index.html
      style.css
   і папку images/ 
   <img width="337" height="42" alt="image" src="https://github.com/user-attachments/assets/bf73771a-e13c-407c-a9f4-c539196badc0" />


4. `index.html`.
```html
<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <title>Мій вебсайт</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <img src="images/logo.png" alt="Логотип" class="logo">
        <h1>Вітаю на моєму сайті!</h1>
    </header>

    <main>
        <p>Це мій перший вебсайт з HTML і CSS.</p>
        <p>Тут можна додавати текст, зображення та інші елементи.</p>
    </main>

    <footer>
        <p>Автор: Учень Тернопільської ЗОШ I-III ступенів № 3 | 2026</p>
    </footer>
</body>
</html>
```
5. `styles.css`.
```css
/* Загальні стилі */
body {
    font-family: Arial, sans-serif;
    background-color: #f0f8ff;
    margin: 0;
    padding: 0;
    text-align: center;
}

/* Header */
header {
    background-color: #4682b4;
    color: white;
    padding: 20px 0;
}

/* Логотип */
.logo {
    width: 100px;
    height: auto;
}

/* Основний контент */
main {
    padding: 20px;
    font-size: 18px;
}

/* Footer */
footer {
    background-color: #4682b4;
    color: white;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}
```
6. В папку `images` добав туди logo.png (будь яке лого на ваш вибір з інтернету)
7. Як створити свою веб сторінку на основі вашої репозиторії описано ось тут https://docs.github.com/en/pages/quickstart
