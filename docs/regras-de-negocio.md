# Regras de Negócio — Sistema Urbanly

## RN001 — Avaliação apenas para usuários autenticados

O sistema deve permitir que **apenas usuários autenticados** realizem avaliações e comentários em estabelecimentos.

---

## RN002 — Busca disponível para usuários não autenticados

Usuários não autenticados devem poder:

* buscar estabelecimentos
* visualizar detalhes de estabelecimentos
* visualizar avaliações

Não sendo necessário realizar login para essas ações.

---

## RN003 — Uma avaliação por usuário em cada estabelecimento

Cada usuário poderá registrar **apenas uma avaliação por estabelecimento**.

Caso o usuário já tenha realizado uma avaliação, o sistema deve permitir:

* edição da avaliação existente
* atualização da nota e comentário

Não deve permitir múltiplas avaliações para o mesmo local.

---

## RN004 — Associação obrigatória de palavras-chave

Todo estabelecimento cadastrado deve possuir **pelo menos uma palavra-chave associada**.

Essas palavras-chave serão utilizadas para:

* indexação
* busca
* recomendação de estabelecimentos.

---

## RN005 — Exibir apenas estabelecimentos ativos

O sistema deve exibir nas buscas **somente estabelecimentos com status ativo**.

Estabelecimentos removidos ou desativados pelo administrador não devem aparecer nos resultados.

---

## RN006 — Palavras-chave únicas por estabelecimento

O sistema deve garantir que **palavras-chave associadas a um estabelecimento não sejam duplicadas**, evitando inconsistência nos resultados de busca.
