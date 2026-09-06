<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#06111f">

<title>Mídia a Bordo</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #02060b;
    color: white;
    overflow: hidden;
}

/* =========================
   TOPO
========================= */

.topo {
    height: 15vh;
    min-height: 90px;
    background: linear-gradient(135deg, #071a31, #03101e);
    display: grid;
    grid-template-columns: 1.1fr 1.4fr 1fr 1.5fr;
    align-items: center;
    border-bottom: 1px solid #1b5f9e;
    padding: 0 2%;
}

.info {
    display: flex;
    align-items: center;
    gap: 15px;
    padding: 0 20px;
    border-right: 1px solid rgba(255,255,255,.15);
    height: 65%;
}

.icone {
    font-size: clamp(30px, 4vw, 55px);
}

.info h2 {
    font-size: clamp(20px, 2.2vw, 34px);
}

.info p {
    color: #b7c7d9;
    font-size: clamp(11px, 1.2vw, 17px);
    margin-top: 4px;
}

.relogio {
    text-align: center;
}

.hora {
    font-size: clamp(38px, 5vw, 75px);
    font-weight: bold;
    letter-spacing: 2px;
}

.data {
    color: #aebed0;
    font-size: clamp(11px, 1.2vw, 18px);
}

.chamada {
    text-align: center;
    padding: 10px;
}

.chamada strong {
    display: block;
    color: #31c5ff;
    font-size: clamp(17px, 2vw, 30px);
}

.chamada span {
    display: block;
    color: #d7e0e9;
    margin-top: 5px;
    font-size: clamp(10px, 1vw, 15px);
}

/* =========================
   ÁREA DOS ANÚNCIOS
========================= */

.area-anuncios {
    height: 75vh;
    padding: 2vh 1.5vw;
    display: flex;
    align-items: center;
    justify-content: center;
}

.anuncio {
    width: 100%;
    height: 100%;
    border-radius: 24px;
    overflow: hidden;
    position: relative;
    display: grid;
    grid-template-columns: 58% 42%;
    box-shadow: 0 0 45px rgba(0,0,0,.55);
    animation: entrada .7s ease;
}

@keyframes entrada {
    from {
        opacity: 0;
        transform: scale(.97);
    }

    to {
        opacity: 1;
        transform: scale(1);
    }
}

.conteudo {
    padding: 5%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
    z-index: 2;
}

.categoria {
    text-transform: uppercase;
    letter-spacing: 3px;
    font-size: clamp(11px, 1.2vw, 17px);
    font-weight: bold;
    opacity: .85;
    margin-bottom: 15px;
}

.titulo {
    font-size: clamp(38px, 5.5vw, 90px);
    line-height: .95;
    font-weight: 900;
    margin-bottom: 25px;
}

.subtitulo {
    font-size: clamp(17px, 2vw, 30px);
    line-height: 1.25;
    max-width: 850px;
    margin-bottom: 30px;
}

.destaques {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-bottom: 30px;
}

.destaque {
    background: rgba(255,255,255,.14);
    padding: 10px 16px;
    border-radius: 30px;
    font-size: clamp(11px, 1.1vw, 16px);
    backdrop-filter: blur(5px);
}

.contato {
    display: flex;
    align-items: center;
    gap: 20px;
}

.botao {
    background: white;
    color: #111;
    padding: 16px 25px;
    border-radius: 15px;
    font-weight: bold;
    font-size: clamp(14px, 1.4vw, 21px);
}

.numero {
    font-size: clamp(14px, 1.5vw, 23px);
    font-weight: bold;
}

/* =========================
   IMAGEM DO ANÚNCIO
========================= */

.visual {
    position: relative;
    overflow: hidden;
    background-size: cover;
    background-position: center;
}

.visual::after {
    content: "";
    position: absolute;
    inset: 0;
    background: linear-gradient(
        90deg,
        rgba(0,0,0,.35),
        transparent 40%
    );
}

.produto {
    position: absolute;
    inset: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: clamp(100px, 15vw, 260px);
    z-index: 1;
    filter: drop-shadow(0 20px 25px rgba(0,0,0,.4));
}

/* =========================
   QR CODE
========================= */

.qr {
    position: absolute;
    right: 25px;
    bottom: 25px;
    z-index: 5;
    background: white;
    padding: 10px;
    border-radius: 12px;
    text-align: center;
    color: #111;
}

.qr img {
    width: clamp(65px, 7vw, 115px);
    height: clamp(65px, 7vw, 115px);
    display: block;
}

.qr small {
    font-size: 9px;
    display: block;
    margin-top: 5px;
    font-weight: bold;
}

/* =========================
   RODAPÉ
========================= */

.rodape {
    height: 10vh;
    min-height: 65px;
    background: #061322;
    display: flex;
    align-items: center;
    justify-content: space-around;
    border-top: 1px solid #123b5f;
}

.rodape-item {
    display: flex;
    align-items: center;
    gap: 10px;
    color: #c5d4e3;
    font-size: clamp(11px, 1.2vw, 18px);
}

.rodape-icone {
    font-size: clamp(20px, 2vw, 30px);
}

.pontos {
    position: absolute;
    bottom: 11vh;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    gap: 8px;
    z-index: 10;
}

.ponto {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: rgba(255,255,255,.35);
}

.ponto.ativo {
    background: #20bfff;
    transform: scale(1.3);
}

/* =========================
   RESPONSIVO
========================= */

@media(max-width: 700px) {

    .topo {
        grid-template-columns: 1fr 1fr;
        height: 18vh;
    }

    .info:nth-child(3),
    .chamada {
        display: none;
    }

    .info {
        border: none;
    }

    .area-anuncios {
        height: 72vh;
        padding: 10px;
    }

    .anuncio {
        grid-template-columns: 1fr;
    }

    .visual {
        display: none;
    }

    .conteudo {
        padding: 8%;
    }

    .rodape-item:nth-child(2) {
        display: none;
    }
}
</style>
</head>

<body>

<!-- =========================
     TOPO
========================= -->

<header class="topo">

    <div class="info">
        <div class="icone" id="iconeTempo">☀️</div>

        <div>
            <h2 id="temperatura">--°C</h2>
            <p id="descricaoTempo">Carregando...</p>
        </div>
    </div>

    <div class="info">
        <div class="icone">📍</div>

        <div>
            <h2>Campo Mourão - PR</h2>
            <p id="maxmin">Máx. --° | Mín. --°</p>
        </div>
    </div>

    <div class="relogio">
        <div class="hora" id="hora">00:00</div>
        <div class="data" id="data">--</div>
    </div>

    <div class="chamada">
        <strong>📢 PUBLICIDADE A BORDO</strong>
        <span>Conectando passageiros ao comércio local.</span>
    </div>

</header>


<!-- =========================
     ANÚNCIO
========================= -->

<main class="area-anuncios">

    <div id="anuncio" class="anuncio">

        <div class="conteudo">

            <div class="categoria" id="categoria">
                PUBLICIDADE LOCAL
            </div>

            <div class="titulo" id="titulo">
                Carregando...
            </div>

            <div class="subtitulo" id="subtitulo">
                Aguarde...
            </div>

            <div class="destaques" id="destaques"></div>

            <div class="contato">

                <div class="botao" id="botao">
                    Saiba mais
                </div>

                <div class="numero" id="numero">
                    WhatsApp
                </div>

            </div>

        </div>


        <div class="visual" id="visual">

            <div class="produto" id="produto">
                🛍️
            </div>

        </div>


        <div class="qr">

            <img id="qrCode" src="" alt="QR Code">

            <small>Aponte a câmera</small>

        </div>

    </div>

</main>


<!-- =========================
     INDICADORES
========================= -->

<div class="pontos" id="pontos"></div>


<!-- =========================
     RODAPÉ
========================= -->

<footer class="rodape">

    <div class="rodape-item">
        <div class="rodape-icone">📺</div>
        <span id="contador">Anúncio 1 de 3</span>
    </div>

    <div class="rodape-item">
        <div class="rodape-icone">⏱️</div>
        <span>Novos anúncios a cada 10 segundos</span>
    </div>

    <div class="rodape-item">
        <div class="rodape-icone">❤️</div>
        <span>Valorize o comércio local!</span>
    </div>

</footer>


<script>

/* =====================================================
   ⭐ CLIENTES
   =====================================================

   PARA ADICIONAR UM CLIENTE:

   1. Copie um bloco inteiro.
   2. Cole antes do último "];"
   3. Troque as informações.
   4. Salve no GitHub.

   ===================================================== */

const CLIENTES = [

    {
        categoria: "SUPERMERCADO",

        titulo: "Super Mercado<br>Bom Preço",

        subtitulo:
        "Qualidade, variedade e economia para toda sua família!",

        destaques: [
            "🛒 Ofertas",
            "🥦 Hortifruti",
            "🥩 Açougue",
            "🥖 Padaria"
        ],

        botao: "Faça seu pedido",

        telefone: "44 99999-1111",

        whatsapp: "5544999991111",

        emoji: "🛒",

        fundo:
        "linear-gradient(135deg,#075b26,#16a34a,#052e16)"

    },


    {
        categoria: "BARBEARIA",

        titulo: "Barbearia<br>Do João",

        subtitulo:
        "Seu estilo começa aqui. Corte, barba e acabamento profissional.",

        destaques: [
            "✂️ Corte",
            "🧔 Barba",
            "⭐ Profissional",
            "📅 Agendamento"
        ],

        botao: "Agende seu horário",

        telefone: "44 99999-2222",

        whatsapp: "5544999992222",

        emoji: "💈",

        fundo:
        "linear-gradient(135deg,#111827,#374151,#000000)"

    },


    {
        categoria: "DISTRIBUIDORA DE ÁGUA",

        titulo: "Água<br>Safira",

        subtitulo:
        "Água pura e refrescante para sua casa. Peça agora!",

        destaques: [
            "💧 Água mineral",
            "🚚 Entrega rápida",
            "🥤 Garrafa 500ml",
            "🏠 Entrega em casa"
        ],

        botao: "Peça pelo WhatsApp",

        telefone: "44 99999-3333",

        whatsapp: "5544999993333",

        emoji: "💧",

        fundo:
        "linear-gradient(135deg,#0369a1,#0284c7,#082f49)"

    }

];


/* =====================================================
   SISTEMA DE ANÚNCIOS
===================================================== */

let atual = 0;

const tempoAnuncio = 10000;


function mostrarAnuncio() {

    const cliente = CLIENTES[atual];

    const anuncio = document.getElementById("anuncio");

    const categoria =
    document.getElementById("categoria");

    const titulo =
    document.getElementById("titulo");

    const subtitulo =
    document.getElementById("subtitulo");

    const destaques =
    document.getElementById("destaques");

    const botao =
    document.getElementById("botao");

    const numero =
    document.getElementById("numero");

    const visual =
    document.getElementById("visual");

    const produto =
    document.getElementById("produto");

    const qrCode =
    document.getElementById("qrCode");


    /* Atualiza informações */

    categoria.innerHTML = cliente.categoria;

    titulo.innerHTML = cliente.titulo;

    subtitulo.innerHTML = cliente.subtitulo;

    botao.innerHTML = cliente.botao;

    numero.innerHTML = "📲 " + cliente.telefone;


    /* Destaques */

    destaques.innerHTML = "";

    cliente.destaques.forEach(item => {

        const div = document.createElement("div");

        div.className = "destaque";

        div.innerHTML = item;

        destaques.appendChild(div);

    });


    /* Fundo */

    anuncio.style.background =
    cliente.fundo;

    visual.style.background =
    cliente.fundo;


    /* Emoji */

    produto.innerHTML =
    cliente.emoji;


    /* QR Code */

    const mensagem =
    encodeURIComponent(
        "Olá! Vi seu anúncio no tablet do carro e gostaria de saber mais."
    );

    const linkWhatsApp =
    "https://wa.me/" +
    cliente.whatsapp +
    "?text=" +
    mensagem;


    qrCode.src =
    "https://api.qrserver.com/v1/create-qr-code/?size=300x300&data=" +
    encodeURIComponent(linkWhatsApp);


    /* Contador */

    document.getElementById("contador").innerHTML =
    "Anúncio " +
    (atual + 1) +
    " de " +
    CLIENTES.length;


    /* Pontos */

    criarPontos();


    /* Reinicia animação */

    anuncio.style.animation = "none";

    void anuncio.offsetWidth;

    anuncio.style.animation =
    "entrada .7s ease";
}


/* =====================================================
   PONTOS
===================================================== */

function criarPontos() {

    const pontos =
    document.getElementById("pontos");

    pontos.innerHTML = "";

    CLIENTES.forEach((cliente, index) => {

        const ponto =
        document.createElement("div");

        ponto.className = "ponto";

        if(index === atual) {

            ponto.classList.add("ativo");

        }

        pontos.appendChild(ponto);

    });

}


/* =====================================================
   PRÓXIMO ANÚNCIO
===================================================== */

function proximoAnuncio() {

    atual++;

    if(atual >= CLIENTES.length) {

        atual = 0;

    }

    mostrarAnuncio();

}


/* =====================================================
   RELÓGIO
===================================================== */

function atualizarRelogio() {

    const agora =
    new Date();

    const horas =
    String(agora.getHours()).padStart(2,"0");

    const minutos =
    String(agora.getMinutes()).padStart(2,"0");

    const segundos =
    String(agora.getSeconds()).padStart(2,"0");


    document.getElementById("hora").innerHTML =
    horas + ":" + minutos;


    const dias = [
        "Domingo",
        "Segunda-feira",
        "Terça-feira",
        "Quarta-feira",
        "Quinta-feira",
        "Sexta-feira",
        "Sábado"
    ];


    const meses = [
        "Janeiro",
        "Fevereiro",
        "Março",
        "Abril",
        "Maio",
        "Junho",
        "Julho",
        "Agosto",
        "Setembro",
        "Outubro",
        "Novembro",
        "Dezembro"
    ];


    const texto =
    dias[agora.getDay()] +
    ", " +
    String(agora.getDate()).padStart(2,"0") +
    " de " +
    meses[agora.getMonth()];


    document.getElementById("data").innerHTML =
    texto;

}


setInterval(atualizarRelogio,1000);

atualizarRelogio();


/* =====================================================
   PREVISÃO DO TEMPO
   Campo Mourão
===================================================== */

async function buscarTempo() {

    try {

        const latitude = -24.0431;

        const longitude = -52.3783;


        const url =
        "https://api.open-meteo.com/v1/forecast" +
        "?latitude=" + latitude +
        "&longitude=" + longitude +
        "&current=temperature_2m,weather_code" +
        "&daily=temperature_2m_max,temperature_2m_min" +
        "&timezone=America%2FSao_Paulo";


        const resposta =
        await fetch(url);

        const dados =
        await resposta.json();


        const temperatura =
        Math.round(
            dados.current.temperature_2m
        );


        const maxima =
        Math.round(
            dados.daily.temperature_2m_max[0]
        );


        const minima =
        Math.round(
            dados.daily.temperature_2m_min[0]
        );


        document.getElementById("temperatura")
        .innerHTML =
        temperatura + "°C";


        document.getElementById("maxmin")
        .innerHTML =
        "Máx. " +
        maxima +
        "° | Mín. " +
        minima +
        "°";


        const codigo =
        dados.current.weather_code;


        let descricao =
        "Tempo agradável";

        let icone =
        "☀️";


        if(codigo === 0) {

            descricao = "Céu limpo";

            icone = "☀️";

        }

        else if(codigo <= 3) {

            descricao = "Parcialmente nublado";

            icone = "🌤️";

        }

        else if(codigo <= 48) {

            descricao = "Neblina";

            icone = "🌫️";

        }

        else if(codigo <= 67) {

            descricao = "Chuva";

            icone = "🌧️";

        }

        else if(codigo <= 82) {

            descricao = "Pancadas de chuva";

            icone = "🌦️";

        }

        else {

            descricao = "Trovoadas";

            icone = "⛈️";

        }


        document.getElementById("descricaoTempo")
        .innerHTML =
        descricao;


        document.getElementById("iconeTempo")
        .innerHTML =
        icone;

    }

    catch(erro) {

        document.getElementById(
            "descricaoTempo"
        ).innerHTML =
        "Previsão indisponível";

    }

}


buscarTempo();


/* Atualiza previsão a cada 30 minutos */

setInterval(
    buscarTempo,
    30 * 60 * 1000
);


/* =====================================================
   INICIA SISTEMA
===================================================== */

mostrarAnuncio();


setInterval(
    proximoAnuncio,
    tempoAnuncio
);

</script>

</body>
</html>
