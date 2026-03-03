# 🧩 Cenários de Teste – SoulVerse (Testes Manuais)

---

## 📌 Módulo: Cadastro de Conta

### CT-CAD-001 — Cadastro com dados válidos
- **Pré-condição:** Usuário não cadastrado anteriormente
- **Dados de teste:**  
  - Usuário: `Teste01`  
  - Email: `Teste01@gmail.com`  
  - Senha: `123456`  
  - Confirmar senha: `123456`
- **Passos:**
  1. Acessar a tela de cadastro
  2. Preencher Usuário, Email, Senha e Confirmar senha com dados válidos
  3. Clicar em **Registrar**
- **Resultado esperado:** Cadastro realizado com sucesso (exibir mensagem de sucesso: "Your account has been created!")

Execução do Teste

- Status: ✔ Pass

- Data da execução: 16/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Cadastro/CT-CAD-001_Sucesso.gif)

---

### CT-CAD-002 — Tentar registrar com campos vazios
- **Pré-condição:** Estar na tela de cadastro
- **Passos:**
  1. Deixar todos os campos vazios
  2. Clicar em **Registrar**
- **Resultado esperado:** Sistema impede o cadastro e exibe mensagens de validação para campos obrigatórios

Execução do Teste

- Status: ✔ Pass

- Data da execução: 17/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Cadastro/CT-CAD-002_Sucesso.gif)

---

### CT-CAD-003 — Usuário com menos de 3 letras
- **Dados de teste:** Usuário: `AB`
- **Passos:**
  1. Preencher todos os campos corretamente, exceto Usuário com menos de 3 letras
  2. Clicar em **Registrar**
- **Resultado esperado:** Sistema impede o cadastro e informa que o Usuário deve ter no mínimo 3 letras

Execução do Teste

- Status: ✔ Pass

- Data da execução: 17/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Cadastro/CT-CAD-003_Sucesso.gif)

---

### CT-CAD-004 — Senha com menos de 3 caracteres
- **Dados de teste:** Senha: `ab`
- **Passos:**
  1. Preencher todos os campos corretamente, exceto Senha com menos de 3 caracteres
  2. Clicar em **Registrar**
- **Resultado esperado:** Sistema impede o cadastro e informa que a senha deve ter no mínimo 3 caracteres

Execução do Teste

- Status: ✔ Pass

- Data da execução: 17/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Cadastro/CT-CAD-004_Sucesso.gif)

---

### CT-CAD-005 — Confirmar senha diferente da senha
- **Dados de teste:**  
  - Senha: `abc`  
  - Confirmar senha: `abcd`
- **Passos:**
  1. Preencher todos os campos
  2. Informar Senha e Confirmar senha diferentes
  3. Clicar em **Registrar**
- **Resultado esperado:** Sistema impede o cadastro e exibe mensagem informando que as senhas não coincidem

Execução do Teste

- Status: ✔ Pass

- Data da execução: 17/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Cadastro/CT-CAD-005_Sucesso.gif)

---

### CT-CAD-006 — Email em formato inválido
- **Dados de teste:** Email: `testegmail`
- **Passos:**
  1. Preencher os campos com Email inválido
  2. Clicar em **Registrar**
- **Resultado esperado:** Sistema impede o cadastro e informa que o Email é inválido

Execução do Teste

- Status: ✔ Pass

- Data da execução: 17/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Cadastro/CT-CAD-006_Sucesso.gif)

---

### CT-CAD-007 — Verificar se o botão Registrar valida antes de enviar
- **Objetivo:** Garantir que ao clicar em Registrar o sistema valida campos obrigatórios e regras mínimas
- **Passos:**
  1. Preencher apenas 1 ou 2 campos
  2. Clicar em **Registrar**
- **Resultado esperado:** Sistema não conclui cadastro e aponta exatamente quais campos/regas faltam

Execução do Teste

- Status: ✔ Pass

- Data da execução: 17/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Cadastro/CT-CAD-007_Sucesso.gif)


