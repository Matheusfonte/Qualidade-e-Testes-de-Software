20.03.26

# Plano de Testes e Relatório de Análise

Nesta aula foi abordado o conceito de **Plano de Testes**, sua importância dentro do processo de qualidade de software e a aplicação prática em sala, utilizando **planilhas para organização e detalhamento dos testes**.

---

# O que é um Plano de Testes?

O Plano de Testes é um documento que define **como os testes serão realizados em um sistema**.

Ele descreve:

- O que será testado
- Como será testado
- Quais critérios serão utilizados
- Quem será responsável pelos testes
- Quais ferramentas serão usadas

O objetivo é garantir que os testes sejam feitos de forma **organizada, padronizada e eficiente**.

---

# Syllabus vs Prática em Sala

### 📘 Syllabus (Teoria)

No modelo teórico, o Plano de Testes normalmente contém:

- Objetivo do teste
- Escopo (o que será e não será testado)
- Estratégia de testes
- Tipos de teste (funcional, desempenho, etc.)
- Ambiente de testes
- Critérios de entrada e saída
- Cronograma
- Riscos

---

### 🧪 Aplicação em Sala (Prática)

Na prática realizada em sala, o foco foi simplificar e aplicar o conceito utilizando **planilhas**, contendo:

- Cenários de teste
- Dados de entrada
- Resultado esperado
- Resultado obtido
- Status do teste (Aprovado/Reprovado)

Essa abordagem facilita a visualização e execução dos testes no dia a dia.

---

# Estrutura da Planilha de Testes

A planilha criada segue um padrão simples e eficiente para controle dos testes.

### Campos utilizados:

- **ID do Teste:** identificador único
- **Cenário de Teste:** descrição do que será testado
- **Passos:** ações realizadas no teste
- **Dados de Entrada:** valores utilizados
- **Resultado Esperado:** comportamento esperado do sistema
- **Resultado Obtido:** comportamento real após execução
- **Status:** Aprovado ou Reprovado

---

# Exemplo de Caso de Teste

| ID | Cenário | Passos | Dados de Entrada | Resultado Esperado | Resultado Obtido | Status |
|----|--------|--------|-----------------|--------------------|------------------|--------|
| 01 | Soma de números positivos | Executar função somar | 10 e 20 | Retornar 30 | Retornou 30 | Aprovado |
| 02 | Soma com número negativo | Executar função somar | -5 e 15 | Retornar 10 | Retornou 10 | Aprovado |
| 03 | Soma com valores inválidos | Executar função somar | "abc" e 10 | Exibir erro | Exibiu erro | Aprovado |

---

# Relatório de Análise de Testes

Após a execução dos testes, é importante gerar um relatório contendo:

- Quantidade de testes executados
- Quantidade de testes aprovados
- Quantidade de testes reprovados
- Principais erros encontrados
- Possíveis melhorias no sistema

---

# Exemplo de Análise

- Total de testes: 10  
- Aprovados: 8  
- Reprovados: 2  

### Problemas identificados:

- Sistema não valida corretamente entradas de texto
- Falta de tratamento para valores nulos

### Melhorias sugeridas:

- Implementar validação de dados
- Criar mensagens de erro mais claras
- Adicionar testes automatizados

---

# Conclusão

O Plano de Testes é essencial para garantir a qualidade do software, permitindo:

- Organização dos testes
- Melhor controle dos resultados
- Identificação rápida de falhas

A utilização de planilhas torna o processo mais simples e acessível, principalmente em projetos iniciais ou acadêmicos.