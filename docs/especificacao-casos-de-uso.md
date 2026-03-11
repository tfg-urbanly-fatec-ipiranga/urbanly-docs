# Especificação de Casos de Uso — Sistema Urbanly

---

## UC01 — Criar Conta

**Ator principal:** Visitante  

**Descrição:**  
Permite que um visitante crie uma conta no sistema para acessar funcionalidades restritas do aplicativo.

**Pré-condições**
- O usuário ainda não possui conta cadastrada.

**Fluxo principal**

1. O visitante acessa a opção de cadastro.
2. O sistema solicita os dados necessários.
3. O visitante informa:
   - nome
   - e-mail
   - senha
4. O sistema valida os dados informados.
5. O sistema cria a conta.
6. O sistema confirma o cadastro.

**Fluxos alternativos**

**4A – E-mail já cadastrado**

1. O sistema detecta que o e-mail já está em uso.
2. O sistema informa o erro ao usuário.

**Pós-condições**

- Uma nova conta é registrada no sistema.

---

## UC02 — Autenticar Usuário

**Ator principal:** Usuário  

**Descrição:**  
Permite que o usuário realize login no sistema para acessar funcionalidades que exigem autenticação.

**Pré-condições**

- O usuário possui conta cadastrada.

**Fluxo principal**

1. O usuário acessa a tela de login.
2. O usuário informa e-mail e senha.
3. O sistema valida as credenciais.
4. O sistema autentica o usuário.
5. O usuário passa a ter acesso às funcionalidades autenticadas.

**Fluxos alternativos**

**3A – Credenciais inválidas**

1. O sistema identifica erro nas credenciais.
2. O sistema solicita nova tentativa.

**Pós-condições**

- O usuário está autenticado no sistema.

---

## UC03 — Buscar Estabelecimentos

**Ator principal:** Visitante / Usuário  

**Descrição:**  
Permite que qualquer usuário realize buscas por estabelecimentos utilizando palavras-chave.

**Pré-condições**

- O sistema está disponível.

**Fluxo principal**

1. O usuário acessa a funcionalidade de busca.
2. O usuário informa uma palavra-chave.
3. O sistema processa a busca.
4. O sistema retorna os resultados encontrados.

**Informações exibidas nos resultados**

- nome do estabelecimento
- categoria
- cidade
- avaliação média

**Pós-condições**

- O sistema apresenta uma lista de estabelecimentos correspondentes à busca.

---

## UC04 — Filtrar Estabelecimentos

**Ator principal:** Visitante / Usuário  

**Descrição:**  
Permite aplicar filtros adicionais aos resultados da busca.

**Pré-condições**

- Uma busca já foi realizada.

**Fluxo principal**

1. O usuário seleciona filtros.
2. O usuário define critérios como:
   - cidade
   - categoria
   - avaliação
3. O sistema aplica os filtros.
4. O sistema atualiza os resultados da busca.

**Pós-condições**

- Os resultados exibidos refletem os filtros aplicados.

---

## UC05 — Visualizar Detalhes do Estabelecimento

**Ator principal:** Usuário  

**Descrição:**  
Permite que usuários autenticados visualizem informações completas sobre um estabelecimento.

**Pré-condições**

- O usuário está autenticado.
- O estabelecimento existe no sistema.

**Fluxo principal**

1. O usuário seleciona um estabelecimento nos resultados da busca.
2. O sistema verifica se o usuário está autenticado.
3. O sistema exibe os detalhes completos do estabelecimento.

**Informações exibidas**

- descrição
- endereço
- palavras-chave
- fotos
- avaliações
- comentários

**Fluxo alternativo**

**2A – Usuário não autenticado**

1. O sistema solicita login.
2. O usuário realiza autenticação.
3. O sistema exibe os detalhes do estabelecimento.

**Pós-condições**

- O usuário visualiza as informações completas do estabelecimento.

---

## UC06 — Avaliar Estabelecimento

**Ator principal:** Usuário  

**Descrição:**  
Permite que usuários autenticados avaliem um estabelecimento.

**Pré-condições**

- O usuário está autenticado.
- O estabelecimento existe.

**Fluxo principal**

1. O usuário acessa os detalhes do estabelecimento.
2. O usuário seleciona a opção de avaliação.
3. O usuário atribui uma nota (1 a 5 estrelas).
4. O usuário escreve um comentário.
5. O sistema salva a avaliação.

**Pós-condições**

- A avaliação é registrada no sistema.

---

## UC07 — Favoritar Estabelecimento

**Ator principal:** Usuário  

**Descrição:**  
Permite que o usuário adicione um estabelecimento à sua lista de favoritos.

**Pré-condições**

- Usuário autenticado.

**Fluxo principal**

1. O usuário visualiza um estabelecimento.
2. O usuário seleciona a opção "favoritar".
3. O sistema registra o estabelecimento na lista de favoritos do usuário.

**Pós-condições**

- O estabelecimento é salvo na lista de favoritos.

---

## UC08 — Administrar Estabelecimentos

**Ator principal:** Administrador  

**Descrição:**  
Permite que administradores gerenciem estabelecimentos cadastrados no sistema.

**Pré-condições**

- Administrador autenticado.

**Fluxo principal**

1. O administrador acessa a área administrativa.
2. O administrador pode:
   - cadastrar estabelecimentos
   - editar estabelecimentos
   - remover estabelecimentos.

**Pós-condições**

- As informações dos estabelecimentos são atualizadas no sistema.

---

## UC09 — Moderar Avaliações

**Ator principal:** Administrador  

**Descrição:**  
Permite que o administrador modere avaliações feitas pelos usuários.

**Pré-condições**

- Administrador autenticado.

**Fluxo principal**

1. O administrador acessa a lista de avaliações.
2. O administrador seleciona uma avaliação.
3. O administrador pode remover avaliações inadequadas.

**Pós-condições**

- A avaliação é removida ou mantida no sistema.
