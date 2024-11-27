<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Простая форма</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        form {
            max-width: 400px;
            margin: 0 auto;
        }
        label {
            display: block;
            margin: 10px 0 5px;
        }
        input, textarea, select {
            width: 100%;
            padding: 8px;
            margin-bottom: 15px;
            box-sizing: border-box;
        }
        button {
            padding: 10px 20px;
            margin-right: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Простая форма</h1>
    <form action="#" method="post">
        <fieldset>
            <legend>Данные пользователя</legend>          
            <label for="name">Имя:</label>
            <input type="text" id="name" name="name" required placeholder="Введите ваше имя">
            <label for="email">Электронная почта:</label>
            <input type="email" id="email" name="email" required placeholder="Введите вашу почту">
            <label for="password">Пароль:</label>
            <input type="password" id="password" name="password" required placeholder="Введите пароль">
            <label for="comments">Комментарии:</label>
            <textarea id="comments" name="comments" rows="4" placeholder="Напишите ваш комментарий"></textarea>
        </fieldset>
        <fieldset>
            <legend>Дополнительная информация</legend>    
            <label for="country">Выберите страну:</label>
            <select id="country" name="country" required>
                <option value="">Выберите страну</option>
                <option value="russia">Россия</option>
                <option value="usa">США</option>
                <option value="canada">Канада</option>
            </select>
        </fieldset>
        <button type="submit">Отправить</button>
        <button type="reset">Сбросить</button>
    </form>
</body>
</html>

