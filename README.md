# Exercício 6 - Voltar a Commits Anteriores

1. Liste todos os commits feitos na master.
2. Altere o arquivo `contact.html`, para o seguinte código:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contato</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Entre em Contato Comigo!</h1>
    </header>
    <div class="container">
        <form id="contactForm">
            <label for="name">Nome:</label>
            <input type="text" id="name" name="name" required>

            <label for="tel">Telefone:</label>
            <input type="tel" id="tel" name="tel" required>

            <label for="email">E-mail:</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Mensagem:</label>
            <textarea id="message" name="message" rows="4" required></textarea>

            <button type="submit">Enviar</button>
        </form>
    </div>
</body>
</html>

```
3. Adicione o arquivo `contact.html` a staging area, mas não commita. Use git status para acompanhar os arquivos.
4. Restaure o arquivo `contact.html` da staging area para o workspace
5. Restaure o arquivo `contact.html` para que ele volte ao seu último commit.
6. Altere o arquivo `style.css`, para o seguinte código:

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #6a4dff;
}
header {
    background-color: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
}
h1 {
    margin: 0;
}
.container {
    max-width: 800px;
    margin: auto;
    padding: 20px;
}
p {
    line-height: 1.6;
}
form {
    margin-top: 20px;
}
label {
    display: block;
    margin-bottom: 10px;
}
input, textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-sizing: border-box;
}
button {
    background-color: #333;
    color: #fff;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

```
7. Adicione e comite as alterações, com a mensagem de commit "atualizar cor de background".
8. Resete com --hard o arquivo `style.css` para HEAD~1.
9. Altere o arquivo `contact.html`, para o seguinte código:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contato</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Entre em Contato Comigo!</h1>
    </header>
    <div class="container">
        <form id="contactForm">
            <label for="name">Nome:</label>
            <input type="text" id="name" name="name" required>

            <label for="tel">Telefone:</label>
            <input type="tel" id="tel" name="tel" required>

            <label for="email">E-mail:</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Mensagem:</label>
            <textarea id="message" name="message" rows="4" required></textarea>

            <button type="submit">Enviar</button>
        </form>
    </div>
</body>
</html>

```
10. Adicione e comite as alterações, com a mensagem de commit "atualizar página de contato para receber telefone".
11. Reverta o commit anterior.
12. teste reverter
