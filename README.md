
# Página Pessoal - Rodrigo Bergenthal

![Profile Avatar](https://avatars.githubusercontent.com/u/116042656?v=4)

## Sobre

Este projeto é uma página pessoal criada para apresentar informações sobre Rodrigo Bergenthal, um engenheiro front-end. A página inclui uma biografia, links para redes sociais e uma lista de projetos.

## Tecnologias Utilizadas

- HTML5
- CSS3 (LESS)
- JavaScript
- Google Fonts

## Estrutura do Projeto

```plaintext
├── .build
│   └── styles
│       └── main.css
├── src
│   └── images
│       ├── github.svg
│       ├── instagram.svg
│       ├── linkedin.svg
│       └── mail.svg
├── index.html
├── main.less
└── README.md
```

## Funcionalidades

- **Biografia**: Informações sobre Rodrigo Bergenthal.
- **Links Sociais**: Ícones clicáveis que direcionam para perfis de redes sociais.
- **Projetos**: Lista de projetos com links para visualização.

## Como Usar

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/RodrigoBergenthal/pagina-pessoal.git
   ```

2. **Navegue até o diretório do projeto:**

   ```bash
   cd pagina-pessoal
   ```

3. **Abra o arquivo `index.html` em um navegador para visualizar a página:**

   ```bash
   open index.html
   ```

## Código Exemplo

### HTML

```html
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pagina Pessoal - Rodrigo Bergenthal</title>
    <link rel="stylesheet" href=".build/styles/main.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
</head>

<body>
    <div class="container">
        <header>
            <img class="profile-avatar" src="https://via.placeholder.com/96x96" />
            <div class="profile-bio">
                <h1 class="profile-bio-name">Página do Rodrigo Bergenthal</h1>
                <h2 class="profile-bio-subtitle"> Engenheiro Front-end</h2>
                <p class="profile-bio-description">Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                    Accusantium sed veniam qui sint laborum eos hic.
                    Officia odio earum asperiores perferendis ullam,
                    ipsum ipsa eligendi quaerat nobis animi at dolorem?</p>
            </div>
        </header>
        <nav>
            <ul class="social-links">
                <li>
                    <a href="https://www.instagram.com/RodrigoBergenthal" target="_blank" rel="noopener noreferrer">
                        <img src="./src/images/instagram.svg" alt="logo-instagram">
                    </a>
                </li>
                <li>
                    <a href="https://www.linkedin.com/in/RodrigoBergenthal" target="_blank" rel="noopener noreferrer">
                        <img src="./src/images/linkedin.svg" alt="logo-linkedin">
                    </a>
                </li>
                <li>
                    <a href="https://github.com/RodrigoBergenthal" target="_blank" rel="noopener noreferrer">
                        <img src="./src/images/github.svg" alt="logo-github">
                    </a>
                </li>
                <li>
                    <a href="mailto:rodrigo@exemplo.com?subject=Contato" target="_blank" rel="noopener noreferrer">
                        <img src="./src/images/mail.svg" alt="logo-de-email">
                    </a>
                </li>
            </ul>
        </nav>
        <nav>
            <ul class="projects-list">
                <li class="projects-list-item">
                    <a href="https://github.com/RodrigoBergenthal/calculadora-medias" target="_blank" rel="noopener noreferrer">
                        Visite o projeto "Calculadora de médias"
                    </a>
                </li>
                <li class="projects-list-item">
                    <a href="https://github.com/RodrigoBergenthal/game-shop" target="_blank" rel="noopener noreferrer">
                        Visite o projeto "Game Shop"
                    </a>
                </li>
                <li class="projects-list-item">
                    <a href="https://github.com/RodrigoBergenthal/galeria-fotos" target="_blank" rel="noopener noreferrer">
                        Visite o projeto "Galeria de Fotos"
                    </a>
                </li>
            </ul>
        </nav>
    </div>
</body>

</html>
```

### LESS

```less
@import "mapas.less";
@breakpointMobile: ~"(max-width: 767px)";
@breakpointtablet: ~"(min-width: 768px) and (max-width: 1023px)";

.marginbotton8 {
  margin-bottom: 8px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
}

body {
  background-color: #colors [backgroundColor];
  color: #colors [textColor];
}

.container {
  max-width: 960px;
  width: 100%;
  margin: 0 auto;

  @media @breakpointMobile {
    max-width: 70%;
    background-color: red;
  }

  @media @breakpointTablet {
    max-width: 80%;
    background-color: yellow;
  }
}

li {
  list-style: none;
}

header {
  padding: 24px;

  .profile-avatar {
    display: block;
    margin: 0 auto 24px;
    border-radius: 100px;
  }
}

.profile-bio {
  text-align: center;

  &-name {
    font-size: 10px;
    .marginbotton8();
  }

  &-subtitle {
    font-size: 14px;
    .marginbotton8();
  }

  &-description {
    font-size: 14px;
    opacity: 70%;
  }
}

.social-links {
  display: flex;
  justify-content: space-between;
  max-width: 240px;
  width: 100%;
  margin: 0 auto;

  img {
    transition: all ease 0.3s;
    &:hover {
      transform: scale(1.5);
    }
  }
}

.projects-list {
  &-item {
    a {
      text-decoration: none;
      background-color: #colors [buttonColor];
      display: block;
      padding: 16px 20px;
    }
  }
}
```
```

Como Usar
Clone o repositório:
git clone https://github.com/RodrigoBergenthal/pagina-pessoal.git
