# Markdown

Markdown é uma linguagem simples de marcação originalmente criada por John Gruber e Aaron Swartz. Markdown converte seu texto em HTML válido. Markdown é frequentemente usado para formatar arquivos README, para escrever mensagens em fóruns de discussão online e para criar rich text usando um editor de texto simples.

<details>
<summary>Click Para ver a Imagem</summary>

![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/1200px-Markdown-mark.svg.png ':size=250')
  
</details>

## Syntax

[Markdown Syntax](https://www.markdownguide.org/basic-syntax/) é uma sintaxe usada para padronizar e facilitar formatação de texto na web. Textos estilizados com Markdown são, na maioria dos casos, apenas texto com caracteres não-alfabéticos, como `#, \* e ![]()`, usados para a configuração de títulos, listas, itálico, negrito e inserção de imagens.

## Lista de comandos em Markdown

Veja abaixo uma lista dos comandos em markdown e alguns exemplos de seu uso:

### Titulação

```markdown
# Título <h1>
## Título <h2>
### Título <h3>
#### Título <h4>
##### Título <h5>
```

### Ênfase

Este é um exemplo de um texto que possui uma ênfase em **negrito**, e outro em _itálico_.

```markdown
Este é um exemplo de um texto que possui uma ênfase em **negrito**, e outro em _itálico_.
```

### Links

Existem duas formas de inserir link em Markdown, através de um link direto ou usando um texto-âncora:

* **Texto-âncora:** utilize os caracteres `[]()` adicionando entre chaves o texto que você quer que apareça, e entre os parênteses, o endereço de destino, no formato `[exemplo](https://exemplo.com/).`

* **Link direto:** envolva o endereço da web em chaves `<>`. O endereço ficará visível e será clicável pelo usuário. O endereço em forma de link direto tem o formato `<https://exemplo.com/>`.

**Resultado:** Este é um link em formato de texto, e este é um link direto <https://www.markdownguide.org/>

### Listas de itens

Para listas não ordenadas, utilize um asterisco `*` na frente to item da lista:

```markdown
* Item 1
* Item 2
* Item 3
```

Para listas ordenadas, utilize o número do item seguido de ponto `.` :

```markdown
1. Item 1
2. Item 2
3. Item 3
```

### Imagens

O código para inserir uma imagem no conteúdo é semelhante ao código de inserir links-âncora, adicionando um ponto de exclamação `!` no início do código, como no exemplo abaixo:

`![Alt ou título da imagem](URL da imagem)`

### Citação

Para transformar um texto em uma citação ou comentário, semelhante ao código HTML `<blockquote>`, utilize o sinal `>` ou `!>` ou `?>` no início da linha que será formatada:

```markdown
>Este é um *blockquote*. O sinal usado abre e fecha este código no HTML. 
>Para adicionar mais uma linha à citação, basta teclar Enter para um novo
>código sinal. Isso gerará um novo parágrafo dentro do *blockquote*.
>Códigos de **negrito**, _itálico_ e <https://links.com> funcionam aqui.

!> Este é um *blockquote*. O sinal usado abre e fecha este código no HTML.

?> Este é um *blockquote*. O sinal usado abre e fecha este código no HTML.
```

### Código

Há dois modos de adicionar trechos de código ao Markdown:

* **Código em linha:** adicione um acento grave `ˋ` no início e no final do código.
* **Múltiplas linhas de código:** envolva as linhas de código com três acentos graves `ˋˋˋ` ou três tils `~~~`

```markdown
 Esta é uma linha que contém um ˋcódigoˋ.

ˋˋˋ
Esta é uma linha de código
 ˋˋˋ
```

Para especificar que tipo de linguagem está sendo apresentada no bloco de códigos adicionando o nome da linguagem de programação após os três acentos graves ou três tils, por exemplo:

`~~~javascript`.

```markdown
~~~javascript
Esta é uma linha de código em Javascript.
~~~

~~~php
Esta é uma linha de código em PHP.
~~~

~~~html
Esta é uma linha de código em HTML.
~~~
```

### Tabelas

Escolha os títulos das colunas e use `|` para delimitar as colunas. Depois, utilize hífen `-` na segunda linha para indicar que acima estão os títulos das colunas, usando novamente o `|` para delimitar colunas. Veja um exemplo abaixo:

```markdown
Exemplo   | Valor do exemplo |
--------- | ---------------- |  
Exemplo 1 | R$ 10            |
Exemplo 2 | R$ 8             |
Exemplo 3 | R$ 7             |
Exemplo 4 | R$ 8             |
```

Para especificar o tipo de alinhamento que deseja ter nas tabelas, utilize `:` ao lado do campo horizontal de hífens `---`, na segunda linha da sua tabela. Veja abaixo:

Alinhado a esquerda: usar `:` no lado esquerdo (alinhamento padrão);
Alinhado a direita: usar `:` no lado direito;
Centralizado: usar `:` dos dois lados.

Veja no exemplo:

```markdown
Alinhado a esquerda | Centralizado | Alinhado a direita
:---------          |  :------:    | -------:
Valor               | Valor        | Valor
```
