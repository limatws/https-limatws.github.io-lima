<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Meu Site</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <header>
        <h1>Meu Site</h1>

        <nav>
            <a href="#inicio">Início</a>
            <a href="#sobre">Sobre</a>
            <a href="#projetos">Projetos</a>
            <a href="#contato">Contato</a>
        </nav>
    </header>

    <main>

        <section id="inicio" class="inicio">
            <h2>Bem-vindo ao meu site!</h2>
            <p>Este site foi criado com HTML, CSS e JavaScript.</p>

            <button onclick="mostrarMensagem()">
                Clique aqui
            </button>

            <p id="mensagem"></p>
        </section>


        <section id="sobre">
            <h2>Sobre mim</h2>

            <p>
                Estou aprendendo desenvolvimento web e este é
                um dos meus primeiros projetos publicados no GitHub.
            </p>
        </section>


        <section id="projetos">
            <h2>Meus Projetos</h2>

            <div class="projetos">

                <div class="card">
                    <h3>Projeto 1</h3>
                    <p>Meu primeiro projeto em HTML.</p>
                </div>

                <div class="card">
                    <h3>Projeto 2</h3>
                    <p>Projeto utilizando HTML e CSS.</p>
                </div>

                <div class="card">
                    <h3>Projeto 3</h3>
                    <p>Projeto utilizando JavaScript.</p>
                </div>

            </div>
        </section>


        <section id="contato">
            <h2>Contato</h2>

            <p>
                Entre em contato comigo através das minhas redes sociais.
            </p>
        </section>

    </main>


    <footer>
        <p>© 2026 Meu Site</p>
    </footer>


    <script src="script.js"></script>

</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background-color: #111827;
    color: white;
}


/* MENU */

header {
    background-color: #0f172a;
    padding: 20px;

    display: flex;
    justify-content: space-between;
    align-items: center;

    position: sticky;
    top: 0;
}

header h1 {
    color: #38bdf8;
}

nav a {
    color: white;
    text-decoration: none;
    margin-left: 20px;
}

nav a:hover {
    color: #38bdf8;
}


/* SEÇÕES */

section {
    min-height: 80vh;
    padding: 80px 10%;
}

section h2 {
    font-size: 35px;
    margin-bottom: 20px;
}


/* INÍCIO */

.inicio {
    min-height: 90vh;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
}

.inicio h2 {
    font-size: 50px;
}

.inicio p {
    margin-bottom: 20px;
    font-size: 18px;
}


/* BOTÃO */

button {
    padding: 12px 25px;

    background-color: #38bdf8;
    color: #111827;

    border: none;
    border-radius: 8px;

    font-weight: bold;
    cursor: pointer;
}

button:hover {
    background-color: #0ea5e9;
}


/* PROJETOS */

.projetos {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}

.card {
    background-color: #1e293b;

    padding: 25px;
    border-radius: 10px;

    width: 250px;

    transition: 0.3s;
}

.card:hover {
    transform: translateY(-10px);
}

.card h3 {
    color: #38bdf8;
    margin-bottom: 10px;
}


/* RODAPÉ */

footer {
    background-color: #0f172a;
    padding: 25px;
    text-align: center;
}


/* CELULAR */

@media (max-width: 700px) {

    header {
        flex-direction: column;
        gap: 15px;
    }

    nav a {
        margin: 0 7px;
    }

    .inicio h2 {
        font-size: 35px;
    }

    section {
        padding: 60px 25px;
    }

    .card {
        width: 100%;
    }
} 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Meu Site</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { font-family: Arial, sans-serif; color: #1f2937; }
    header {
      background: #2563eb; color: white; padding: 80px 20px;
      text-align: center;
    }
    h1 { font-size: 42px; margin-bottom: 15px; }
    section { max-width: 900px; margin: auto; padding: 55px 20px; }
    h2 { color: #2563eb; margin-bottom: 15px; }
    p { line-height: 1.6; margin-bottom: 15px; }
    .botao {
      display: inline-block; background: white; color: #2563eb;
      padding: 12px 20px; border-radius: 6px; text-decoration: none;
      font-weight: bold; margin-top: 10px;
    }
    .servicos { display: flex; gap: 16px; flex-wrap: wrap; }
    .card {
      flex: 1; min-width: 200px; background: #f3f4f6;
      padding: 22px; border-radius: 8px;
    }
    footer { text-align: center; background: #111827; color: white; padding: 22px; }
  </style>
</head>
<body>
  <header>
    <h1>Meu Site</h1>
    <p>Uma presença simples e profissional na internet.</p>
    <a class="botao" href="#contato">Entre em contato</a>
  </header>

  <section>
    <h2>Sobre mim</h2>
    <p>Bem-vindo ao meu site. Aqui você pode apresentar seu trabalho, empresa ou portfólio.</p>
  </section>

  <section>
    <h2>Serviços</h2>
    <div class="servicos">
      <div class="card"><h3>Serviço 1</h3><p>Descrição do primeiro serviço.</p></div>
      <div class="card"><h3>Serviço 2</h3><p>Descrição do segundo serviço.</p></div>
      <div class="card"><h3>Serviço 3</h3><p>Descrição do terceiro serviço.</p></div>
    </div>
  </section>

  <section id="contato">
    <h2>Contato</h2>
    <p>Email: contato@exemplo.com</p>
  </section>

  <footer>© 2026 </footer>
</body>
</html
git init
git add index.html
git commit -m "Publica meu site"
git branch -M main
git remote add origin https://github.com/LIMATWS_.git
git push -u origin main
https://limatws.github.io/limatws/

