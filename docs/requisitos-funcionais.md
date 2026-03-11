# Requisitos Funcionais — Sistema Urbanly

---

## RF001 — Fazer Cadastro de Usuário
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve permitir que o usuário realize cadastro informando nome, e-mail e senha para criação de uma conta no aplicativo.

O cadastro também poderá ser realizado por meio de autenticação social utilizando conta Google.

---

## RF002 — Fazer Login
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve permitir que o usuário realize autenticação utilizando e-mail e senha ou login social com Google para acessar funcionalidades que exigem autenticação.

---

## RF003 — Editar Perfil
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve permitir que usuários autenticados editem suas informações de perfil, incluindo:

- nome
- foto
- senha

---

## RF004 — Cadastrar Estabelecimento
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve permitir o cadastro de estabelecimentos contendo as seguintes informações:

- nome do estabelecimento
- descrição
- endereço
- categoria
- palavras-chave
- horário de funcionamento
- fotos

---

## RF005 — Buscar Estabelecimentos por Palavra-Chave
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve permitir que qualquer usuário (autenticado ou não) pesquise estabelecimentos utilizando palavras-chave ou nome do local.

O sistema deve retornar uma lista de resultados correspondentes.

---

## RF006 — Filtrar Estabelecimentos
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve permitir que qualquer usuário aplique filtros aos resultados da busca.

Os filtros disponíveis devem incluir:

- categoria
- cidade
- avaliação média

---

## RF007 — Visualizar Resultados de Busca
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve exibir uma lista de estabelecimentos encontrados a partir da busca realizada.

Para usuários não autenticados, devem ser exibidas apenas informações resumidas:

- nome do estabelecimento
- categoria
- cidade
- avaliação média

---

## RF008 — Visualizar Detalhes do Estabelecimento
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve permitir que usuários autenticados visualizem informações completas sobre um estabelecimento.

As informações exibidas devem incluir:

- descrição
- endereço
- palavras-chave
- fotos
- avaliações
- comentários

Caso um usuário não autenticado tente acessar os detalhes de um estabelecimento, o sistema deve solicitar login.

---

## RF009 — Avaliar Estabelecimento
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve permitir que usuários autenticados avaliem um estabelecimento atribuindo uma nota entre **1 e 5 estrelas** e escrevendo um comentário sobre sua experiência.

---

## RF010 — Visualizar Avaliações
**Prioridade:** Essencial  

**Descrição:**  
O sistema deve exibir a lista de avaliações de um estabelecimento, incluindo:

- nota atribuída
- comentário
- nome do usuário que realizou a avaliação

Essa funcionalidade deve estar disponível apenas na visualização de detalhes do estabelecimento.

---

## RF011 — Adicionar aos Favoritos
**Prioridade:** Importante  

**Descrição:**  
O sistema deve permitir que usuários autenticados adicionem ou removam estabelecimentos de sua lista de favoritos.

---

## RF012 — Administrar Estabelecimentos
**Prioridade:** Importante  

**Descrição:**  
O sistema deve permitir que administradores gerenciem estabelecimentos cadastrados, podendo:

- cadastrar estabelecimentos
- editar estabelecimentos
- remover estabelecimentos

---

## RF013 — Moderar Avaliações
**Prioridade:** Importante  

**Descrição:**  
O sistema deve permitir que administradores removam avaliações que violem as diretrizes da plataforma.
