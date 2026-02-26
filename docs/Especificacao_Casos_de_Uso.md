# Especificação de Casos de Uso

## Buscar estabelecimentos por palavra-chave

**Atores:** Usuário (deslogado ou logado)\
**Objetivo:** Encontrar estabelecimentos relacionados a uma
palavra-chave.\

### Fluxo Principal

1.  Usuário informa palavra-chave.
2.  Sistema valida entrada (não vazia).
3.  Sistema executa busca.
4.  Sistema exibe lista resumida de estabelecimentos.

### Fluxos Alternativos

-   Palavra-chave vazia → sistema solicita preenchimento.
-   Nenhum resultado encontrado → sistema informa e sugere ajustar
    termos.

### Pós-condições

Lista de resultados exibida.

------------------------------------------------------------------------

## Buscar estabelecimentos por palavra-chave, localização e interesses

**Atores:** Usuário\
**Objetivo:** Refinar resultados considerando localização e interesses.\
**Pré-condições:** Permissão de localização concedida ou localização
informada manualmente e usuário autenticado.\

### Fluxo Principal

1.  Usuário informa palavra-chave.
2.  Usuário define filtros (distância/interesses).
3.  Sistema obtém localização.
4.  Sistema executa busca com filtros.
5.  Sistema exibe resultados ordenados por relevância e proximidade.

### Fluxos Alternativos

-   Usuário nega localização → busca apenas por palavra-chave.
-   Nenhum resultado → sistema sugere ampliar raio ou remover filtros.

### Pós-condições

Lista filtrada exibida.

------------------------------------------------------------------------

## Visualizar detalhes de estabelecimento

**Atores:** Usuário\
**Objetivo:** Visualizar informações detalhadas do estabelecimento.\
**Pré-condições:** Usuário autenticado.\

### Fluxo Principal

1.  Sistema valida autenticação.
2.  Sistema carrega detalhes do estabelecimento.
3.  Sistema exibe tela de detalhes.

### Fluxos Alternativos

-   Usuário deslogado → redirecionar para autenticação.
-   Estabelecimento indisponível → informar e retornar à lista.

### Pós-condições

Detalhes exibidos.

------------------------------------------------------------------------

## Avaliar estabelecimento

**Atores:** Usuário\
**Objetivo:** Registrar avaliação com nota e comentário.\
**Pré-condições:** Usuário autenticado.\

### Fluxo Principal

1.  Usuário informa nota (1 a 5) e comentário opcional.
2.  Sistema valida dados.
3.  Sistema salva avaliação.
4.  Sistema atualiza média e exibe confirmação.

### Fluxos Alternativos

-   Usuário já avaliou → permitir edição.

### Pós-condições

Avaliação registrada.

------------------------------------------------------------------------

## Favoritar estabelecimento

**Atores:** Usuário\
**Objetivo:** Salvar estabelecimento como favorito.\
**Pré-condições:** Usuário autenticado.\

### Fluxo Principal

1.  Sistema registra favorito.
2.  Sistema atualiza interface.

### Fluxos Alternativos

-   Já favoritado → remover favorito (toggle).

### Pós-condições

Estabelecimento favoritado ou desfavoritado.

------------------------------------------------------------------------

## Criar conta

**Atores:** Usuário\
**Objetivo:** Criar nova conta no sistema.\

### Fluxo Principal

1.  Usuário escolhe método (e-mail ou Google).
2.  Sistema valida dados.
3.  Sistema cria conta.
4.  Sistema inicia sessão (opcional).

### Fluxos Alternativos

-   E-mail já cadastrado → sugerir login.

### Pós-condições

Conta criada.

------------------------------------------------------------------------

## Autenticar

**Atores:** Usuário\
**Objetivo:** Iniciar sessão no sistema.\
**Pré-condições:** Conta existente.\

### Fluxo Principal

1.  Usuário informa credenciais ou utiliza Google.
2.  Sistema valida autenticação.
3.  Sistema inicia sessão.

### Fluxos Alternativos

-   Credenciais inválidas → informar erro.

### Pós-condições

Usuário autenticado.

------------------------------------------------------------------------

## Cadastrar estabelecimentos

**Atores:** Administrador\
**Objetivo:** Inserir novo estabelecimento no sistema.\
**Pré-condições:** Administrador autenticado.\

### Fluxo Principal

1.  Admin preenche dados obrigatórios.
2.  Sistema valida informações.
3.  Sistema salva estabelecimento.

### Pós-condições

Estabelecimento disponível para busca.

------------------------------------------------------------------------

## Editar detalhes dos estabelecimentos

**Atores:** Administrador\
**Objetivo:** Atualizar informações do estabelecimento.\
**Pré-condições:** Administrador autenticado.\
**Gatilho:** Admin seleciona "Editar".

### Fluxo Principal

1.  Sistema exibe dados atuais.
2.  Admin altera informações.
3.  Sistema valida e salva alterações.

### Pós-condições

Estabelecimento atualizado.

------------------------------------------------------------------------

## Moderar comentários

**Atores:** Administrador\
**Objetivo:** Garantir qualidade e segurança dos comentários.\
**Pré-condições:** Administrador autenticado.\

### Fluxo Principal

1.  Sistema exibe comentários pendentes.
2.  Admin aprova, remove ou oculta comentário.
3.  Sistema registra decisão.

### Pós-condições

Comentários moderados.
