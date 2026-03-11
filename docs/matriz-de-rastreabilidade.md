# Matriz de Rastreabilidade — Urbanly

A matriz de rastreabilidade relaciona **requisitos funcionais** com os **casos de uso**, garantindo que todos os requisitos definidos sejam atendidos pelo sistema.

| Requisito | Descrição                                 | Caso de Uso                                |
| --------- | ----------------------------------------- | ------------------------------------------ |
| RF001     | Fazer cadastro de usuário                 | UC01 — Criar conta                         |
| RF002     | Fazer login                               | UC02 — Autenticar                          |
| RF003     | Editar perfil                             | UC11 — Editar perfil                       |
| RF004     | Cadastrar estabelecimento                 | UC08 — Cadastrar estabelecimento           |
| RF005     | Buscar estabelecimentos por palavra-chave | UC03 — Buscar estabelecimentos             |
| RF006     | Filtrar estabelecimentos                  | UC04 — Buscar estabelecimentos com filtros |
| RF007     | Visualizar detalhes do estabelecimento    | UC05 — Visualizar detalhes                 |
| RF008     | Avaliar estabelecimento                   | UC06 — Avaliar estabelecimento             |
| RF009     | Visualizar avaliações                     | UC05 — Visualizar detalhes                 |
| RF010     | Adicionar aos favoritos                   | UC07 — Favoritar estabelecimento           |
| RF011     | Visualizar estabelecimentos por cidade    | UC04 — Buscar com filtros                  |
| RF012     | Administrar estabelecimentos              | UC08 / UC09                                |
| RF013     | Moderar avaliações                        | UC10 — Moderar avaliações                  |

---

## Relação com Regras de Negócio

| Regra de Negócio | Casos de Uso Relacionados |
| ---------------- | ------------------------- |
| RN001            | UC06                      |
| RN002            | UC03 / UC04               |
| RN003            | UC06                      |
| RN004            | UC08                      |
| RN005            | UC03 / UC04               |
| RN006            | UC08                      |
