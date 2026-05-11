[contato.html](https://github.com/user-attachments/files/27602254/contato.html)
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contato - Lucas Lima Emerici</title>
    <link rel="stylesheet" href="style.css">
</head>[style.css](https://github.com/user-attachments/files/27602259/style.css)
[sobre.html](https://github.com/user-attachments/files/27602258/sobre.html)
[portfolio.html](https://github.com/user-attachments/files/27602257/portfolio.html)
[index.html](https://github.com/user-attachments/files/27602256/index.html)
[formacao.html](https://github.com/user-attachments/files/27602255/formacao.html)

<body>

<header>
        <nav>
            <ul>
                <li><a href="sobre.html">Sobre mim</a></li>
                <li><a href="formacao.html">Formação</a></li>
                <li><a href="portfolio.html">Portfólio</a></li>
                <li><a href="contato.html" class="active">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="contato">
            <h1>Entre em Contato</h1>
            <p>Preencha o formulário abaixo para me enviar uma mensagem. Retornarei o mais breve possível!</p>
            
            <form id="formContato">
                <div>
                    <label for="nome">Nome Completo:</label>
                    <input type="text" id="nome" placeholder="Digite seu nome">
                </div>

                <div>
                    <label for="email">E-mail:</label>
                    <input type="email" id="email" placeholder="usuario@dominio.com">
                </div>

                <div>
                    <label for="mensagem">Mensagem:</label>
                    <textarea id="mensagem" placeholder="Escreva sua mensagem aqui..."></textarea>
                </div>

                <button type="submit">Enviar Mensagem</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 - Lucas Lima Emerici. Desenvolvido para a disciplina Desenvolvimento Web.</p>
    </footer>

    <script>
        const form = document.getElementById('formContato');

        form.addEventListener('submit', function(event) {            
            event.preventDefault();  // Previne o recarregamento padrão da página ao enviar o formulário
           
            const nome = document.getElementById('nome').value.trim();
            const email = document.getElementById('email').value.trim();
            const mensagem = document.getElementById('mensagem').value.trim();
         
            if (nome === '' || email === '' || mensagem === '') {
                alert('Por favor, preencha todos os campos antes de enviar.');
                return; // Para a execução aqui se houver erro
            }
           
            const regexEmail = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;  // Expressão regular para validar se o formato do e-mail está correto
            if (!regexEmail.test(email)) {
                alert('Por favor, insira um endereço de e-mail válido (ex: usuario@dominio.com).');
                return; 
            }
          
            alert('Mensagem enviada com sucesso!');
            form.reset(); 
        });
    </script>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formação - Lucas Lima Emerici</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <nav>
            <ul>
                <li><a href="sobre.html">Sobre mim</a></li>
                <li><a href="formacao.html" class="active">Formação</a></li>
                <li><a href="portfolio.html">Portfólio</a></li>
                <li><a href="contato.html">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="formacao">
            <h1>Formação e Experiência</h1>
            
            <h2>Educação Acadêmica</h2>
            <div style="margin-bottom: 20px;">
                <h3>Bacharelado em Ciência da Computação</h3>
                <p><strong>Instituição:</strong> Uninter</p>
                <p><strong>Período:</strong> Em andamento (Previsão de conclusão em 2028)</p>
                <p>
                    Foco no desenvolvimento de software, algoritmos e fundamentos da computação. 
                    Aprofundamento prático e teórico em disciplinas como Hardware e Redes de Computadores.
                </p>
            </div>

            <h2>Experiência Profissional</h2>
            <div style="margin-bottom: 20px;">
                <h3>Assistente Financeiro</h3>
                <p><strong>Empresa:</strong> Gasparini Transportes</p>
                <p><strong>Período:</strong> 2020 - 2021</p>
                <p>
                    Atuação em rotinas administrativas e financeiras, com forte foco em emissão de notas fiscais, 
                    controle de faturamento e organização de processos internos.
                </p>
            </div>

            <h2>Cursos Complementares e Idiomas</h2>
            <ul class="lista-hobbies">
                <li>
                    <strong>Introduction to cybersecurity - Cisco</strong> 
                </li>
                <li>
                    <strong>Introduction to networking - Cisco</strong>
                </li>
                <li>
                    <strong>Principios da Segurança - DIO</strong>
                </li>
                <li>
                    <strong>Inglês: Nível Avançado.</strong>
                </li>
            </ul>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 - Lucas Lima Emerici. Desenvolvido para a disciplina Desenovlvimento Web.</p>
    </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Início - Lucas Lima Emerici</title>
    <link rel="stylesheet" href="style.css">
</head>
<body class="home-body"> <main class="home-container">
    
        <section class="boas-vindas">
            <h1>Bem-vindo ao meu Portfólio!</h1>
            <p>Olá, sou o Lucas Lima Emerici. Estudante de Ciência da Computação apaixonado por Cybersegurança e Hardware.</p>
            <p>Escolha uma seção para navegar:</p>
            
            <div class="botoes-home">
                <a href="sobre.html" class="btn-home">👨‍💻 Sobre mim</a>
                <a href="formacao.html" class="btn-home">🎓 Formação</a>
                <a href="portfolio.html" class="btn-home">🚀 Portfólio</a>
                <a href="contato.html" class="btn-home">✉️ Contato</a>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 - Lucas Lima Emerici. Desenvolvido para a disciplina Desenvolvimento Web.</p>
    </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio - Lucas Lima Emerici</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <nav>
            <ul>
                <li><a href="sobre.html">Sobre mim</a></li>
                <li><a href="formacao.html">Formação</a></li>
                <li><a href="portfolio.html" class="active">Portfólio</a></li>
                <li><a href="contato.html">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="portfolio">
            <h1>Meu Portfólio</h1>
            <p>
                Abaixo estão alguns projetos e implementações lógicas que desenvolvi, unindo 
                os conhecimentos da Ciência da Computação com resoluções de problemas do meu dia a dia.
            </p>

            <div style="margin-bottom: 25px; padding: 20px; border: 1px solid #ddd; border-radius: 8px;">
                <h3>Cofrinho</h3>
                <p><strong>Descrição:</strong> Projeto feito para trabalho de faculdade, em que temos um cofrinho e podemos adicionar moedas de diferentes tipos, como dólar, euro e real, e também podendo ver o quantia total em real.</p>
                <p><strong>Tecnologias:</strong> Java.</p>
                <a href="https://github.com/lemerici/TrabalhoCofrinho" target="_blank" style="color: #0c2c4d; font-weight: bold; text-decoration: none;">Ver projeto no GitHub</a>
            </div>

            <div style="margin-bottom: 25px; padding: 20px; border: 1px solid #ddd; border-radius: 8px;">
                <h3>ChatBot</h3>
                <p><strong>Descrição:</strong> Projeto feito para atividade extensionista, onde temos um chatbot para tirar duvidas sobre ongs.</p>
                <p><strong>Tecnologias:</strong> Python.</p>
                <a href="https://github.com/lemerici/ChatBot" target="_blank" style="color: #0c2c4d; font-weight: bold; text-decoration: none;">Ver projeto no GitHub</a>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 - Lucas Lima Emerici. Desenvolvido para a disciplina Desenovlimento Web.</p>
    </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio - Lucas Lima Emerici</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <nav>
            <ul>
                <li><a href="sobre.html" class="active">Sobre mim</a></li>
                <li><a href="formacao.html">Formação</a></li>
                <li><a href="portfolio.html">Portfólio</a></li>
                <li><a href="contato.html">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="sobre">
            <h1>Olá, eu sou Lucas Lima Emerici!</h1>
            <h2>Estudante de Ciência da Computação</h2>
            
            <p>
                Bem-vindo(a) ao meu portfólio online. Sou um grande entusiasta da tecnologia, atualmente cursando 
                o bacharelado em Ciência da Computação, com previsão de formatura para 2028. Tenho um perfil analítico 
                e estou direcionando meus estudos para a área de Tecnologia da Informação na área de cybersegurança e infraestrutura/hardware.
            </p>
            <p>
                Profissionalmente, já atuei como assistente financeiro lidando com rotinas de faturamento e emissão de notas fiscais, 
                o que me trouxe uma sólida experiência em organização de processos e visão administrativa. Hoje, minha rotina é dividida 
                entre o aprofundamento em disciplinas técnicas — como Cybersegurança e Hardware — e meus projetos pessoais.
            </p>
            
            <h3>Meus Hobbies</h3>
            <ul class="lista-hobbies">
                <li><strong>Musculação e Vida Saudável:</strong> Mantenho uma rotina de treinos para garantir foco e disciplina, aliado a uma dieta estruturada.</li>
                <li><strong>Hardware de PC:</strong> Sou aficionado por montar e otimizar computadores. Adoro pesquisar especificações de placas-mãe, processadores e fazer testes de estresse em GPUs.</li>
                <li><strong>Games:</strong> Nas horas de lazer, gosto de jogar e ler.</li>
            </ul>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 - Lucas Lima Emerici. Desenvolvido para a disciplina Desenvolvimento Web.</p>
    </footer>

</body>
</html>
/* Reset básico para padronizar o layout em todos os navegadores */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}


html, body {
    margin: 0;
    padding: 0;
    width: 100%;
}

/* Estilização do Menu Fixo e Navegação */
header {
    background-color: #0c2c4d; 
    position: fixed; 
    top: 0;      
    left: 0;     
    width: 100%;
    height: 60px;
    z-index: 1000;
    display: flex;
    align-items: center; 
    justify-content: center;
}

nav {
    width: 100%;
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
    padding: 0;
    height: 100%;
}

body {
    padding-top: 80px; 
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    font-size: 1.1rem;
    font-weight: bold;
    padding: 10px 15px;
    border-radius: 5px;
    transition: background-color 0.3s;
}

nav ul li a:hover, nav ul li a.active {
    background-color: #2c344b; 
}

main {
    max-width: 800px;
    margin: 40px auto;
    padding: 30px;
    background-color: #fff;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

h1, h2, h3 {
    margin-bottom: 15px;
    color: #2c3e50;
}

/* Classe criada para centralizar os botões apenas na Landing Page */
.home-body {
    padding-top: 0 !important;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

.home-body .home-container {
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto;
}

.home-container {
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 55vh;
}

.boas-vindas h1 {
    font-size: 2.5rem;
    color: #0c2c4d;
    margin-bottom: 15px;
}

.boas-vindas p {
    font-size: 1.2rem;
    color: #555;
    margin-bottom: 10px;
    text-align: center;
}

.botoes-home {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    margin-top: 40px;
}

.btn-home {
    display: inline-block;
    padding: 20px 10px;
    font-size: 1.2rem;
    font-weight: bold;
    color: #fff;
    background-color: #0c2c4d;
    text-decoration: none;
    border-radius: 8px;
    transition: background-color 0.3s, transform 0.2s;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    width: 200px;
}

.btn-home:hover {
    background-color: #2c344b;
    transform: translateY(-5px);
}

p {
    line-height: 1.6;
    margin-bottom: 15px;
    text-align: justify;
}

.lista-hobbies {
    margin-left: 20px;
    margin-top: 10px;
}

.lista-hobbies li {
    margin-bottom: 10px;
    line-height: 1.5;
}

footer {
    display: flex;
    justify-content: center;
    align-items: center; 
    text-align: center;
    padding: 15px;
    background-color: #0c2c4d;
    color: #fff;
    width: 100%;
    margin-top: 50px;
    min-height: 60px;
}

form {
    display: flex;
    flex-direction: column;
    gap: 15px;
    margin-top: 20px;
}

label {
    font-weight: bold;
    color: #2c3e50;
}

input, textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 1rem;
    width: 100%;
}

textarea {
    resize: vertical;
    min-height: 120px;
}

button {
    padding: 12px;
    background-color: #2c3e50;
    color: #fff;
    border: none;
    border-radius: 5px;
    font-size: 1.1rem;
    font-weight: bold;
    cursor: pointer;
    transition: background-color 0.3s;
}

button:hover {
    background-color: #1abc9c;
}

