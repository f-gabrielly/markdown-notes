# Markdown

O objetivo desse repositório é compartilhar algumas anotações que fiz enquanto estudava um pouco de Markdown e a partir disso espero que esse conteúdo seja útil para alguém que esteja estudando.

## Titulação

O Markdown possui uma estrutura de títulos semelhante ao HTML, ou seja, títulos que variam do tamanho 1 ao 6 conforme o grau de importância.

`# Titulo 1` 
`## Titulo 2`
`### Titulo 3`
`#### Titulo 4`
`##### Titulo 5`
`###### Titulo 6`

## Parágrafo

Para criar parágrafos, usa-se uma linha em branco para separar uma ou mais linhas de texto, ou seja, digitar enter 2x. 

## Ênfase

* `**Negrito**` ou `__Negrito__`
* `*Itálico*` ou `_Itálico_`
* `***NegritoEItalico***` ou `__*NegritoEItalico*__` ou `**_NegritoEItalico_**`
* `~~riscado~~`
* `>citação`

## Listas

### Lista não-ordenada:

A lista não-ordenada pode se feita com `*`, `-` ou `+`.
`* item 1`
`- item 2`
`+ item 3`

**observação:** a criação de lista igual a acima não é uma boa prática, pois tem que usar o mesmo caractere delimitador.

### Lista ordenada:

Pode escrever sequencialmente os números ou basta digitar `1.` e dar enter que já gerará a sequência automaticamente.
`1. item 1`
`2. item 2`
`3. item 3`

## Linha Horizontal

Para criar uma linha horizontal, use três ou mais asteriscos `***`, hifens `---` ou underscores `___` sozinhos em uma linha.

* `***`ou `* * *`
* `---` ou `- - -`
* `___`ou `_ _ _`

## Link

* Link com um texto: `[Texto](url)`
* Link direto: `<url>`
 
## Imagem

`![texto alternativo](caminho da imagem)`

## Tabela

Usa `|` para delimitar as colunas e hífen `-` na segunda linha para indicar que acima estão os títulos das colunas, usando novamente o `|` para delimitar colunas. Veja um exemplo abaixo:
```
Exemplo   | Valor do exemplo
---       | ---
Exemplo 1 | valor 1
Exemplo 2 | valor 2
Exemplo 3 | valor 3
```

Para especificar o tipo de alinhamento que deseja ter nas tabelas, utiliza `:` ao lado do campo horizontal de hífens `---`, na segunda linha da sua tabela. Veja abaixo:

À esquerda | Ao Centro | À direita
:--------  |:-----: | -------:
Valor      | Valor  | Valor

**Observação:** não precisa estar alinhado.

## Código

-   **Código em linha** (_inline_): adicione um acento grave `ˋ` no início e no final do código.
	<code>`puts "Hello, world!"`</code>
-   **Múltiplas linhas de código**: envolva as linhas de código com três acentos graves `ˋˋˋ` ou três tils `~~~`. É interessante que é possível especificar a linguagem de programação, dessa forma o markdown faz o highlights.

<pre>
<code>~~~java
	public class HelloWorld{
		public static void main (String[] args){
			System.out.print("Hello, world!");
	}
~~~
</code>
</pre>

<pre>
<code>
```ruby
	print "Digite seu nome: "
	nome = gets
	print "Olá, #{nome}!"
```
</code>
</pre>

## HTML

Muitas aplicações Markdown permite que você use tags HTML em texto formatado em Markdown. Isso é útil se você preferir determinadas tags HTML à sintaxe Markdown. Por exemplo, algumas pessoas acham mais fácil usar tags HTML para imagens. Usar HTML também é útil quando você precisa alterar os atributos de um elemento, como especificar a cor do texto ou alterar a largura de uma imagem.
