<!DOCTYPE html>
<html>
<head>
    <title>uma surpresa pra você do seu futuro namorado</title>
    <style>
        /* Estilo para ajustar a imagem a 30% da largura da página em dispositivos móveis */
        img {
            width: 30vw;
            height: auto;
            display: block;
            margin: 0 auto;
        }

        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #b1cfb29d; /* Definindo uma cor de fundo sólida */
            color: #000000; /* Definindo a cor do texto como preto */
        }

        h1 {
            color: #4287f5;
        }

        .descubra-button,
        .filme-button {
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            margin: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            color: #ffffff;
        }

        .descubra-button {
            background-color: #f29a9a;
        }

        .filme-button {
            background-color: #8cd19d;
        }

        /* Classe para definir a cor do texto do filme escolhido como preto */
        .filme-escolhido {
            color: #000000;
        }
    </style>
</head>
<body>
    <h1>uma surpresa pra você do seu futuro namorado</h1>
    <p>Olá, Senhora Rosalice, vulgo ninhaaa! Bem-vinda ao seu momento de relaxamentooo.</p>
    <button class="descubra-button">Clique e Descubra</button>
    <br>
    <br>
    <p>Clique no botão abaixo para escolher o filme surpresa:</p>
    <button class="filme-button">Escolher Filme Surpresa</button>
    <!-- Elemento com a classe "filme-escolhido" para alterar a cor do texto para preto -->
    <p class="filme-escolhido" id="filmeEscolhido"></p>
    <p id="mensagemEspecial"></p>

    <!-- Imagem aleatória e fofa ajustada a 30% da largura da página -->
    <img src="https://i.imgur.com/OYa7J0g.jpg" alt="Imagem Aleatória Fofa">

    <script>
        const filmesSurpresa = [
            "A Bela e a Fera",
            "O Senhor dos Anéis",
            "O Diabo Veste Prada",
            "Forrest Gump",
            "De Repente 30",
            "Esqueceram de Mim",
            "Mamma Mia!",
            "Jurassic Park",
            "Dirty Dancing",
            "Titanic",
            "Harry Potter e a Pedra Filosofal"
        ];

        function escolherFilmeSurpresa() {
            const indiceFilme = Math.floor(Math.random() * filmesSurpresa.length);
            return filmesSurpresa[indiceFilme];
        }

        document.querySelector(".descubra-button").addEventListener("click", function() {
            alert("você merece uma fabrica de chocolate, mas ainda não cheguei lá ainda, então aproveite uma barrinha pelo menos, amo você..");
        });

        document.querySelector(".filme-button").addEventListener("click", function() {
            const filmeEscolhido = escolherFilmeSurpresa();
            // Utilizando a classe "filme-escolhido" para definir a cor do texto como preto
            document.querySelector("#filmeEscolhido").textContent = `Filme Surpresa: ${filmeEscolhido}`;
            document.querySelector("#mensagemEspecial").textContent = "você merece esse descanso amo você estresadinha"
        });
    </script>
</body>
</html>
