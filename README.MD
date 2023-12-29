## Projeto em NodeJS sobre Sessões e Cookies 🍪🚀

Os cookies são pequenos pedaços de dados armazenados no navegador do cliente. Aqui estão alguns pontos importantes sobre cookies:
- são excelentes para armazenar dados no cliente (navegador);
- não armazene dados sensíveis aqui, pois podem ser visualizados e manipulados.
- os cookies podem ser configurados para expirar quando o navegador é fechado (=> "Session Cookie") ou quando uma determinada idade/data de expiração é atingida ("Permanent Cookie").
- funcionam bem em conjunto com sessões.

Exemplo de uso de Cookie em Express 🍪: 
~~~javascript
const express = require('express');
const cookieParser = require('cookie-parser');

const app = express();

// Configurando o uso do cookie-parser
app.use(cookieParser());

app.get('/definir-cookie', (req, res) => {
  res.cookie('exemplo', '123');
  res.send('Cookie definido com sucesso!');
});

app.get('/
~~~
