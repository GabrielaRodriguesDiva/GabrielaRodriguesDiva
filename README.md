<main>
    <div class="passo ativo" id="passo-0">
        <img src="img/cenario-passo0.png" alt="">
        <p>Um dia desses, dentro de um livro da biblioteca da escola, eu descobri uma carta antiga sobre uma cidade perdida, escondida por riquezas e belezas naturais. Nessa carta, a autora deixa algumas pistas para encontrar essa cidade e eu decidi segui-las!</p>
        <button class="btn-proximo" data-proximo="1">Rio de Janeiro</button>
        <button class="btn-proximo" data-proximo="2">Pernambuco</button>
    </div>
    <div class="passo" id="passo-1">
        <p>Você começa sua jornada no Rio de Janeiro, subindo o Pico da Tijuca ao amanhecer para encontrar a primeira pista.</p>
        <button class="btn-proximo" data-proximo="3">Procurar a pista no topo do pico</button>
        <button class="btn-proximo" data-proximo="4">Desistir e voltar para casa</button>
    </div>
    <div class="passo" id="passo-2">
        <p>Em Pernambuco, você visita a histórica cidade de Olinda. Na carta, uma das pistas indica que para localizar a entrada para a cidade perdida você deve procurar a próxima pista em um dos pontos turísticos da cidade. Por qual você começa?</p>
        <button class="btn-proximo" data-proximo="5">Investigar as igrejas antigas</button>
        <button class="btn-proximo" data-proximo="6">Explorar as praias próximas</button>
    </div>
        </main>
        
body {
    background-color: #1D4221;
    color: white;
    font-family: "Bai Jamjuree", sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 700px;
    margin: 0;
}

button {
    background-color: #64A712;
    color: white;
    font-family: "Bai Jamjuree", sans-serif;
}

h1 {
    color: #FF6347; /* Cor do texto */
  }
  
  body {
    background-color: #E6E6FA; /* Cor de fundo */
  }
  const avanca = document.querySelectorAll('.btn-proximo');

avanca.forEach(button => {
    button.addEventListener('click', function(){
        const atual = document.querySelector('.ativo');
        const proximoPasso = 'passo-' + this.getAttribute('data-proximo');

        atual.classList.remove('ativo');
        document.getElementById(proximoPasso).classList.add('ativo');
    })
})
<!-- código omitido -->

<script src="script.js"></script>
</body>
</html>
let botao = document.querySelector('.meu-botao');
let paragrafos = document.querySelectorAll('p');
<div class="passo ativo" id="passo-0">
    <img src="cenario-passo0.png" alt="">
    <p>Um dia desses, dentro de um livro da biblioteca da escola, descobri uma carta antiga sobre uma cidade perdida, escondida por riquezas e belezas naturais. Nessa carta, a autora deixa algumas pistas para encontrar essa cidade e eu decidi segui-las!</p>
    <button class="btn-proximo" data-proximo="1">Rio de Janeiro</button>
    <button class="btn-proximo" data-proximo="2">Pernambuco</button>
</div>
