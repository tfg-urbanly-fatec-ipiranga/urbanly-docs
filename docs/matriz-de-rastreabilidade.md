# Matriz de Rastreabilidade — Sistema Urbanly

A matriz de rastreabilidade estabelece a relação entre **requisitos funcionais**, **casos de uso**, **regras de negócio** e **diagramas UML**, garantindo que todos os requisitos definidos sejam atendidos pelos elementos de modelagem do sistema.

---

# Relação entre Requisitos Funcionais e Casos de Uso

| Requisito Funcional | Descrição | Caso de Uso |
|---|---|---|
| RF001 | Fazer cadastro de usuário | UC01 — Criar Conta |
| RF002 | Fazer login | UC02 — Autenticar Usuário |
| RF003 | Editar perfil | UC02 — Autenticar Usuário |
| RF004 | Cadastrar estabelecimento | UC08 — Administrar Estabelecimentos |
| RF005 | Buscar estabelecimentos por palavra-chave | UC03 — Buscar Estabelecimentos |
| RF006 | Filtrar estabelecimentos | UC04 — Filtrar Estabelecimentos |
| RF007 | Visualizar resultados de busca | UC03 — Buscar Estabelecimentos |
| RF008 | Visualizar detalhes do estabelecimento | UC05 — Visualizar Detalhes |
| RF009 | Avaliar estabelecimento | UC06 — Avaliar Estabelecimento |
| RF010 | Visualizar avaliações | UC05 — Visualizar Detalhes |
| RF011 | Adicionar aos favoritos | UC07 — Favoritar Estabelecimento |
| RF012 | Administrar estabelecimentos | UC08 — Administrar Estabelecimentos |
| RF013 | Moderar avaliações | UC09 — Moderar Avaliações |

---

# Relação entre Casos de Uso e Regras de Negócio

| Caso de Uso | Regras de Negócio Associadas |
|---|---|
| UC03 — Buscar Estabelecimentos | RN002, RN005, RN007 |
| UC04 — Filtrar Estabelecimentos | RN002, RN005 |
| UC05 — Visualizar Detalhes | RN007, RN008 |
| UC06 — Avaliar Estabelecimento | RN001, RN003 |
| UC07 — Favoritar Estabelecimento | RN008 |
| UC08 — Administrar Estabelecimentos | RN004, RN006 |
| UC09 — Moderar Avaliações | RN001 |

---

# Relação entre Casos de Uso e Diagramas UML

| Caso de Uso | Diagramas Relacionados |
|---|---|
| UC01 — Criar Conta | Diagrama de Casos de Uso |
| UC02 — Autenticar Usuário | Diagrama de Casos de Uso |
| UC03 — Buscar Estabelecimentos | Diagrama de Atividades — Busca de Estabelecimentos |
| UC04 — Filtrar Estabelecimentos | Diagrama de Atividades — Busca de Estabelecimentos |
| UC05 — Visualizar Detalhes | Diagrama de Atividades — Busca de Estabelecimentos |
| UC06 — Avaliar Estabelecimento | Diagrama de Atividades — Avaliar Estabelecimento |
| UC07 — Favoritar Estabelecimento | Diagrama de Casos de Uso |
| UC08 — Administrar Estabelecimentos | Diagrama de Casos de Uso |
| UC09 — Moderar Avaliações | Diagrama de Casos de Uso |

---

# Relação entre Requisitos Funcionais e Diagramas

| Requisito Funcional | Diagramas Relacionados |
|---|---|
| RF001 | Diagrama de Casos de Uso |
| RF002 | Diagrama de Casos de Uso |
| RF003 | Diagrama de Casos de Uso |
| RF004 | Diagrama de Casos de Uso |
| RF005 | Diagrama de Atividades — Busca |
| RF006 | Diagrama de Atividades — Busca |
| RF007 | Diagrama de Atividades — Busca |
| RF008 | Diagrama de Atividades — Busca |
| RF009 | Diagrama de Atividades — Avaliação |
| RF010 | Diagrama de Atividades — Avaliação |
| RF011 | Diagrama de Casos de Uso |
| RF012 | Diagrama de Casos de Uso |
| RF013 | Diagrama de Casos de Uso |

---

# Visão Geral de Rastreabilidade

```

Requisitos Funcionais
↓
Casos de Uso
↓
Regras de Negócio
↓
Diagramas UML

```

Essa estrutura garante que:

- todos os requisitos possuem representação nos casos de uso
- as regras de negócio são aplicadas corretamente
- os diagramas UML representam as funcionalidades do sistema.
