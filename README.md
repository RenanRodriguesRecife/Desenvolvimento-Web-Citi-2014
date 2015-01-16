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