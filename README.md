
````html
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
            <button onclick="mostrarMensagem()">Clique aqui</button>
            <p id="mensagem"></p>
        </section>

        <section id="sobre">
            <h2>Sobre mim</h2>
            <p>Estou aprendendo desenvolvimento web e este é um dos meus primeiros projetos publicados no GitHub.</p>
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
            <p>Entre em contato comigo através das minhas redes sociais.</p>
        </section>
    </main>

    <footer>
        <p>© 2026 Meu Site</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
````

````css
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
````

````javascript
function mostrarMensagem() {
    document.getElementById("mensagem").textContent = "Olá! Você clicou no botão!";

