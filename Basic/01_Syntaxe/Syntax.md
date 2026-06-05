# Syntaxe

[ING]
AMPscript runs at server-side, before the email is sent and rendered on the client. The client does not see the AMPscript logic being developed, only the HTML and CSS used.

AMPscript is inserted during the creation of the HTML and respects the execution order. Therefore, if you create the AMPscript before the HTML, it will be executed first; otherwise, if you create the AMPscript in the middle or at the end of the HTML, it will be executed according to order.

All the AMPscript logic must be developed inside these parameters: %%[ (ampscript logic) ]%% 
And we can create variables using ```var @variableName``` and define a value using ``` set @variableName = "Value"```

This value accepts Strings, Integers, and Booleans.

JSONs, Arrays, tuples, and others are not accepted.

And we use the function %%=v(@variableName)=%% direct in HTML to return variable value.

```v()``` is the function, and ```%%= =%%``` are the AMPscript callers, and the internal variable will be returned.

[PT-BR]
AMPscript roda no lado do servidor, antes do email ser enviado e renderizado para o cliente. O mesmo não vê a lógica AMPscript que foi implementada, apenas o HTML e CSS usados.

O AMPscript é inserido durante a criação do HTML e respeita ordem de execução. Isso significa que se você criar o AMPscript antes do HTML, ele será exectado primeiro, caso você crie no meio ou no final do HTML, então ele será executado de acordo.

Toda a lógica AMPscript deve ser desenolvida dentro desses parâmetros: %%[ (lógica ampscript) ]%% 
E nós podemos criar variáveis usando ```var @nomeVariavel``` e definir valores usando ```set @nomeVariavel = "valor"```

Esse valor pode ser String, Inteiro e Boleanos
Porém JSONs, Arrays, Tuplas e outras não são aceitos.

E nós usamos a função ```%%=v(@nomeVariavel)=%%``` para retornar o valor da variavel

```v()``` é a função, e ```%%= =%%``` são os chamadores do AMPscript, e a variável dentro do ```v()``` será retornada naquele local.