06.03.26

# BDD - CRUD de Usuários e Login

Este documento apresenta os cenários de **BDD (Behavior Driven Development)** para um sistema web simples de gerenciamento de usuários.
O sistema possui funcionalidades de **CRUD (Create, Read, Update, Delete)** e **autenticação de usuários (Login)**.

---

# Princípios de Teste Utilizados

* **Testar funcionalidades individualmente:** cada cenário valida apenas uma operação específica.
* **Cenários claros e objetivos:** escritos de forma compreensível para desenvolvedores e analistas.
* **Independência dos testes:** cada cenário pode ser executado sem depender de outros testes.
* **Resultados consistentes:** executando nas mesmas condições, o resultado deve ser sempre o mesmo.
* **Casos positivos e negativos:** testes com dados válidos e inválidos.
* **Possibilidade de automação:** os cenários podem ser utilizados em ferramentas de automação de testes.
* **Facilidade de manutenção:** os testes são organizados de forma simples para futuras alterações.

---

# Funcionalidade: Registro de Usuário

Como administrador do sistema
Quero registrar novos usuários
Para que eles possam acessar o sistema

```gherkin
Funcionalidade: Registro de usuário

Cenário: Registro realizado com sucesso
Dado que estou na página de cadastro de usuário
Quando informo todos os campos obrigatórios corretamente
E clico no botão "Cadastrar"
Então o sistema deve exibir a mensagem "Cadastro realizado com sucesso"

Cenário: Cadastro com campos obrigatórios não preenchidos
Dado que estou na página de cadastro de usuário
Quando deixo campos obrigatórios vazios
E tento finalizar o cadastro
Então o sistema deve informar que existem campos obrigatórios não preenchidos
```

---

# Funcionalidade: Consulta de Usuários

Como administrador do sistema
Quero visualizar todos os usuários cadastrados
Para gerenciar os registros existentes

```gherkin
Funcionalidade: Listagem de usuários

Cenário: Visualizar lista de usuários
Dado que existem usuários cadastrados no sistema
Quando acesso a página de usuários
Então o sistema deve exibir uma tabela com todos os usuários registrados

Cenário: Nenhum usuário cadastrado
Dado que não existem usuários cadastrados no sistema
Quando acesso a página de usuários
Então o sistema deve informar que não há usuários cadastrados
```

---

# Funcionalidade: Atualização de Usuário

Como administrador do sistema
Quero editar informações de um usuário
Para manter os dados atualizados

```gherkin
Funcionalidade: Atualização de usuário

Cenário: Atualizar dados de usuário com sucesso
Dado que estou na página de edição de um usuário existente
Quando modifico os dados necessários
E salvo as alterações
Então o sistema deve exibir a mensagem "Usuário atualizado com sucesso"

Cenário: Atualização com dados inválidos
Dado que estou editando um usuário existente
Quando informo dados inválidos
E tento salvar as alterações
Então o sistema deve exibir uma mensagem de erro
```

---

# Funcionalidade: Exclusão de Usuário

Como administrador do sistema
Quero remover usuários
Para manter o sistema organizado

```gherkin
Funcionalidade: Exclusão de usuário

Cenário: Remover usuário com sucesso
Dado que estou na página de listagem de usuários
E existe um usuário que desejo excluir
Quando clico no botão "Excluir"
Então o sistema deve remover o usuário
E ele não deve mais aparecer na lista

Cenário: Cancelar exclusão de usuário
Dado que selecionei um usuário para exclusão
Quando cancelo a operação
Então o usuário deve permanecer cadastrado no sistema
```

---

# Funcionalidade: Login no Sistema

Como usuário do sistema
Quero realizar login
Para acessar minhas funcionalidades

```gherkin
Funcionalidade: Login

Cenário: Login realizado com sucesso
Dado que estou na página de login
E possuo um usuário válido
Quando informo email e senha corretos
E clico em "Entrar"
Então devo ser redirecionado para a página inicial

Cenário: Tentativa de login com credenciais incorretas
Dado que estou na página de login
Quando informo email ou senha inválidos
E clico em "Entrar"
Então o sistema deve exibir a mensagem "Credenciais inválidas"
```
