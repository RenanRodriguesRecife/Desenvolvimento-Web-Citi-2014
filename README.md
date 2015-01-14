# Desenvolvimento Web (Citi)

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

Principais tags

```html
<meta name="Description" content="Conteúdo da Página"><!-- Descrição da página: Inportante para página de buscas -->

```