## 📌 Módulo: Login

### CT-LOG-001 — Login com credenciais válidas (servidor Online)
- **Pré-condição:** Server status = **Online** e usuário cadastrado
- **Dados de teste:**
  - Usuário: `Teste01`
  - Senha: `123456`
- **Passos:**
  1. Abrir o cliente do jogo
  2. Confirmar que o **Server status** está **Online**
  3. Informar Usuário e Senha válidos
  4. Clicar em **Entrar**
- **Resultado esperado:** Login realizado com sucesso e redirecionar para a próxima tela (seleção de personagem)

Execução do Teste

- Status: ✔ Pass

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Login/CT-LOG-001_Sucesso.gif)

---

### CT-LOG-002 — Tentar entrar com campos vazios
- **Pré-condição:** Server status = **Online**
- **Passos:**
  1. Deixar Usuário e Senha vazios
  2. Clicar em **Entrar**
- **Resultado esperado:** Sistema impede login e exibe validação de campos obrigatórios

Execução do Teste

- Status: ✔ Pass

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Login/CT-LOG-002_Sucesso.gif)

---

### CT-LOG-003 — Usuário com menos de 3 letras
- **Pré-condição:** Server status = **Online**
- **Dados de teste:** Usuário: `ab`
- **Passos:**
  1. Preencher Senha com valor válido
  2. Informar Usuário com menos de 3 letras
  3. Clicar em **Entrar**
- **Resultado esperado:** Sistema impede login e informa regra de mínimo 3 letras para Usuário ou Senha

Execução do Teste

- Status: ✔ Pass

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../..//Evidencias/Login/CT-LOG-003_Sucesso.gif)

---

### CT-LOG-004 — Senha com menos de 3 caracteres
- **Pré-condição:** Server status = **Online**
- **Dados de teste:** Senha: `12`
- **Passos:**
  1. Preencher Usuário com valor válido
  2. Informar Senha com menos de 3 caracteres
  3. Clicar em **Entrar**
- **Resultado esperado:** Sistema impede login e informa regra de mínimo 3 caracteres para Usuário ou Senha

Execução do Teste

- Status: ✔ Pass

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Login/CT-LOG-004_Sucesso.gif)

---

### CT-LOG-005 — Usuário inexistente
- **Pré-condição:** Server status = **Online**
- **Dados de teste:** Usuário: `Teste00` Senha: `123456`
- **Passos:**
  1. Informar usuário inexistente e uma senha qualquer
  2. Clicar em **Entrar**
- **Resultado esperado:** Sistema não loga e exibe mensagem de credenciais inválidas: "That account name does not exist."

Execução do Teste

- Status: ✔ Pass

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Login/CT-LOG-005_Sucesso.gif)

---

### CT-LOG-006 — Senha incorreta para usuário existente
- **Pré-condição:** Server status = **Online** e usuário cadastrado
- **Passos:**
  1. Informar Usuário válido
  2. Informar Senha incorreta
  3. Clicar em **Entrar**
- **Resultado esperado:** Sistema não loga e exibe mensagem de erro: "You've entered an incorrect password."

Execução do Teste

- Status: ✔ Pass

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Login/CT-LOG-006_Sucesso.gif)

---

### CT-LOG-007 — Tentar logar com servidor Offline
- **Pré-condição:** Server status = **Offline**
- **Passos:**
  1. Abrir o cliente
  2. Confirmar que o Server status está **Offline**
  3. Informar Usuário e Senha válidos
  4. Clicar em **Entrar**
- **Resultado esperado:** Sistema impede login e informa que o servidor está indisponível/offline

Execução do Teste

- Status: ❌ Fail

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Login/CT-LOG-007_Fail.gif)

- Defeito relacionado: BUG-002

- Motivo do Fail:

- Resultado esperado não foi atendido (não exibiu mensagem ao usuário que o servidor está offline)


---

### CT-LOG-008 — Link “Clique aqui” leva para cadastro
- **Pré-condição:** Estar na tela de login
- **Passos:**
  1. Clicar em **Clique aqui** (Ainda não possui conta?)
