# Desenvolvimento Web (Citi)

<table>
    <tr><th>sites</th><tr>
    <tr><td>www.codeacademy.com</td></tr>
    <tr><td>www.w3schools.com (tags)</td></tr>
    <tr><td>leapforce.com - emprego: avalia páginas</td></tr>
</table>



O desenvolvimento web é baseado no conceito MVC (Qual o programa é dividido em três camadas de desenvolvimento):

- Modelo (Ex: Banco de Dados)
- Visão (Ex: A linguagem que formata o modelo)
- Controle (Ex: A linguagem que altera o modelo)

No desenvolvimento Web funciona assim:

Comportamento - JavaScript
Formatação - CSS
Informação - HTML

HTML - É uma linguagem de descrição

- Baseada em Tags
    sintaxe: 
    ```html
    <tag>...</tag>
    ```
- Atributos: 
```html
<tag atributo1="...">...</tag>
```
(Algo que a tag contém)

- HTML é universal para navegadores
*Obs: O internet Explore não entende algumas tegs de CSS.

- DOCTYPE - Valida toda a documentação HTML
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd"
<html xmlns="http://www.w3.org/1999/xhtml"xml:lang="en">
<head>
    <meta http-equiv="Content-Type" content="text/html;charset=UTF-8"/>
    <title>Desenvolvimento Web Client-side</title>
</head>
```

Boas práticas de programação: Deve identar (Não obrigatório para não perder)

```html
<html><!--tag principal: abre e fecha o programa-->
    <!--meta: informações que não são visíveis ao usuário-->    
    <head>
        <title>Minha Primeira Página HTML!!!</title><!--titulo-->
    </head>
    <!--body: tudo que vai aparecer para o usuário-->
    <body>
        <p>Essa é a primeira página HTML!!!</p><!--parágrafo-->
        <!--acéntos: caracteres especiais para a codificação UTF-8(sem bom)&a grave (não usado na prática)-->
    </body>
</html>
```

OBS: Em alguns nagegadores são formatados para aceitar a lingua sem acento (Ingles)
formate no notepad++ (UTF-8)(codificação)

## Principais tags

```html
<meta name="Description" content="Conteúdo da Página"><!-- Descrição da página: Inportante para página de buscas -->
<meta name="kayWords" content="palavra-chave da página">
<!--- Plavra chave da página (rankeada em sites de busca)-->
```

### tags body

```html
- <p></p><!--parágrafo-->
- <br/><!--Quebra de linhas-->
- <hr/><!--Quebra a linha e adiciona uma linha-->
- <h1><!--tamanho da fonte pode variar 1 (maior)... 7(menor)...-->
- <i><!--  Itálico-->
- <b><!-- negrito-->
- <u><!-- sublinhado-->
```

### Imagem tag - (Adicionar uma imagem)

```html
<img src="..." alt="...">
<!--alt - para aparecer um texto ao invés do ícone corrompido, caso a imagem não apareça-->
```

jpg - Não aceita fundo transparente (funciona melhor com imagens com tons contínuos de cores)

gif - Aceita fundo transparente

### Link tag - (Adiciona um Link)

```html
<a href="link para alguma página" target="_blank" title="texto que aparece na caixa amarela quando passa o mouse">Nome do Link</a>
<!--Target: Para abrir uma nova aba-->
```

### Listas Ordenadas

- numerada
```html
<ol>
    <li></li>
    <li></li>
</ol>
```

### Listas não Ordenadas

- pontos
```html
<ul>
    <li></li>
    <li></li>
</ul>
```
### Tabelas

```html
<table></table>

<th></th>(titulo)

<tfoot></tfoot> <tbody></tbody> <thead></thead>

<tr></tr>(linhas)

<td></td>(colunas)
```

### Formulário

Form
```html
<form method="GET" action="#"><!--action="#" - chama na página -->
    <fieldset>
        <legend>formulário de teste</legend>
        <label for="campo-nome">Nome</label>
        <input type="text">
        <input type="submit" value="cadastrar"/>
        <input type="reset" value="limpar campos">
    </fieldset>
</form>
```

GET -> Passa os dados para URL

POST -> Não passa os dados para URL. É mais lenta mas é mais segura

```html
<fieldset>
    <legend>testando os inputs</legend>
    <label for="campo-senha">senha</label>
    <input type="password" name="senha" id="campo-senha"/>
    <label for="campo-teste1">Teste 1</label>
    <input type="radio" name="teste" id="campo-teste1" value="teste1"/>
    <label for="campo-teste2">teste 2</label>
    <input type="radio" name="teste" id="campo-teste2" value="teste2"/>

    <br><br>

    <label for="campo-check">Checkbox</label>
    <input type="checkbox" nome="checando" id="campo-check" value="checando"/>
    <label for="campo-texto">Area</label>
    <textarea name="senha" id="campo-texto" rows="20" cols="30">qualquer coisa</textarea>

    <br><br>

    <table for="campo-select">Seletor Grego</label>
    <select id="campo-select" name="seltor">
        <option value="1">Alpha</option>
        <option value="2">Beta</option>
    </select>
