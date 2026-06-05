# Here are the Operators allowed in If conditions
Use the AND/OR operators to combine and make decisions rules, validations and more.
## - 
Utilize os operadores AND/OR para combinar e fazer regras de decisões, validações e mais.

Example / Exemplo:
```` html
set @age = AttributeValue("Age")
set @gender = AttributeValue("Gender)

if @age <= 15 and (@gender == 'F' OR @gender == 'M') then
    set @msg = 'Little Teen'

elseif @age >= 18 AND @gender == 'M' then
    set @msg = 'Adult'

endif


```


| Operator / Operador | What it Means / O que significa | Example / Exemplo |
| :--- | :--- | :--- |
| `==`  | Equal to (Igual a) | `If @status == "Ativo" Then` |
| `!=`  | Different (Diferente de) | `If @status != "Cancelado" Then` |
| `AND` | All conditions must be TRUE (Todas as condisções precisam ser verdadeiras) | `If @idade >= 18 AND @pais == "BR" Then` |
| `OR` | One of are conditions must be TRUE (pelo menos uma precisa ser verdadeira) | `If @plano == "Premium" OR @plano == "VIP" Then` |
| `NOT` | Negative (Inversão) | `If NOT Empty(@nome) Then` |