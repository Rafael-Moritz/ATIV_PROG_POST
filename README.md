# ATIV_PROG_POST

## Função Lambda
![aws00](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/af5510ec-d23e-4004-b40c-6c975f24af0c)

## End Point

https://pdfcgbkem3.execute-api.us-east-1.amazonaws.com/default/Post_func

## Passo a passo
1- Inicie acessando o Console de Gerenciamento da AWS e navegue até o serviço Lambda.

2- Inicie o processo clicando na opção "Criar função" e selecione "Começar do zero" para criar uma nova função a partir do zero.

3- Nomeie a função, escolha a linguagem de programação desejada (por exemplo, Python) e finalize a criação da função.

4- Ao acessar a página de configuração da função, você encontrará um editor de código. Substitua o código existente com o código necessário para a sua função.

5- Agora, clique em "Adicionar gatilho" e escolha a opção "API Gateway".

6- Opte por configurar uma requisição REST e selecione a opção "Abrir".

## Testes
### Tudo em ordem

<pre>
{
  "body": "{\"name\": \"Afonso\", \"age\": 22, \"city\": \"SP\", \"password\": \"afonsinho\"}"
}
</pre>

![aws01](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/2d4e930f-765b-4a57-8e00-b68643079a9f)

### JSON inválido
<pre>
{
    "body": "Isso não é um JSON"
}
</pre>

![aws02](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/60ab7395-5b73-4ff6-8cf4-912db797272c)

### string no lugar de um int
<pre>
{
  "body": "{\"name\": \"Afonso\", \"age\": vinte e dois, \"city\": \"SP\", \"password\": \"afonsinho\"}"
}
</pre>

![aws03](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/214450fe-4b11-4be4-aefb-ec5121117d9d)

### Senha errada
<pre>
{
  "body": "{\"name\": \"Afonso\", \"age\": 22, \"city\": \"SP\", \"password\": \"renato\"}"
}
</pre>

![aws04](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/cd1ba4d3-c922-41cd-ace7-7885af4b0dfd)
