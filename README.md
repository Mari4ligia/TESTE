<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Academia</title>
<style>
  body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    background-color: #f0f0f0;
  }
  .container {
    text-align: center;
  }
  .logo {
    width: 150px;
    height: auto;
  }
  .buttons {
    margin-top: 20px;
  }
  .btn {
    display: inline-block;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    border-radius: 5px;
    background-color: #007bff;
    color: #fff;
    text-decoration: none;
    transition: background-color 0.3s;
  }
  .btn:hover {
    background-color: #0056b3;
  }
  .btn.disabled {
    background-color: #ccc;
    cursor: not-allowed;
  }
</style>
</head>
<body>

<div class="container">
  <h1>Academia</h1>
  <img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.canva.com%2Fpt_br%2Flogos%2Fmodelos%2Facademia%2F&psig=AOvVaw3Vc5XObmU57zFZcoTJUVxw&ust=1720283098809000&source=images&cd=vfe&opi=89978449&ved=0CA8QjRxqFwoTCOjZv4qokIcDFQAAAAAdAAAAABAE" alt="Logo da Academia" class="logo">
  <h2>Vamos à academia hoje?</h2>
  
  <div class="buttons">
    <button id="btnSim" class="btn">Sim</button>
    <button id="btnNao" class="btn">Não</button>
  </div>
  
  <div id="mensagem" style="margin-top: 20px;"></div>
</div>

<script>
  document.getElementById('btnSim').addEventListener('click', function() {
    document.getElementById('mensagem').innerHTML = '<h3>Certeza?? 🎉🎉</h3>';
    
  });

  document.getElementById('btnNao').addEventListener('click', function() {
    document.getElementById('btnNao').classList.add('disabled');
    document.getElementById('btnNao').setAttribute('disabled', 'true');
  });
</script>

</body>
</html>

