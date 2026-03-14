13.03.26

# Qualidade e Teste de Software

Este repositório contém um resumo dos principais conceitos vistos na aula sobre **testes de software**, incluindo **princípios, níveis, tipos e técnicas de teste**, com exemplos simples para facilitar o entendimento.

---

# Princípios de Teste

Os princípios de teste ajudam a garantir que os testes sejam feitos de forma eficiente e organizada.

### Exemplos de princípios

- **Testes ajudam a encontrar defeitos**  
  O objetivo do teste é identificar problemas no sistema.

- **Não é possível testar tudo**  
  Como sistemas podem ser muito grandes, é necessário priorizar testes.

- **Testes devem começar cedo**  
  Quanto antes os testes começarem no desenvolvimento, menor o custo para corrigir erros.

**Exemplo:**  
Testar o login do sistema ainda na fase inicial do desenvolvimento.

---

# Níveis de Teste

Os níveis de teste indicam **em qual parte do sistema o teste está sendo realizado**.

### 1. Teste de Unidade (Componente)
Testa pequenas partes do sistema, como funções ou métodos.

**Exemplo:**  
Testar uma função que calcula a soma de dois números.

---

### 2. Teste de Integração
Verifica se diferentes partes do sistema funcionam corretamente juntas.

**Exemplo:**  
Testar se o sistema de cadastro envia corretamente os dados para o banco de dados.

---

### 3. Teste de Sistema
Testa o sistema completo funcionando como um todo.

**Exemplo:**  
Cadastrar um usuário, fazer login e acessar o sistema.

---

### 4. Teste de Aceite
Valida se o sistema atende às necessidades do usuário ou do cliente.

**Exemplo:**  
Usuários testando o sistema para verificar se o cadastro e login funcionam corretamente.

---

# Tipos de Teste

Os tipos de teste definem **o que será avaliado no sistema**.

### Teste Funcional
Verifica se as funcionalidades do sistema funcionam corretamente.

**Exemplo:**  
Verificar se o botão de login realmente permite acessar o sistema.

---

### Teste Não Funcional
Avalia características como desempenho, segurança e usabilidade.

**Exemplo:**  
Testar se o sistema suporta muitos usuários acessando ao mesmo tempo.

---

### Teste Caixa-Branca
Analisa o código interno do sistema.

**Exemplo:**  
Verificar se todas as condições `if` de uma função foram executadas.

---

### Teste Relacionado à Mudança
Executado quando algo é alterado no sistema.

**Exemplo:**  
Após alterar o sistema de login, testar novamente para garantir que nada quebrou.

---

# Técnicas de Teste

As técnicas ajudam a **definir como os testes serão feitos**.

### Caixa-Preta
Testa o sistema sem olhar o código, apenas entradas e saídas.

**Exemplo:**  
Inserir usuário e senha no login e verificar se o acesso funciona.

---

### Caixa-Branca
Testa a lógica interna do código.

**Exemplo:**  
Garantir que todas as linhas de uma função sejam executadas durante os testes.

---

### Baseado em Experiência
Testes baseados no conhecimento e experiência do testador.

**Exemplo:**  
O testador tenta inserir dados inválidos para ver se o sistema quebra.

---

# Conclusão

Os testes de software são essenciais para garantir qualidade, confiabilidade e bom funcionamento de sistemas.  
Utilizando diferentes **princípios, níveis, tipos e técnicas**, é possível encontrar erros mais rapidamente e melhorar a experiência do usuário.