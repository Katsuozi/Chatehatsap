<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Fale Comigo no WhatsApp</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      text-align: center;
      padding: 50px;
    }
    .container {
      background-color: #fff;
      padding: 30px;
      max-width: 400px;
      margin: 0 auto;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    input {
      padding: 10px;
      width: 90%;
      margin-bottom: 20px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 16px;
    }
    button {
      background-color: #25D366;
      color: white;
      border: none;
      padding: 12px 20px;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
    }
    button:hover {
      background-color: #1ebe57;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Quer saber mais sobre os empreendimentos?</h2>
    <p>Digite seu telefone e fale comigo no WhatsApp:</p>
    <input type="tel" id="phoneInput" placeholder="(19) 98271-7457">
    <button onclick="enviarWhatsApp()">Falar no WhatsApp</button>
  </div>

  <script>
    function enviarWhatsApp() {
      const phone = document.getElementById("phoneInput").value;
      const numeroCorretor = "5511999999999"; // coloque aqui seu número com DDI (ex: 55 + DDD + número)
      const mensagem = `Olá! Meu telefone é ${phone}, vi o site e gostaria de saber mais sobre os empreendimentos em Piracicaba.`;
      const url = `https://wa.me/${numeroCorretor}?text=${encodeURIComponent(mensagem)}`;
      window.open(url
