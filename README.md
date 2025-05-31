<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>FlashMoney</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body { font-family: sans-serif; background: #f0f9ff; margin: 0; padding: 0; }
    .container { max-width: 800px; margin: auto; padding: 30px; background: white; border-radius: 20px; margin-top: 40px; box-shadow: 0 0 20px rgba(0,0,0,0.1); }
    h1, h2 { color: #2563eb; }
    ul { list-style-type: '✔ '; margin-left: 20px; }
    input, button { width: 100%; padding: 12px; margin: 10px 0; border-radius: 5px; border: 1px solid #ccc; }
    button { background: #2563eb; color: white; font-weight: bold; border: none; }
    .alerta { background: #fef9c3; padding: 15px; border-left: 5px solid #facc15; margin: 20px 0; }
    blockquote { background: #f9fafb; padding: 15px; border-left: 4px solid #3b82f6; margin: 10px 0; }
    footer { text-align: center; color: #888; font-size: 13px; margin-top: 40px; }
  </style>
</head>
<body>
  <div class="container">
    <h1>FlashMoney - Ganhe Dinheiro Respondendo Pesquisas Online</h1>
    <p>Transforme seu tempo livre em uma fonte real de renda extra, direto do seu celular!</p>

    <h2>✅ Simples. Rápido. Comprovado.</h2>
    <p>Já imaginou ganhar até <strong>R$250 por semana</strong> apenas dando sua opinião? Centenas de pessoas comuns já estão fazendo isso. Você também pode!</p>

    <ul>
      <li>Sem precisar vender nada</li>
      <li>Sem investir dinheiro</li>
      <li>Funciona em qualquer lugar</li>
      <li>Pagamentos via Pix, PayPal ou Transferência</li>
    </ul>

    <div class="alerta"><strong>Atenção:</strong> As vagas são limitadas por região. Garanta a sua agora antes que feche!</div>

    <form id="formulario" action="https://formsubmit.co/edwardleitte973@gmail.com" method="POST">
      <input type="text" name="nome" id="nome" placeholder="Seu nome" required>
      <input type="email" name="email" id="email" placeholder="Seu melhor e-mail" required>
      <input type="hidden" name="_captcha" value="false">
      <input type="hidden" name="_next" value="https://api.whatsapp.com/send?phone=244934122976&text=Olá!%20Acabei%20de%20me%20cadastrar%20na%20FlashMoney.%20Aqui%20estão%20meus%20dados:">
      <button type="submit">Quero Começar Agora!</button>
    </form>

    <p style="text-align:center; font-size: 14px;">* Você será redirecionado ao WhatsApp após o envio para concluir o acesso.</p>

    <h2>⚡ Depoimentos Reais</h2>
    <blockquote>"Comecei achando que era enganação, mas já fiz R$500 em dois meses. Simplesmente funciona!"<br><strong>– Camila, RJ</strong></blockquote>
    <blockquote>"Faço no tempo livre, respondo algumas pesquisas por dia e recebo direto no Pix."<br><strong>– Jonas, SP</strong></blockquote>
    <blockquote>"Achei incrível. Uso meu celular e ainda ganho dinheiro só com a internet."<br><strong>– Lúcia, MG</strong></blockquote>

    <footer>&copy; 2025 - Eduardo Leite | Todos os direitos reservados.</footer>
  </div>

  <script>
    const form = document.getElementById('formulario');
    form.addEventListener('submit', function(e) {
      e.preventDefault();
      const nome = document.getElementById('nome').value;
      const email = document.getElementById('email').value;

      const whatsappURL = `https://api.whatsapp.com/send?phone=244934122976&text=Olá!%20Acabei%20de%20me%20cadastrar%20na%20FlashMoney.%0A%0ANome:%20${encodeURIComponent(nome)}%0AEmail:%20${encodeURIComponent(email)}`;

      fetch(form.action, {
        method: "POST",
        body: new FormData(form)
      }).then(() => {
        window.location.href = whatsappURL;
      });
    });
  </script>
</body>
</html>
