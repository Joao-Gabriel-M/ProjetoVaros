# ProjetoVaros

Dashboard com cotações e notícias sobre três empresas

Com o objetivo de criar um dashboard similar ao presente no link:"http://18.208.84.221/", foi construído um código em Python para coletar informações e cotações financeiras sobre três empresas. 

As três empresas são: 

- Petrobras, que possui ticker de ações (código da bolsa de valores) formado por PETR4 e consigo realizar pesquisas no site de notícias com o nome da empresa
- Weg, que possui ticker WEGE3.SA e consigo realizar pesquisas no site de notícias com o nome da empresa
- C&A, que possui ticker CEAB3.SA e consigo realizar pesquisas no site de notícias com "c%26a".

Primeiramente, foi reunído todas essas informações de nome da empresa, ticker da bolsa de valores e nome para pesquisa no site de notítias Brazil Journal na variável companies. 

A seguir, o tempo de 1 (um) ano foi definido para a coleta de cotações financeiras dessas três empresas, similar ao que consta no Dashboard modelo. 

As cotações financeiras foram reunidas através da plataforma Yahoo Finance, utilizando a biblioteca python yfinance que pode estar com o apelido ao longo do código de yf.

Dessas informações do Yahoo Finance, apenas os valores de "Open", "High", "Low" e "Close", além da data foram importados, como é apresentado também pelo dashboard modelo. 

O site para a coleta de notícias foi o "https://braziljournal.com/" e foi utilizado o BeautifulSoup para coletar as informações de Tag de categoria das notícias, título das notícias (manchetes) e o link das mesmas, que levasse a uma outra página.

Foi utilizada o framework do Dash para a criação do Dashboard e funcionalidade de um botão dropdown para a escolha das empresas.

O gráfico foi similar ao utilizado no modelo, conhecido como gráfico candlestick. 