- **Resultado esperado:** Abrir a tela de cadastro/registro

Execução do Teste

- Status: ✔ Pass

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Login/CT-LOG-008_Sucesso.gif)

---

### CT-LOG-009 — Botão “X” fecha a janela de login
- **Pré-condição:** Janela de login aberta
- **Passos:**
  1. Clicar no botão **X**
- **Resultado esperado:** Janela de login é fechada (sair do jogo)

Execução do Teste

- Status: ✔ Pass

- Data da execução: 18/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Login/CT-LOG-009_Sucesso.gif)

---

## 📌 Módulo: Seleção de Personagem

### CT-SEL-001 — Exibir slots vazios corretamente
- **Pré-condição:** Login realizado com conta sem personagens criados
- **Passos:**
  1. Realizar login com sucesso
- **Resultado esperado:**
  - Exibir 8 slots
  - Cada slot deve mostrar "Slot de Personagem Vazio"

  Execução do Teste

- Status: ✔ Pass

- Data da execução: 19/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Selecao-Personagem/CT-SEL-001_Sucesso.gif)

---

### CT-SEL-002 — Botão Criar redireciona para criação
- **Pré-condição:** Estar na tela de seleção
- **Passos:**
  1. Clicar em "Criar"
- **Resultado esperado:**
  - Sistema deve abrir tela de criação de personagem

 Execução do Teste

- Status: ✔ Pass

- Data da execução: 19/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Selecao-Personagem/CT-SEL-002_Sucesso.gif)  

---

### CT-SEL-003 — Botão Voltar retorna para tela anterior
- **Pré-condição:** Estar na tela de seleção
- **Passos:**
  1. Clicar em "Voltar"
- **Resultado esperado:**
  - Retornar para tela anterior (login ou menu principal)

  Execução do Teste

- Status: ✔ Pass

- Data da execução: 19/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Selecao-Personagem/CT-SEL-003_Sucesso.gif) 

---

### CT-SEL-004 — Scroll lateral funciona corretamente
- **Pré-condição:** Estar na tela de seleção
- **Passos:**
  1. Utilizar a barra de rolagem
- **Resultado esperado:**
  - Rolagem suave
  - Nenhum travamento visual

  Execução do Teste

- Status: ✔ Pass

- Data da execução: 19/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Selecao-Personagem/CT-SEL-001_Sucesso.gif)

---

## CT-SEL-005 — Conectar ao jogo após selecionar personagem

**Pré-condição:**  
Usuário logado com sucesso e possuir pelo menos 1 personagem criado. Servidor com status **Online**.

**Passos:**

1. Realizar login com credenciais válidas  
2. Na tela de seleção, escolher um personagem existente  
3. Clicar em **Entrar**  
4. Aguardar carregamento do mapa inicial  

**Resultado esperado:**  
Sistema deve carregar o personagem corretamente no mapa inicial, exibir HUD (vida, mana, level, etc.) e permitir movimentação sem apresentar erro de conexão ou travamento.

Execução do Teste

- Status: ✔ Pass  
- Data da execução: 03/03/2026
- Versão testada: Beta  
- Ambiente: Cliente Desktop  
- Executor: Daniel Chicotti  

**Evidência:** [Visualizar GIF](../../Evidencias/Selecao-Personagem/CT-SEL-005_Sucesso.gif)

---

## 📌 Módulo: Criação de Personagem

## CT-CHAR-001 — Criar personagem com dados válidos

**Pré-condição:** Estar na tela de seleção

**Dados de teste:**

* Nome: Ichigo (Ou algum outro nome se esse já estiver sendo utilizado)

**Passos:**

1. Acessar a tela de criação de personagem
2. Informar um nome válido
3. Manter a classe padrão (Shinigami)
4. Clicar em **Criar**

**Resultado esperado:**
Personagem criado com sucesso e entrada no jogo.

Execução do Teste

- Status: ✔ Pass

