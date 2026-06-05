
[ING]

## 🏆 Challenge: Sun Resorts Bar Menu Launch

Hello, AMPscript enthusiast! Hope you are doing well. 👋

To lock in what you've learned so far, here is a practical challenge to test your skills in basic concepts, variables, and conditionals.

### 🏢 Context
**Sun Resorts** is hosting an exclusive event to launch its new premium bar menu. Your mission is to create a personalized email invitation targeting only the right customers based on specific business rules.

### ⚠️ Business Rules

1. **Age Gate & Status:** Only customers who are adults (**Age greater than or equal to 18**) AND have an **"Approved"** status are eligible for the new bar menu.
2. **Composite ID:** To help the data team manage the guest list, you need to create a custom ID string composed of their `status` (in lowercase) and their `last_document_numbers`, separated by an underscore. Example: `approved_1234`.
3. **Data Cleaning:** Due to a poor CRM integration, some text data was saved with inconsistent casing (e.g., "APPROVED", "approved", "guSTaVo", "gustavo"). You must normalize these values using AMPscript before rendering the email.
4. **Conditional Messaging:**
   * **If eligible:** Display this message: 
     > *"Hello, **[Name with only the first letter capitalized]**! You are eligible for our new special menu! Feel free to visit one of our restaurants in **[Customer City]**. To access the new menu, use your invitation code: **[Custom ID]**"*
   * **If NOT eligible:** Display this message: 
     > *"Sorry, **[Name with only the first letter capitalized]**, you are not eligible for our new special menu. Stay tuned for the next season!"*

### 📊 Data Extension Setup
Create a Data Extension with the following schema:

| Attribute | Type | Primary Key |
| :--- | :--- | :--- |
| Id | Text | True |
| Name | Text | False |
| Age | Number | False |
| City | Text | False |
| Status | Text | False |
| Last_document_numbers | Text | False |

👉 **Next Step:** Download the `Sun_Resorts_Customers.csv` file from this folder, import it into your Data Extension, and write your AMPscript solution!


[PT-BR]
## 🏆 Desafio: Lançamento do Menu do Bar - Sun Resorts

Olá, entusiasta de AMPscript! Espero que esteja bem. 👋

Para fixar tudo o que aprendemos até aqui, propomos um desafio prático para testar suas habilidades com conceitos básicos, variáveis e condicionais.

### 🏢 Contexto
O **Sun Resorts** vai realizar um evento exclusivo para lançar o seu novo menu premium do bar. Sua missão é criar um e-mail personalizado para convidar apenas os clientes elegíveis, seguindo regras de negócio específicas.

### ⚠️ Regras de Negócio

1. **Restrição de Idade e Status:** Apenas clientes maiores de idade (**Idade maior ou igual a 18**) E com o status **"Approved"** (Aprovado) são elegíveis para o novo menu.
2. **ID Composto:** Para ajudar a equipe de dados, você precisa gerar um ID customizado composto pelo `status` (em letras minúsculas) e os `last_document_numbers`, separados por um underline. Exemplo: `approved_1234`.
3. **Limpeza de Dados:** Por conta de uma integração ruim com o CRM, alguns dados de texto foram salvos com letras maiúsculas e minúsculas bagunçadas (ex: "APPROVED", "approved", "GUSTAVO", "gustavo"). Você deve normalizar esses valores usando AMPscript.
4. **Mensagem Condicional:**
   * **Se for elegível:** Exiba a mensagem: 
     > *"Olá, **[Nome apenas com a primeira letra maiúscula]**! Você é elegível ao novo menu especial! Visite um dos nossos restaurentes em **[Cidade do uduário]**. Utilize o código: **[ID Customizado]**."*
   * **Se NÃO for elegível:** Exiba a mensagem: 
     > *"Sorry, **[Nome apenas com a primeira letra maiúscula]**, you are not eligible for our new special menu. Stay tuned for the next season!"*

### 📊 Estrutura da Data Extension
Crie uma Data Extension com a seguinte estrutura:

| Atributo | Tipo | Chave Primária |
| :--- | :--- | :--- |
| Id | Texto | Sim |
| Name | Texto | Não |
| Age | Number | Não |
| City | Texto | Não |
| Status | Texto | Não |
| Last_document_numbers | Texto | Não |

👉 **Próximo Passo:** Faça o download do arquivo `Sun_Resorts_Customers.csv` nesta pasta, importe-o para a sua Data Extension e desenvolva a sua solução em AMPscript!