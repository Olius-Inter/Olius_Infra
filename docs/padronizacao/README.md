# Padrões de desenvolvimento

Documento oficial para padronização de commits, branches, Pull Requests, revisão
de código e merge do projeto Olius. As regras devem ser seguidas por todos os integrantes.

## Objetivo

Garantir consistência entre integrantes, organização do histórico Git,
rastreabilidade entre tarefas e código, qualidade e segurança na integração,
reduzindo erros antes do merge.

## Guias

| Documento | Conteúdo |
| --- | --- |
| [Commits](commits.md) | Formato, tipos permitidos e exemplos |
| [Branches](branches.md) | Nomenclatura e identificação da tarefa |
| [Pull Requests](pull-requests.md) | Títulos, template e rastreabilidade |
| [Revisão e merge](revisao-e-merge.md) | Verificações obrigatórias e aprovação |
| [Responsabilidades](responsabilidades.md) | Papel de cada participante e ferramenta |

## Fluxo oficial

```text
Tarefa / Card → Branch → Desenvolvimento → Commits → Pull Request
                                                       ↓
                                             CI + Sonar + CodeRabbit
                                                       ↓
                                                Revisão humana
                                                       ↓
                                                   Aprovação
                                                       ↓
                                                     Merge
```

A tarefa deve ser rastreável pela branch, pelos commits associados, pela PR,
pela revisão e pelo merge.

## Resumo das regras

| Elemento | Padrão |
| --- | --- |
| Commit | `<tipo>(<escopo>): <descrição>`; escopo quando relevante |
| Branch | `<tipo>/<id-da-tarefa>-<descricao-curta>` |
| Hotfix | Tipo exclusivo de branch |
| Título da PR | `<Tipo da PR> - <O que foi feito>`, sem nome do autor |
| ID da tarefa na PR | Obrigatório |
| Template da PR | Obrigatório |
| CI | Obrigatório, com verificações obrigatórias aprovadas |
| Sonar | Obrigatório, com Quality Gate aprovado |
| CodeRabbit | Execução obrigatória, como auxílio à revisão |
| Aprovação humana | Mínimo de uma antes do merge |
| Integração direta na principal | Não permitida |

## Exemplo completo

Para a tarefa `86e2tk3p3 - Implementar login OAuth`:

```text
Branch: feat/86e2tk3p3-login-oauth

Commits:
feat(auth): adiciona tela de login
feat(auth): implementa autenticação OAuth
test(auth): adiciona testes de autenticação

Título da PR: Feat - Implementação do fluxo de login
Referência na PR: Issue/Card: ClickUp - 86e2tk3p3
```

Após CI e testes aprovados, Sonar com Quality Gate aprovado, execução do
CodeRabbit e pelo menos uma aprovação humana, a alteração pode ser integrada.

## Aplicação das regras

Estes arquivos definem a política. O template em
[`.github/pull_request_template.md`](../../.github/pull_request_template.md)
é apresentado pelo GitHub ao abrir uma PR.

A aplicação automática da política depende de configurar CI, Sonar, CodeRabbit
e proteção da branch principal no GitHub. A criação desta documentação não ativa
essas integrações nem configura bloqueios de merge.
