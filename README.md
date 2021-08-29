# Desafio Individual – Formulário Pessoal
| Autor: Herick Portugal Bomtorin                              |
| ------------------------------------------------------------ |
| Idade: 39 anos                                               |
| Tipo de deficiência: Deficiente auditivo bilateral profunda  |
| CID: H90.5                                                   |
| Objetivo: Desenvolver um formulário de cadastro dos clientes a fim de facilitar de validações e expressão regulares. |

# `Ferramenta`:
- Visual Studio Code no Windows.


# `Linguagens`:

- HTML
- CSS
- JavaScript

# `HTML`

No ínício, começa com <!DOCTYPE HTML>, uma declaração para avisar aos navegadores que é um documento HTML, e dentro, tem <html> representa a raiz de um documento HTML e contém um atributo "lang" para declarar o idioma da página da web a fim de ajudar os mecanismos de busca e os navegadores.

Dentro desse elemento, tem um elemento <head> designado para informar os metadados e buscar os recursos. Está entre <html> e <body>.

Metadados
O <link> é um elemento que conecta os recursos externos aos documentos atuais para renderizar as coisas. Em seguida, os atributos:

O atributo "rel" é um relacionamento de tipo de arquivo;
O atributo "type" é um tipo de arquivo;
O atributo "media" especifica quais os dispositivos o documento deve ser renderizado.

"<meta charset="UTF-8">": É um elemento de metadado para a codificação e a renderização de caracteres para o documento HTML

"<meta http-equiv="X-UA-Compatible" content="IE=edge">": É um elemento de metadado de fornecimento de HTTP para o conteúdo do navegador

"<meta name="viewport" content="width=device-width, initial-scale=1.0">": É um elemento de metadado para renderizar a compatiblidade de visualizacão da página com todos os dispositivos

"<title>Dados Pessoais-ItauTech</title>: O <title>" é um elemento que renderiza o título para a aba do navegador.


# <h1>Corpo</h1>
O elemento <body> renderiza todo o corpo de um document.

No corpo, vocês encontram os elementos que são divisões ou uma seções num documento HTML. O atributo "class" é um nome de classe para um elemento para pegar os seletores de um arquivo CSS.
Além disso, numa divisão, temos:

- h1 é um cabeçalho de primeiro grau.

- h2 é um cabeçalho de segundo grau.

- p é uma definição de parágrafos.

- hr é um mais frequentemente exibido como uma regra horizontal que é usada para separar conteúdo (ou definir uma alteração) numa página HTML.

  <h1>Formulário</h1>

- O form é um elemento de criação de formulário usado para onde o usuário possa preencher os campos. Nele, tem um atributo "onsumbit" é um evento de submissão em JavaScript que executa a função. Dentro do formulário, definimos as classes grupo-de-caixa para agrupar o rótulo e o campo para uma mesma linha e expandir a largura do campo até à largura da classe "descricao".


Temos neles:

<h2>Rótulos<h2>

- O <label> é um elemento que rotula a informação.
- O atributo "for" é um método que pega o identificador do campo de entrada.
- Campos de entrada
- O "<input> " é um elemento de campo de entrada para o usuário escrever o valor e preenchê-lo.

- O atributo "id" é uma vinculação do campo ao rótulo.
- O atributo "required" significa que o campo não pode ser vazio.
- O atributo "maxlength" define o limite de caracteres.
- O atributo "placeholder" é um valor da dica ou do exemplo.
- O atributo "pattern" é um método de expressão regular.

<h3>Validações e botão submit</h3>

O comando <input type="submit" name="submit" id="submit" value="Enviar"> é um botão de submissão com um valor para renderizar

O comando <script type="text/javascript" src="funcoes_CPF.js"></script> é elemento para anexar o arquivo externo em JavaScript e define o tipo de documento

# JavaScript
Executamos uma função (function) chamada validarCPF(), que foi executada ao clicar o botão em HTML. Dentro de uma função, usamos de variáveis para pegar o CPF por meio de um identificador do campo de entrada. Então ao obter o valor, analisamos 3 casos:

Checamos se for if (d1 == 0), avisamos (alert) que o CPF deve ter CPF inválidos.

No segundo caso, checamos o if (d1 > 9) d1 = 0, avisamos o retorno como CPF inválidos.

No ultimo caso de checagem a qual retornou de aviso de alerta que teve CPF válido ao digitar dado correto.

Outro caso sobre o botão "enviar":

Criamos uma alerta de aviso que os dados foram enviados. Em caso for incompleto já temos configuração em HTML que exibe dados obrigatórios.


# Referências
<h3>HTML</h3>

- O uso de no site https://www.w3schools.com/html/default.asp
- O uso de expressão regular de números permitidos (maxleght).
- JavaScript
- A expressão regular de CPF e ENVIAR.
- CSS