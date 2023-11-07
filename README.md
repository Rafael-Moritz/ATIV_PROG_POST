# ATIV_PROG_POST

## Função Lambda
![aws0](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/b00a4a46-0f13-4577-82a1-b841a80f81a5)

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
    "body": "{\"name\": \"Afonso\", \"age\": 22, \"city\": \"SP\"}"
}
</pre>

![aws1](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/fefaf2e8-9e35-466b-a3ec-2489ca25c235)

### JSON inválido
<pre>
{
    "body": "Isso não é um JSON"
}
</pre>

![aws2](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/e0d6da02-e5bf-4f93-acc2-a2dc60a15556)

### string no lugar de um int
<pre>
{
    "body": "{\"name\": \"Afonso\", \"age\": vinte e dois, \"city\": \"SP\"}"
}
</pre>

![aws3](https://github.com/Rafael-Moritz/ATIV_PROG_POST/assets/99282359/8bfb238f-23c6-4cbf-82fd-c39fcdda939b)
