# uc-15-18
<!DOCTYPE html>
<html>
<head>
    <title>Viagem</title>
    <script src="javas.js"></script>
</head>

<body>

    <h1 id="titulo">caminhão</h1>

    <input id="cidade" placeholder="Digite uma cidade">

    <button onclick="mostrarCidade()">Mostrar</button>

    <p id="mensagem"></p>

    <button onclick="destacar()">Destacar</button>

    <h2>Contador</h2>

    <button onclick="menos()">-</button>

    <span id="contador">100</span>

    <button onclick="mais()">+</button>

    <script>
        let contador = 10;

        function mostrarCidade() {
            let cidade = document.getElementById("cidade").value;

            document.getElementById("mensagem").textContent =
                "Quero conhecer " + cidade + "!";
        }

        function destacar() {
            document.getElementById("mensagem").style.color = "red";
            document.getElementById("mensagem").style.fontSize = "25px";
        }

        function mais() {
            contador = contador + 1;
            document.getElementById("contador").textContent = contador;
        }

        function menos() {
            contador = contador - 1;
            document.getElementById("contador").textContent = contador;
        }
    </script>

</body>
</html>

let contador = 10;

function mostrarCidade() {
    let cidade = document.getElementById("cidade").value;
    document.getElementById("mensagem").textContent = "Você escolheu " + cidade;
}

function destacar() {
    document.getElementById("mensagem").style.color = "red";
    document.getElementById("mensagem").style.fontSize = "25px";
}

function mais() {
    contador++;
    document.getElementById("contador").textContent = contador;
}

function menos() {
    contador--;
    document.getElementById("contador").textContent = contador;
}
