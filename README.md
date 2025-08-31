<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Selecione Pacotes de Fraldas</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f7faff;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      min-height: 100vh;
    }
    .container {
      margin-top: 3rem;
      padding: 2rem;
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.08);
      width: 100%;
      max-width: 1100px;
    }
    h1 {
      color: #2b2d42;
      font-size: 1.3rem;
      margin-bottom: 1.2rem;
      text-align: center;
    }
    .cards-title {
      font-size: 1.15em;
      font-weight: bold;
      margin: 1.3em 0 0.6em 0;
      color: #457;
      text-align: center;
      width: 100%;
    }
    .cards-group {
      display: flex;
      gap: 1.2rem;
      justify-content: flex-start;
      flex-wrap: wrap;
      margin-bottom: 2rem;
    }
    .card {
      background: #fcf9e7;
      border: 1px solid #e0e5ec;
      border-radius: 8px;
      padding: 1.2rem 1rem;
      box-shadow: 0 1px 4px rgba(44, 62, 80, 0.06);
      width: 135px;
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-bottom: 1rem;
    }
    .card-desc {
      font-weight: bold;
      font-size: 1.1em;
      margin-bottom: 0.7em;
      color: #2b2d42;
    }
    .card-size {
      margin-bottom: 1em;
      color: #666;
      font-size: 0.97em;
    }
    .label-fraldas {
      background: #d8f3dc;
      color: #234;
      padding: 0.33em 1.1em;
      border-radius: 12px;
      font-size: 0.95em;
      margin-bottom: 1em;
      font-weight: bold;
    }
    .nome-input {
      border: 1px solid #b2b6c1;
      border-radius: 4px;
      padding: 0.4em;
      font-size: 1em;
      margin-bottom: 0.5em;
      width: 95%;
      box-sizing: border-box;
      text-align: center;
    }
    .select-btn {
      background: #a86e44;
      color: #fff;
      border: none;
      border-radius: 6px;
      padding: 0.5em 1.2em;
      font-size: 1em;
      cursor: pointer;
      margin-top: 0.5em;
      transition: background 0.2s;
    }
    .select-btn.selected {
      background: #1b8030;
    }
    .resultado {
      margin-top: 1.4rem;
      text-align: center;
      font-weight: bold;
      color: #2b2d42;
      min-height: 1.2em;
    }
    @media (max-width: 1100px) {
      .container { max-width: 99vw; }
      .cards-group { justify-content: center; }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Selecione um pacote e coloque seu nome</h1>
    <!-- RN -->
    <div class="cards-title">Tamanho RN</div>
    <div class="cards-group" id="cards-rn">
      <div class="card" id="cardRN1">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: RN 1</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeRN1" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnRN1">Quero dar este!</button>
      </div>
      <div class="card" id="cardRN2">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: RN 2</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeRN2" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnRN2">Quero dar este!</button>
      </div>
      <div class="card" id="cardRN3">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: RN 3</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeRN3" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnRN3">Quero dar este!</button>
      </div>
    </div>
    <!-- P -->
    <div class="cards-title">Tamanho P</div>
    <div class="cards-group" id="cards-p">
      <!-- 7 pacotes P -->
      <div class="card" id="cardP1">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: P 1</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeP1" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnP1">Quero dar este!</button>
      </div>
      <div class="card" id="cardP2">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: P 2</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeP2" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnP2">Quero dar este!</button>
      </div>
      <div class="card" id="cardP3">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: P 3</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeP3" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnP3">Quero dar este!</button>
      </div>
      <div class="card" id="cardP4">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: P 4</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeP4" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnP4">Quero dar este!</button>
      </div>
      <div class="card" id="cardP5">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: P 5</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeP5" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnP5">Quero dar este!</button>
      </div>
      <div class="card" id="cardP6">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: P 6</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeP6" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnP6">Quero dar este!</button>
      </div>
      <div class="card" id="cardP7">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: P 7</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeP7" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnP7">Quero dar este!</button>
      </div>
    </div>
    <!-- M -->
    <div class="cards-title">Tamanho M</div>
    <div class="cards-group" id="cards-m">
      <!-- 10 pacotes M -->
      <div class="card" id="cardM1">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 1</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM1" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM1">Quero dar este!</button>
      </div>
      <div class="card" id="cardM2">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 2</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM2" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM2">Quero dar este!</button>
      </div>
      <div class="card" id="cardM3">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 3</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM3" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM3">Quero dar este!</button>
      </div>
      <div class="card" id="cardM4">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 4</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM4" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM4">Quero dar este!</button>
      </div>
      <div class="card" id="cardM5">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 5</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM5" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM5">Quero dar este!</button>
      </div>
      <div class="card" id="cardM6">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 6</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM6" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM6">Quero dar este!</button>
      </div>
      <div class="card" id="cardM7">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 7</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM7" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM7">Quero dar este!</button>
      </div>
      <div class="card" id="cardM8">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 8</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM8" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM8">Quero dar este!</button>
      </div>
      <div class="card" id="cardM9">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 9</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM9" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM9">Quero dar este!</button>
      </div>
      <div class="card" id="cardM10">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: M 10</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeM10" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnM10">Quero dar este!</button>
      </div>
    </div>
    <!-- G -->
    <div class="cards-title">Tamanho G</div>
    <div class="cards-group" id="cards-g">
      <!-- 8 pacotes G -->
      <div class="card" id="cardG1">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: G 1</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeG1" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnG1">Quero dar este!</button>
      </div>
      <div class="card" id="cardG2">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: G 2</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeG2" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnG2">Quero dar este!</button>
      </div>
      <div class="card" id="cardG3">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: G 3</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeG3" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnG3">Quero dar este!</button>
      </div>
      <div class="card" id="cardG4">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: G 4</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeG4" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnG4">Quero dar este!</button>
      </div>
      <div class="card" id="cardG5">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: G 5</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeG5" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnG5">Quero dar este!</button>
      </div>
      <div class="card" id="cardG6">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: G 6</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeG6" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnG6">Quero dar este!</button>
      </div>
      <div class="card" id="cardG7">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: G 7</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeG7" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnG7">Quero dar este!</button>
      </div>
      <div class="card" id="cardG8">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: G 8</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeG8" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnG8">Quero dar este!</button>
      </div>
    </div>
    <!-- XG -->
    <div class="cards-title">Tamanho XG</div>
    <div class="cards-group" id="cards-xg">
      <!-- 5 pacotes XG -->
      <div class="card" id="cardXG1">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: XG 1</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeXG1" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnXG1">Quero dar este!</button>
      </div>
      <div class="card" id="cardXG2">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: XG 2</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeXG2" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnXG2">Quero dar este!</button>
      </div>
      <div class="card" id="cardXG3">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: XG 3</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeXG3" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnXG3">Quero dar este!</button>
      </div>
      <div class="card" id="cardXG4">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: XG 4</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeXG4" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnXG4">Quero dar este!</button>
      </div>
      <div class="card" id="cardXG5">
        <div class="card-desc"><b>Pacote</b></div>
        <div class="card-size">Tamanho: XG 5</div>
        <div class="label-fraldas">Fraldas</div>
        <input type="text" class="nome-input" id="nomeXG5" placeholder="Seu nome">
        <button type="button" class="select-btn" id="btnXG5">Quero dar este!</button>
      </div>
    </div>
    <div class="resultado" id="resultado"></div>
  </div>
  <script>
    const resultado = document.getElementById('resultado');
    // Função para seleção RN
    for(let i=1;i<=3;i++){
      document.getElementById('btnRN'+i).addEventListener('click', function() {
        let nome = document.getElementById('nomeRN'+i).value.trim();
        if (!nome) {
          resultado.textContent = `Por favor, digite seu nome para o Pacote RN ${i}.`;
          return;
        }
        for(let j=1;j<=3;j++) document.getElementById('btnRN'+j).classList.remove('selected');
        this.classList.add('selected');
        resultado.textContent = `Você selecionou o Pacote RN ${i}! Nome: ${nome}`;
      });
    }
    // Função para seleção P
    for(let i=1;i<=7;i++){
      document.getElementById('btnP'+i).addEventListener('click', function() {
        let nome = document.getElementById('nomeP'+i).value.trim();
        if (!nome) {
          resultado.textContent = `Por favor, digite seu nome para o Pacote P ${i}.`;
          return;
        }
        for(let j=1;j<=7;j++) document.getElementById('btnP'+j).classList.remove('selected');
        this.classList.add('selected');
        resultado.textContent = `Você selecionou o Pacote P ${i}! Nome: ${nome}`;
      });
    }
    // Função para seleção M
    for(let i=1;i<=10;i++){
      document.getElementById('btnM'+i).addEventListener('click', function() {
        let nome = document.getElementById('nomeM'+i).value.trim();
        if (!nome) {
          resultado.textContent = `Por favor, digite seu nome para o Pacote M ${i}.`;
          return;
        }
        for(let j=1;j<=10;j++) document.getElementById('btnM'+j).classList.remove('selected');
        this.classList.add('selected');
        resultado.textContent = `Você selecionou o Pacote M ${i}! Nome: ${nome}`;
      });
    }
    // Função para seleção G
    for(let i=1;i<=8;i++){
      document.getElementById('btnG'+i).addEventListener('click', function() {
        let nome = document.getElementById('nomeG'+i).value.trim();
        if (!nome) {
          resultado.textContent = `Por favor, digite seu nome para o Pacote G ${i}.`;
          return;
        }
        for(let j=1;j<=8;j++) document.getElementById('btnG'+j).classList.remove('selected');
        this.classList.add('selected');
        resultado.textContent = `Você selecionou o Pacote G ${i}! Nome: ${nome}`;
      });
    }
    // Função para seleção XG
    for(let i=1;i<=5;i++){
      document.getElementById('btnXG'+i).addEventListener('click', function() {
        let nome = document.getElementById('nomeXG'+i).value.trim();
        if (!nome) {
          resultado.textContent = `Por favor, digite seu nome para o Pacote XG ${i}.`;
          return;
        }
        for(let j=1;j<=5;j++) document.getElementById('btnXG'+j).classList.remove('selected');
        this.classList.add('selected');
        resultado.textContent = `Você selecionou o Pacote XG ${i}! Nome: ${nome}`;
      });
    }
  </script>
</body>
</html>
