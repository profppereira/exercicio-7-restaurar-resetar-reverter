# Exercício 6 - Voltar a Commits Anteriores

1. Liste todos os commits feitos na master.
2. Volte ao commit antes de mesclar a branch `about-me-feature`.
3. Imediatamente crie uma nova branch chamado `contact`.
4. Crie um arquivo `contact.html`, adicione o seguinte:

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
        <h1>Entre em Contato</h1>
    </header>
    <div class="container">
        <form id="contactForm">
            <label for="name">Nome:</label>
            <input type="text" id="name" name="name" required>

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

5. Adicione o seguinte código ao final do arquivo `style.css` (abaixo do seletor `p`):

```css
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

6. Adicione e comite as alterações, com a mensagem de commit "adicionar página de contato".
7. Mude para a branch `master`.
8. Mescle (faça um merge) a branch `contact` na branch `master`, que tipo de merge aconteceu?
9. Se houver conflitos, ajuste-os e complete o processo de merge.
10. Liste todos os commits feitos na master.
