# Анкета користувача

Користувач вводить:

- ім’я  
- вік  
- улюблений предмет  

Сайт виводить повідомлення:  

> Привіт, [ім’я]! Тобі [вік] років, і ти любиш [предмет].

---

## 💻 HTML + JavaScript код

```html
<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <title>Анкета учня</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            padding: 20px;
        }
        form {
            background-color: #fff;
            padding: 15px;
            border-radius: 8px;
            max-width: 300px;
        }
        input, button {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
        }
        button {
            cursor: pointer;
        }
        h3 {
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <h2>Анкета учня</h2>

    <form id="myForm">
        <label>Ім’я:</label><br>
        <input type="text" id="name"><br><br>

        <label>Вік:</label><br>
        <input type="number" id="age"><br><br>

        <label>Улюблений предмет:</label><br>
        <input type="text" id="subject"><br><br>

        <button type="submit">Відправити</button>
    </form>

    <h3 id="result"></h3>

    <script>
        document.getElementById("myForm").addEventListener("submit", function(event) {
            event.preventDefault();

            let name = document.getElementById("name").value.trim();
            let age = document.getElementById("age").value.trim();
            let subject = document.getElementById("subject").value.trim();

            if (name === "" || age === "" || subject === "") {
                alert("Заповніть всі поля!");
                return;
            }

            let message = "Привіт, " + name + "! Тобі " + age +
                          " років, і ти любиш " + subject + ".";

            if (age < 18) {
                message += " Ти ще школяр!";
            } else {
                message += " Ти вже дорослий!";
            }

            document.getElementById("result").innerText = message;
        });
    </script>

</body>
</html>
