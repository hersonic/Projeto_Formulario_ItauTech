# Desafio Individual – Formulário Pessoal
| **Autor: Herick Portugal Bomtorin**                          |
| :----------------------------------------------------------- |
| **Idade:** 39 anos                                               |
| **Tipo de deficiência:** Deficiente auditivo bilateral profunda  |
| **CID:** H90.5                                                   |
| **Objetivo:** Desenvolver um formulário de cadastro dos clientes a fim de facilitar de validações e expressão regulares. |

## Ferramenta

-  Visual Studio Code no Windows.

## LINGUAGENS

- HTML
- CSS
- JavaScript

### HTML

#### Início

Temos uma declaração chamada `!DOCTYPE HTML`, que serve para informar os navegadores sobre o tipo de documento.

Temos um elemento `html`, que é uma raiz de um documento HTML, com um atributo `lang` que declara o nosso idioma para a língua da site para ser detectada nos mecanismos de busca e pelos navegadores. 

Então prosseguimos para o elemento `head` que declara os metadados para definir e informar aos navegadores

#### `meta`

- **`meta charset="UTF-8`**: um elemento para a codificação e a renderização de caracteres para o documento HTML;
- **`meta http-equiv="X-UA-Compatible" content="IE=edge`**: um elemento para fornecimento de HTTP para o conteúdo do navegador;
- **`meta name="viewport" content="width=device-width, initial-scale=1.0"`**: um elemento para renderizar o site todos os dispositivos

**title** Dados Pessoais-ItauTech **title**  O **title** é um elemento que renderiza o título para a aba do navegador.

#### `body`

O elemento `body` renderiza e estiliza todo o corpo de um document.

Dentro do `body`, temos uma divisão contendo uma classe chamada `box` que agrupa uma caixa.

Então nessa divisão, temos um elemento `fidelset`, que define uma bordura e um contorno do grupo.

#### `form`

O `form` é um elemento de formulário para preencher os campos. Nele, temos atributos:`

- `action` serve para encaminhar a página ao enviar;
- `method` pega os dados para postá-los no resultado ao enviar;
- `onsubmit` é um evento em JavaScript;

Dentro do `form`, encontramos:

- `legend`: uma legenda do grupo;
- `img`: uma imagem renderizada no documento HTML
  - `alt`: uma alternativa, aso a imagem não carregue, e é uma das regras mais importantes de acessibilidade;
  - `src`: um link de uma imagem externa;
- `b` torna o texto em negrito;
- `br` quebra o elemento em uma nova linha.`

Temos uma divisão com uma classe `inputBox` para agrupar um campo e um rótulo a fim de superar os limites. Nele, temos:

- `input`: um campo de entrada;
  - `type`: um tipo de campo;
  - `name`: um nome do campo;
  - `id`: um identificador do campo;
  - `required`: obrigatório;
  - `onblur`: um evento em JavaScript;
  - `value`: um valor do campo.

- `label`: um rótulo;
  - `for`: uma vinculação do `id` do `input`.

- `select`: uma lista suspensa
  - `option`: uma opção ou uma escolha ou uma alternativa
    - `value`: um valor da opção para o método `get` ou `post`

### JavaScript

Temos uma função chamada `valida()`, dentro da qual, temos um alerta, caso todos os campos sejam preenchidos. 

Já temos outra função `verificaCPF` que é uma verificador de validação de CPF:`

O `var c = s.substr(0,9)` é um método legdo de *string* que é usado para extrair uma *substring* de uma *string*, dada uma posição inicial e um comprimento. Uma `*substring* de primeiros 9 números de CPF.

O `var dv = s.substr(9,2)` extrai primeiros 9 números e últimos 2 do CPF.

```js
for (i = 0; i < 9; i++)
{
    d1 += c.charAt(i)*(10-i);
}
```

Conta 9 números num *loop* para acrescentar os caracteres.

```js
if (d1 == 0)
{
    alert("CPF Inválido")
    v = true;
    return false;
}
```

Checamos se for zero ou vazio, avisamos com um alerta.

```js
d1 = 11 - (d1 % 11);
if (d1 > 9) d1 = 0;
if (dv.charAt(0) != d1){
    alert("CPF Inválido")
    v = true;
    return false;
}
```

Renderizamos e contamos o número de CPF, checamos se for que 9 números e se não é igual, informamos que é um CPF válido.

```js
d1 *= 2;
for (i = 0; i < 9; i++){
    d1 += c.charAt(i)*(11-i);
}
```

Caso tenha um hífen, contamos os números e multiplicamos, então mandamos para a próxima:

```js
d1 = 11 - (d1 % 11);
if (d1 > 9) d1 = 0;
if (dv.charAt(1) != d1){
    alert("CPF Inválido")
    v = true;
    return false;
}
if (!v) {
    alert("CPF Válido")
}
```

Então se checamos o número `1` não é igual à variável contada e multiplicada, informamos que é um CPF inválido. Senão validamos. 

## Referências

### HTML

- [O uso de `HTML` no site](https://www.w3schools.com/html/default.asp)