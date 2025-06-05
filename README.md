<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <title>Portfólio de Brayan</title>
</head>

<body>
    <header class="container text-center">
        <img src="img/avatar-perfil.png" alt="avatar do Brayan" class="rounded-circle" width="150" height="150">
        <p class="lead">Olá, eu sou Brayan</p>
        <h1>Desenvolvedor iniciante em JavaScript e Scratch</h1>
        <p>Tenho experiência básica em programação e robótica. Estou aprendendo e aplicando conhecimentos em tecnologias como JavaScript para desenvolvimento web e Scratch para criação de projetos interativos.</p>
        <p>Minhas habilidades</p>
        <div>
            <p class="badge bg-secondary">JavaScript</p>
            <p class="badge bg-secondary">Scratch</p>
        </div>
    </header>

    <main class="container mt-5">
        <h2>Meus Projetos</h2>
        <div class="row">
            <!-- Projeto 1 -->
            <div class="col-md-4">
                <div class="card">
                    <img src="img/projeto-1.png" class="card-img-top" alt="Imagem do projeto Scratch">
                    <div class="card-body">
                        <h5 class="card-title">Jogo Interativo em Scratch</h5>
                        <p class="card-text">Criei um jogo simples onde o jogador controla um personagem que deve evitar obstáculos. Aprendi a usar lógica de programação através de blocos visuais.</p>
                        <button type="button" class="btn btn-link" data-bs-toggle="modal" data-bs-target="#modal1">Veja o projeto</button>
                    </div>
                </div>
            </div>

            <!-- Projeto 2 -->
            <div class="col-md-4">
                <div class="card">
                    <img src="img/projeto-2.png" class="card-img-top" alt="Imagem do projeto de To-Do List">
                    <div class="card-body">
                        <h5 class="card-title">To-Do List com JavaScript</h5>
                        <p class="card-text">Desenvolvi uma lista de tarefas onde é possível adicionar, remover e marcar tarefas como concluídas. Foi meu primeiro projeto em JavaScript e HTML.</p>
                        <button type="button" class="btn btn-link" data-bs-toggle="modal" data-bs-target="#modal2">Veja o projeto</button>
                    </div>
                </div>
            </div>

            <!-- Projeto 3 -->
            <div class="col-md-4">
                <div class="card">
                    <img src="img/projeto-3.png" class="card-img-top" alt="Imagem do projeto de robô Arduino">
                    <div class="card-body">
                        <h5 class="card-title">Robô Simples com Arduino</h5>
                        <p class="card-text">Criei um robô que se move e evita obstáculos utilizando sensores. Esse projeto me ajudou a entender os conceitos básicos de robótica e programação de hardware.</p>
                        <button type="button" class="btn btn-link" data-bs-toggle="modal" data-bs-target="#modal3">Veja o projeto</button>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <!-- Modal 1 -->
    <div class="modal" id="modal1" tabindex="-1">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Jogo Interativo em Scratch</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <p>Este projeto foi desenvolvido no Scratch, uma plataforma de programação visual. O jogo permite ao jogador controlar um personagem que deve evitar obstáculos em um cenário 2D. Aprendi conceitos como loops e condições usando blocos de código.</p>
                    <img src="img/projeto-1.png" class="img-fluid w-100" alt="Imagem representativa do jogo em Scratch">
                </div>
                <div class="modal-footer">
                    <a href="https://scratch.mit.edu/projects/xyz">Ver projeto ao vivo</a>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 2 -->
    <div class="modal" id="modal2" tabindex="-1">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">To-Do List com JavaScript</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <p>O projeto de To-Do List foi desenvolvido com HTML, CSS e JavaScript. Ele permite ao usuário adicionar tarefas, marcar como concluídas e deletar tarefas. Este foi um projeto fundamental para entender como manipular o DOM com JavaScript.</p>
                    <img src="img/projeto-2.png" class="img-fluid w-100" alt="Imagem representativa da To-Do List">
                </div>
                <div class="modal-footer">
                    <a href="https://meu-site.com/todolist">Ver projeto ao vivo</a>
                    <a href="https://github.com/brayan/todolist">Ver código do projeto</a>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 3 -->
    <div class="modal" id="modal3" tabindex="-1">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Robô Simples com Arduino</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <p>Este projeto envolve um robô simples controlado por Arduino. O robô é programado para se mover automaticamente e evitar obstáculos usando sensores ultrassônicos. Esse projeto foi uma excelente introdução à robótica e programação de hardware.</p>
                    <img src="img/projeto-3.png" class="img-fluid w-100" alt="Imagem representativa do robô">
                </div>
                <div class="modal-footer">
                    <a href="https://github.com/settings/profile">Ver código do projeto</a>
                </div>
            </div>
        </div>
    </div>

    <footer class="container py-5">
        <h2>Entre em contato</h2>
        <div>
            <i class="bi bi-github"></i>
            <a href="https://github.com/brayan">GitHub</a>
        </div>
        <p class="my-5 text-center">© Copyright 2024. Produzido por Brayan</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>

</html>
