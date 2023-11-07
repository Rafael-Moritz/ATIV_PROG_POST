# ATIV_PROG_POST

## Função Lambda
![aws00](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/af5510ec-d23e-4004-b40c-6c975f24af0c)


## Como Usar
Passo 1: Acesse o Console de Gerenciamento da AWS e vá para o serviço Lambda.

Passo 2: Clique em "Criar função" e selecione a opção "Autor do zero" para começar com uma função em branco.

Passo 3: Dê um nome para a função, selecione a linguagem de programação desejada (por exemplo, Python) e clique em "Criar função".

Passo 4: Na página de configuração da função, você verá um editor de código. Substitua o código da imagem.

Passo 5: Clique em adicionar gatilho e clique em API Gateway

Passo 6: Escolha requisição REST e Open.

## End Point

https://pdfcgbkem3.execute-api.us-east-1.amazonaws.com/default/Post_func

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

### senha errada
<pre>
{
  "body": "{\"name\": \"Afonso\", \"age\": 22, \"city\": \"SP\", \"password\": \"renato\"}"
}
</pre>

![aws04](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/cd1ba4d3-c922-41cd-ace7-7885af4b0dfd)