- Data da execução: 24/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Criacao-Personagem/CT-CHAR-001_Sucesso.gif)

---

## CT-CHAR-002 — Verificar classe padrão selecionada

**Pré-condição:** Usuário logado

**Passos:**

1. Acessar a tela de criação de personagem

**Resultado esperado:**
A classe **Shinigami** deve estar selecionada automaticamente.

Execução do Teste

- Status: ✔ Pass

- Data da execução: 24/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Criacao-Personagem/CT-CHAR-002_Sucesso.gif)

---

## CT-CHAR-003 — Alterar classe do personagem

**Pré-condição:** Usuário logado

**Passos:**

1. Acessar a tela de criação de personagem
2. Selecionar a classe **Hollow**
3. Informar um nome válido
4. Clicar em **Criar**

**Resultado esperado:**
Personagem criado com a classe selecionada.

(Repetir o teste para Quincy e Ryoka)

Execução do Teste

- Status: ✔ Pass

- Data da execução: 24/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Criacao-Personagem/CT-CHAR-003_Sucesso.gif)

---

## CT-CHAR-004 — Tentar criar personagem sem nome

**Pré-condição:** Usuário logado

**Passos:**

1. Acessar a tela de criação de personagem
2. Deixar o campo de nome vazio
3. Clicar em **Criar**

**Resultado esperado:**
Sistema deve impedir a criação e exibir mensagem informando que o nome é obrigatório.

Execução do Teste

- Status: ✔ Pass

- Data da execução: 24/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Criacao-Personagem/CT-CHAR-004_Sucesso.gif)

---

## CT-CHAR-005 — Inserir nome com menos de 3 caracteres

**Pré-condição:** Usuário logado

**Dados de teste:**

* Nome: Ab

**Passos:**

1. Acessar a tela de criação de personagem
2. Informar nome com menos de 3 caracteres
3. Clicar em **Criar**

**Resultado esperado:**
Sistema deve exibir validação informando o tamanho mínimo.

Execução do Teste

- Status: ✔ Pass

- Data da execução: 24/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Criacao-Personagem/CT-CHAR-005_Sucesso.gif)

---

## CT-CHAR-006 — Inserir nome com caracteres especiais

**Pré-condição:** Usuário logado

**Dados de teste:**

* Nome: Ichigo!@#

**Passos:**

1. Acessar a tela de criação de personagem
2. Informar nome com caracteres especiais
3. Clicar em **Criar**

**Resultado esperado:**
Sistema deve aceitar apenas caracteres permitidos (letras e números) e exibir mensagem de validação.

Execução do Teste

- Status: ❌ Fail

- Data da execução: 24/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Criacao-Personagem/CT-CHAR-006_Fail.gif)

---

## CT-CHAR-007 — Inserir nome acima do limite permitido

**Pré-condição:** Usuário logado

**Dados de teste:**

* Nome com mais de 50 caracteres

**Passos:**

1. Acessar a tela de criação de personagem
2. Inserir nome muito longo
3. Clicar em **Criar**

**Resultado esperado:**
Sistema deve limitar automaticamente a quantidade de caracteres e permitir a criação de persongem.

Execução do Teste

- Status: ✔ Pass

- Data da execução: 24/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Criacao-Personagem/CT-CHAR-007_Sucesso.gif)

---

## CT-CHAR-008 — Tentar criar múltiplos personagens com o mesmo nome

**Pré-condição:** Já existe um personagem com o nome “Ichigo”

**Passos:**

1. Acessar a tela de criação de personagem
2. Informar o mesmo nome
3. Clicar em **Criar**

**Resultado esperado:**
Sistema deve impedir a criação e informar que o nome já está em uso.

Execução do Teste

- Status: ✔ Pass

- Data da execução: 24/02/2026

- Versão testada: Beta

- Ambiente: Cliente Desktop

- Executor: Daniel Chicotti

**Evidência:** [Visualizar GIF](../../Evidencias/Criacao-Personagem/CT-CHAR-008_Sucesso.gif)



