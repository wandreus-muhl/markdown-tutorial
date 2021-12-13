# Tutorial Markdown

Desenvolvida por John Gruber e Aaron Swartz, é uma linguagem de marcação, assim como o HTML. Muito utilizada para a formatação de documentos de texto na web, a linguagem utiliza-se de caracteres especiais para reallizar a marcação das "_tags_"

Na lista não ordenada abaixo - definida com o caractere ``*``, estão listados alguns dos comandos da linguagem:

* Títulos: os títulos de um documento .md equivalem a tag h(número de hashtags) do HTML. Eles são definidos com o caractere ``#``
    - # Título 1 - ``<h1>``
    - ## Título 2 - ``<h2>``
    - ### Título 3 - ``<h3>``
    - #### Título 4 - ``<h4>``
    - ##### Título 5 - ``<h5>``
    - ###### Título 6 - ``<h6>``

* Ênfase: para destacar um trecho do texto, utiliza-se os caracteres ``*`` ou ``_``:
    - **Negrito** - definido com a utilização de dois caracteres (``__`` ou ``**``) no início e no final da parte que será destacada.
    - *Itálico* - definido com a utilização de apenas um caractere (``_`` ou ``*``) no início e no final do trecho que será enfatizado

* *Links*: para inserir *links* no documento, utiliza-se um texto-âncora (``[]()``). Entre as chaves, informa-se o texto que aparecerá no documento compilado, já nos parênteses, coloca-se o endereço de destino do *link* 

* Citações: essa *tag* transforma o texto em uma citação, semelhante a tag ``<blockquote>`` do HTML. Para definir a citação, utiliza-se o caractere `>`: 
    > Vivamus neque risus, congue non auctor eget, interdum a velit. Cras facilisis sapien nec mi ultrices finibus. Curabitur ut laoreet metus. Vivamus malesuada felis venenatis massa dictum mattis.

* Códigos: transforma o texto em um trecho de código. Para isso, usa-se o caractere `` ` ``. Existem duas formas de definir trechos de código:
    - Inline: utiliza-se dois caracteres `` ` `` no início e final do trecho 
        > Para instalar as dependências dessa aplicação execute ``npm install``
    - Bloco: para definir um bloco de código, utiliza-se três caracteres `` ` `` ou `` ~ `` no início e final do bloco. Também é possível definir a linguagem em que o trecho será escrito, basta adicionar o nome da linguagem depois de abrir o bloco de código com `` ` `` ou `` ~ ``
     ~~~javascript
        const express = require('express')

        const app = express()
        app.use(express.json())

        app.use(express.urlencoded({
        extended: true
        }))
    ~~~

* Tabelas: para definir tabelas em Markdown, usa-se o caractere ``|`` para delimitar as colunas, após isso, utiliza-se o ``-`` para indicar que acima está o título das colunas, e abaixo o conteúdo das mesmas
 Exemplo | Valor 
 --- | ---
 A | 1 
 B | 2 
 C | 3 