</fieldset>
    <input type="submit" value="cadastrar"/>
    <input type="reset" value="limpar campos"/>
</form>

```

### Frameset

Frameset é usado para dividir a tela em páginas independentes.

```html
<frameset row="50%","*,*"><!--row - linha--><!--*,* - dividir no mesmo tamanho -->
<!--caso não suporte o frameset-->
<noframeset>
    <body>
        Desculpe seu navegador não suporta
    </body>
</noframeset>
```

```html
<frameset cols="*,*"><!--cols - colunas -->
```

Frame - referencia outra página html
```html
<iframe></iframe>
```

```html

<iframe src="https://www.w3schools.com" title="W3Schools Free Online Web Tutorials">
</iframe>
<!--src - referencia outra página pelo endereço-->

```

### Fazer um mapa de links

```html
<img src="imagens/nuvem2.jpg" usemap="#meumapa">
<map name="meumapa">
    <area shape cord="" href="link" target="_blank">
</map>
<address>
    Cin-UFPE<br>
    Av. Jorn. Aníbal Fernandes<br>
    s/n - Cidade Universitária<br>
    Recife - PE, 50740-560
<address>
```

=================================

# CSS (Folhas de estilos em cascatas)

### Seletores e Propriedades

```html
<style type="text/css">
    p{
    background-color:green;
    color:red;
}
</style>

```


```css
#RRGGBB(Hexadecimal)
rgb(255,255,255)

```

- Lorem Ipsum - testo que os desingers usam para formatar páginas

- (site) - Color Blander (seleciona cores que conbinam)

- (site) - Color Picker (Pega qualquer cor da tela)


Não é aconselhavel escrever o código CSS junto com o código HTML.

-  Você deve resferenciar um arquivo CSS no código HTML até porque um código HTML pode ter várias formatações CSS.

```html
<link rel="stylesheet" href="style.css" type="text/css">
```

Agora você deve colocar os pedaços de código HTML entre 
```html
<div></div>
```

### Comentários CSS

Antes de escrever qualquer código CSS você precisa dá o reset no CSS. Isso é para corrigir alguns bugs do HTML e CSS.

```css
/*Resolve o bug da margem */

*{
    margin: 0;
    padding: 0;
    list-style:none;
    vertical-align: boaseline;
}

/*Resolve o bug do float*/

.clearfix:after{
    visibility: hidden;
    display: block;
    font-size: 0;
    content: "";
    clear: both;
    height: 0;
}

*html .clearfix {zoom: 1;}/*IE6*/
*:firt-child + html .clearfix {zoom:1;} /*IE7*/

```

## Regra de Hierarquia

Na linha de programação quem estiver em baixo sobrepõe.

### Seletores

```
* -> tudo

tag -> Seletor de tags Ex: p div

# -> seletores de id            id - algo exclusivo

. -> expecifica a classe        class - não exclusivo

E F -> Qualquer nível de hierarquia

E>F -> Imediatamente dentro

E + F -> Depois

E[att=val]

```

#### Seletores específicos para link

```
#linkteste:link -> ainda não foi visitado

#linkteste:visited -> já foi visitado

#linkteste:actived -> se já ativado

#linkteste:hoveu{

}
```

#### Adicionar fonte

Só tem essa propriedade no CSS3
```css

@font-face{
    font-family:DroidSans
    src:url("fonts/BrunbollFet.ttf");
}

.pd{
    font-family: Arial;
    font-size: 150%;
    font-style: italic;
    font-weight: bold;
}

/* text-decoration: underline;
   text-transform: copitalize;
*/
```

What the font (site) - MyFont ou GoogleFonts, você joga a imagem da fonte e ele diz mais ou menos a fonte que você quer

##### Seletores especiais para fontes

```css
:first-line{

}

:first-letter{
    font-size: 200%;
}

list-style-image
list-style-position
list-style-type
```

margem - é o que fica fora da div

padding - é o deslocamento do próprio conteúdo da div

### Border

```css

border-style:|none|dotted|dashed|solid|double|grove(uma borda com degradê)|ridge|inset|outset

border-with

border-color
```

## Posicionamento:

width:
height

Posicinamento absoluto

Posicionamento relativo (É recomendado usar o posicionamento relativo)

Para centralizar uma div na tela: você pode fazer uma pequena gambiarra, usa a margem relativa.

1: Centralizar
    left: 50%;

voltar a margem negativa 50% do comprimento do elemento

Profundidade
    z-index

    (modal e visibility hidden (carrossel)) Jquery

Cursor: (altera a imagem da seta do mouse que fica encima de um conteúdo)

Float(Controla o empilhamento da div)
    display: linear ou block
    float: left, right          obs: (não tem align)
    shadow: Sombra

OBS: O site bootstrap tem vários códigos prémoldados em JQuery para construir um site

```
hospedagem do site
servidor do dialhost 
amazon - servidor em branco
deve cobrar ao cliente uma mensalidade para manutenção (Hospedagem no servidor)
```