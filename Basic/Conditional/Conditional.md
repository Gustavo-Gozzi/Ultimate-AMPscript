# Conditions

[ING]

Here, you will learn how to use **If/Else** conditional structures. 

It's very simple! The basic syntax follows this blueprint:

```amp
ff [your condition] Then
    /* code to execute if TRUE */
else
    /* code to execute if FALSE */
endIf
```

Usage example:
``` html
%%[
  var @name, @greeting
  set @name = AttributeValue("Name")

  if Empty(@name) Then
    set @greeting = "Hello, Friend!"
  else
    set @greeting = Concat("Hello, ", @name, "!")
  endIf
]%%

```

[PT-BR]

Aqui, você vai aprender como utilizar estruturas condicionais com **If/Else**. 

É super simples! A sintaxe básica segue este modelo:

```amp
ff [your condition] Then
    /* code to execute if TRUE */
else
    /* code to execute if FALSE */
endIf
```

Usage example:
``` html
%%[
  var @name, @greeting
  set @name = AttributeValue("Name")

  if Empty(@name) Then
    set @greeting = "Hello, Friend!"
  else
    set @greeting = Concat("Hello, ", @name, "!")
  endIf
]%%

```
