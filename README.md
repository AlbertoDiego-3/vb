<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta
      name="viewport"
      content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0"
    />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="../static/css/style.css" />
    <title>Portafolio</title>
  </head>
  <body>
    <header class="header">
      <nav class="header__nav main-nav">
        <ul class="main-nav__list main-list">
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#home">HOME</a>
          </li>
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#about">ABOUT</a>
          </li>
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#skills">MY SKILLS</a>
          </li>
        </ul>
      </nav>
    </header>
    <main class="main">
      <!-- Vista previa -->
      <section class="main__home home" id="home">
        <h1 class="home__title">Alberto</h1>
        <p class="home__subtitle">WEB-DEVELOPER,PROGRAMMER</p>
      </section>
      <!-- Acerca de mí -->
      <section class="main__about about" id="about">
        <h2 class="about__title">ABOUT ME</h2>
        <div class="about__info info-block">
          <p class="info-block__text">
            Tengo  17 años, soy de Mexico,
             me gusta programar y los videojuegos
          </p>
          <img
            class="info-block__img"
            src="../static/img/profile.png"
            alt="me"
            width="250"
            height="250"
          />
        </div>
      </section>
      <!-- Sección de competencias -->
      <section class="main__skills skills" id="skills">
        <h2 class="skills__title">Mis habilidades</h2>
        <form action="/" method="POST">
          <ul class="skills__list skills-list">
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/python.png"
                alt="python"
                width="150"
                height="150"
              />
              <span class="skill__info">info habilidad en</span>
              <input class="skill__button" type="submit" name="button_python" value="SHOW PROJECT">
              <a href = "https://hub.kodland.org/en/project/266574">proyecto 1</a>
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="https://loghi-famosi.com/wp-content/uploads/2021/02/Discord-Logo.png"
                alt="discord"
                width="150"
                height="150"
              />
              <span class="skill__info">info habilidad en</span>
              <input class="skill__button" type="submit" name="button_discord" value="SHOW PROJECT"> 
              <a href = "https://github.com/AlbertoDiego-3/bot-6.0">github bot</a>
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="https://cdn.pixabay.com/photo/2017/10/10/07/01/focus-2836211_1280.png"
                alt="html"
                width="150"
                height="150"
              />
              <span class="skill__info">info habilidad en</span>
              <input class="skill__button" type="submit" name="button_html" value="SHOW PROJECT">
              <a href = "https://github.com/AlbertoDiego-3/vb/blob/main/README.md">mi bigrafia</a>
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/db.webp"
                alt="SQL"
                width="150"
                height="150"
              />
              <span class="skill__info">info habilidad en</span>
              <input class="skill__button" type="submit" name="button_db" value="SHOW PROJECT"> 
            </li>
          </ul>
        </form>
        {% if button_python%}
          <div class="skills__project project" id="project">
              <img class="project__img" src="../static/img/python-project.png" alt="project" width="500"> 
              <a class="project__link" href="">Abierto en GitHub</a>
          </div>
        {% endif %}
      </section>
      <!-- Formulario de contacto -->
      <section class="main__feedback feedback" id="feedback">
        <h2 class="feedback__title">FEEDBACK</h2>
        <form action="" method="POST" class="feedback__form form">
          <label for="email">
            <input type="email" class="form__input" name="email" id="email" placeholder="Escoge un E-mail" required>
          </label>
          <label for="text">
            <textarea name="text" class="form__input" id="text" cols="70" rows="10" required placeholder="Comentarios"></textarea>
          </label>
          <button class="form__button" type="submit">ENVIAR</button>
        </form>
      </section>
    </main>
    <!-- Pie de página con enlaces a redes sociales -->
    <footer>

    </footer>
  </body>
</html>

