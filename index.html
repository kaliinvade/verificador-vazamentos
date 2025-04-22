<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Verificador de Vazamento</title>
</head>
<body>
  <h1>Verifique se seu e-mail foi vazado</h1>
  <input type="email" id="email" placeholder="Digite seu e-mail"/>
  <button onclick="checkEmail()">Verificar</button>
  <p id="result"></p>

  <script>
    async function checkEmail() {
      const email = document.getElementById('email').value;
      const resultEl = document.getElementById('result');

      resultEl.textContent = 'Verificando...';

      const encodedEmail = encodeURIComponent(email);
      const apiKey = 'SUA_API_KEY_AQUI'; // substitua pela sua chave

      try {
        const res = await fetch(`https://haveibeenpwned.com/api/v3/breachedaccount/${encodedEmail}`, {
          headers: {
            'hibp-api-key': apiKey,
            'User-Agent': 'VerificadorVazamentos'
          }
        });

        if (res.status === 404) {
          resultEl.textContent = 'Boa! Seu e-mail não foi encontrado em nenhum vazamento.';
        } else if (res.ok) {
          const data = await res.json();
          resultEl.textContent = `Ops! Seu e-mail apareceu em ${data.length} vazamento(s): ${data.map(b => b.Name).join(', ')}`;
        } else {
          resultEl.textContent = 'Erro ao consultar. Tente novamente.';
        }
      } catch (error) {
        resultEl.textContent = 'Erro na verificação: ' + error.message;
      }
    }
  </script>
</body>
</html>
