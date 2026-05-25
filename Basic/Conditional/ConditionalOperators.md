| Operador | O que significa | Exemplo em AMPscript |
| :--- | :--- | :--- |
| `==`  | Equal to (Igual a) | `If @status == "Ativo" Then` |
| `!=`  | Different (Diferente de) | `If @status != "Cancelado" Then` |
| `AND` | All conditions must be TRUE (Todas as condisções precisam ser verdadeiras) | `If @idade >= 18 AND @pais == "BR" Then` |
| `OR` | Once of are conditions must be true (pelo menos uma precisa ser verdadeira) | `If @plano == "Premium" OR @plano == "VIP" Then` |
| `NOT` | Negative (Inversão) | `If NOT Empty(@nome) Then` |