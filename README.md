```html
<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <title>Форма з валідацією</title>
    <style>
        body {
            font-family: Arial;
            max-width: 500px;
            margin: 40px auto;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            margin: 8px 0;
        }
        button {
            padding: 10px;
        }
    </style>
</head>
<body>

<h2>Реєстраційна форма</h2>

<form>

    <!-- Текст -->
    <label>Ім'я:</label>
    <input type="text" name="name" required minlength="2" maxlength="20">

    <!-- Email -->
    <label>Email:</label>
    <input type="email" name="email" required>

    <!-- Пароль -->
    <label>Пароль:</label>
    <input type="password" name="password" required minlength="6">

    <!-- Число -->
    <label>Вік:</label>
    <input type="number" name="age" min="1" max="100" required>

    <!-- Телефон (з pattern) -->
    <label>Телефон (+380XXXXXXXXX):</label>
    <input type="tel" name="phone" pattern="\+380[0-9]{9}" required>

    <!-- Дата -->
    <label>Дата народження:</label>
    <input type="date" name="birthdate" required>

    <!-- Вибір зі списку -->
    <label>Стать:</label>
    <select name="gender" required>
        <option value="">Оберіть</option>
        <option value="male">Чоловік</option>
        <option value="female">Жінка</option>
    </select>

    <!-- Радіо -->
    <label>Рівень знань:</label><br>
    <input type="radio" name="level" value="beginner" required> Початковий<br>
    <input type="radio" name="level" value="middle"> Середній<br>
    <input type="radio" name="level" value="advanced"> Просунутий<br>

    <!-- Чекбокс -->
    <label>
        <input type="checkbox" required>
        Я погоджуюсь з правилами
    </label>

    <!-- Текстове поле -->
    <label>Коментар:</label>
    <textarea name="comment" minlength="5" maxlength="200"></textarea>

    <!-- Кнопка -->
    <button type="submit">Відправити</button>

</form>

</body>
</html>
```
