###  Documentação do JSON de Questões

#### Estrutura Geral
O JSON contém um conjunto de registros de questões de um quiz. Cada registro é identificado por uma chave (`Id`), que é um campo autonumérico, funcionando como a chave única do registro.

#### Regras Específicas

1. **Chave `Id`:**
   - Cada questão é identificada de forma única por um campo autonumérico chamado `Id`.

2. **Texto da Questão (`text`):**
   - O campo `text` armazena o enunciado da questão.
   - **Regra:** O texto da questão não pode se repetir em nenhum dos registros.

3. **Tipo de Questão (`type`):**
   - Especifica o tipo de registro, sendo fixado como `"quiz"` para identificar que o registro corresponde a uma questão de um quiz.

4. **Opções de Resposta (`options`):**
   - Cada questão pode ter uma ou várias opções de resposta, representadas em uma lista.
   - Cada opção de resposta possui os seguintes campos:
     - **Texto da Opção (`text`):** Texto que descreve a opção de resposta.
     - **Justificativa (`explanation`):** Explicação sobre por que a opção está correta ou incorreta.
     - **Correto (`correct`):** Campo booleano que indica se a opção é correta (`true`) ou não (`false`).
   - **Regra:** Cada questão pode ter uma ou mais opções marcadas como corretas.

5. **Exemplo de Estrutura de Opção:**
   - `{"text": "Texto da opção", "explanation": "Justificativa da opção", "correct": true/false}`

#### Exemplo de Questão
```json
{
  "1": {
    "type": "quiz",
    "text": "Exemplo de enunciado da questão?",
    "options": [
      {
        "text": "Opção A",
        "explanation": "Justificativa para a opção A.",
        "correct": false
      },
      {
        "text": "Opção B",
        "explanation": "Justificativa para a opção B.",
        "correct": true
      }
    ]
  }
}
```

#### Considerações Finais
- **Autenticidade dos Textos:** O texto das questões e opções deve ser único para evitar duplicações.
- **Justificativa das Opções:** Cada opção de resposta deve ser acompanhada por uma justificativa clara que explique a razão de ser correta ou incorreta.