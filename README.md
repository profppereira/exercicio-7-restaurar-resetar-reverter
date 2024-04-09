# Exercício 5 - Merge

1. Crie uma nova pasta chamada `exercicio-5-merge`.
2. Crie um novo repositório git dentro da pasta (certifique-se de que não está em um repositório existente).
3. Crie um novo arquivo chamado `index.html` (deixe-o vazio por enquanto).
4. Crie um novo arquivo chamado `script.js` (deixe-o vazio por enquanto).
5. Crie um novo arquivo chamado `style.css` (deixe-o vazio por enquanto).
6. Adicione e comite os arquivos vazios, com a mensagem "adicionar arquivos web vazios".
7. Imediatamente crie uma nova branch chamada `home-page` e outra branch chamada `about-me` (ambas baseadas na branch principal).
8. Mude para a branch `home-page` usando o comando "switch" para trocar de branch.
9. No arquivo `index.html`, adicione o seguinte:

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Minha Página Inicial</title>
      <script src="script.js"></script>
      <link rel="stylesheet" href="style.css">
  </head>
  <body>
      <header>
          <h1>Minha Página Inicial</h1>
      </header>
      <div class="container">
          <h2>Bem-vindo à minha página inicial</h2>
          <p>Esta é minha home page.</p>
          <p>Exercícios de Git.</p>
          <button onclick="atualizarHora()">Mostrar Hora Atual</button>
          <p id="horaAtual"></p>
      </div>
  </body>
</html>

```

10. No arquivo `script.js`, adicione o seguinte:

```javascript
function atualizarHora() {
    var data = new Date();
    var hora = data.getHours();
    var minutos = data.getMinutes();
    var segundos = data.getSeconds();

    hora = hora < 10 ? '0' + hora : hora;
    minutos = minutos < 10 ? '0' + minutos : minutos;
    segundos = segundos < 10 ? '0' + segundos : segundos;

    document.getElementById('horaAtual').innerText = hora + ':' + minutos + ':' + segundos;
}

```

11. No arquivo `style.css`, adicione o seguinte:

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f2f2f2;
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

```

12. Adicione e comite as alterações, com a mensagem de commit "adicionar home page do meu website".
13. Mude para a branch `about-me` usando o comando "checkout" para trocar de branch.
14. Crie um novo arquivo chamado `about.html`, e adicione exatamente o seguinte (não altere o texto da página):

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Sobre Mim</title>
      <link rel="stylesheet" href="style.css">
  </head>
  <body>
      <header>
          <h1>Sobre Mim</h1>
      </header>
      <div class="container">
          <h2>Um pouco sobre mim</h2>
          <p>Meu nome é [Seu Nome]. Eu sou um [sua ocupação] interessado em [seus interesses].</p>
          <p>Eu gosto de [suas atividades favoritas] e estou interessado em aprender mais sobre [áreas de interesse].</p>
          <p>Sinta-se à vontade para entrar em contato comigo através do meu e-mail: [seu e-mail].</p>
      </div>
  </body>
</html>

```

15. Adicione e comite as alterações na branch `about-me` com a mensagem de commit "adicionar página sobre mim".
16. Em seguida, crie uma nova branch com base na branch `about-me` chamada `about-me-feature`.
17. Mude para a branch `about-me-feature`.
18. Edite o arquivo `about.html` para que tenha o botão de Mostrar Hora Atual, igual tem no arquivo `index.html`, o código do arquivo `about.html` deve ficar exatamente o seguinte:

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Sobre Mim</title>
      <script src="script.js"></script>
      <link rel="stylesheet" href="style.css">
  </head>
  <body>
      <header>
          <h1>Sobre Mim</h1>
      </header>
      <div class="container">
          <h2>Um pouco sobre mim</h2>
          <p>Meu nome é [Seu Nome]. Eu sou um [sua ocupação] interessado em [seus interesses].</p>
          <p>Eu gosto de [suas atividades favoritas] e estou interessado em aprender mais sobre [áreas de interesse].</p>
          <p>Sinta-se à vontade para entrar em contato comigo através do meu e-mail: [seu e-mail].</p>
          <button onclick="atualizarHora()">Mostrar Hora Atual</button>
          <p id="horaAtual"></p>
      </div>
  </body>
</html>

```

19. Adicione e comite a alteração com a mensagem "adicionar Mostrar Hora Atual na página sobre mim".
20. Mude para a branch `about-me`.
21. Altere o texto da página substituindo tudo que estiver entre colchetes `[]`, por suas informações. Por exemplo, onde estiver `[Seu Nome]`, alterar pelo seu nome de fato, e assim sucessivamente.
22. Adicione e comite a alteração com a mensagem "adicionar informações na página sobre mim".
23. Ainda na branch `about-me`, no arquivo `style.css`, adicione o seguinte:

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #d90000;
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

```
24. Adicione e comite a alteração com a mensagem "atualiza cor de background nas páginas".
25. Mude para a branch `master`.
26. Mescle (faça um merge) a branch `home-page` na branch `master`, que tipo de merge aconteceu?
27. Agora mescle (faça um merge) a branch `about-me` na branch `master`, que tipo de merge aconteceu? Esse merge vai gerar conflito, mantenha as mudanças da branch `about-me`.
28. Agora mescle (faça um merge) a branch `about-me-feature` na branch `master`, que tipo de merge aconteceu? Esse merge vai gerar conflito, mantenha as mudanças da branch `master`.
