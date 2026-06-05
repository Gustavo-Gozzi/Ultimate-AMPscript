# Get Attributes from Data Extensions

[ING]

We can get attributes directly from a Data Extension. 

In Marketing Cloud Engagement, create a Data Extension with these attributes:
- Id (Text)
- Name (Text)
- Age (Number)
- Birthday (Date)

Remember to check the **"Is Sendable?"** flag so it becomes available for email previews.

Now, you can call these attributes inside your AMPscript block using one of the following ways:

```html
%%[
  set @name = [Name]
  set @age = AttributeValue("Age")
]%%
```
Wich is the difference between [Name] and AttributeValue("Age")?

When you use `Set @name = [Name]`, you are calling the attribute directly. However, if that attribute does not exist in the sending Data Extension, you will receive a runtime error and the email will fail to render.

On the other hand, if you use `Set @age = AttributeValue("Age")`, the function will try to retrieve the attribute if it exists. If it doesn't, it safely returns an empty value, meaning no error will appear and your email will send normally.

[PT-BR]

Nós podemos pegar atributos diretamente de uma Data Extension.

No Marketing Cloud Engagement, crie uma Data Extension com os atributos:

- Id (text)
- Name (text)
- Age (number)
- birthday (date)

Lembre de ligar a flag **Is Sendable** para ficar disponíveis para pré-view de e-mails

Agora, podemos chamar atributos dentro do bloco AMPscript usando uma das seguintes formas:

```html
%%[
  set @name = [Name]
  set @age = AttributeValue("Age")
]%%
```
Qual a diferênça entre [Name] e AttributeValue("Age")?

Quando você usa `Set @name = [Name]`, está chamando o atributo diretamente. Porém, se esse atributo não existir na Data Extension de envio, você receberá um erro e o e-mail vai "quebrar" (não vai renderizar).

Por outro lado, se você usar `Set @age = AttributeValue("Age")`, a função vai tentar buscar o atributo se ele existir. Caso não exista, ela simplesmente retorna um valor vazio de forma segura, o que significa que nenhum erro vai aparecer e o seu e-mail será enviado normalmente.