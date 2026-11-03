# Pull Requests

Toda alteração destinada à branch principal deve passar por uma Pull Request.
Alterações diretas na branch principal não são permitidas.

## Título

```text
<Tipo da PR> - <O que foi feito>
```

Use um título claro e objetivo, sem incluir o nome do autor.
Utilize o tipo correspondente à alteração: `Feat`, `Fix`, `Docs`, `Style`,
`Refactor`, `Test`, `Chore`, `Perf` ou `Security`.

```text
Feat - Implementação do fluxo de login
Fix - Correção do cálculo do carrinho
Refactor - Reorganização da camada de serviços
Test - Implementação dos testes de autenticação
Security - Correção da validação de sessão
Perf - Otimização da consulta de produtos
```

## Template obrigatório

Preencha o [template oficial](../../.github/pull_request_template.md), apresentado
pelo GitHub na abertura da PR:

- Descrição objetiva do que foi desenvolvido, corrigido ou alterado.
- Lista de alterações.
- Impactos técnicos: banco de dados, variáveis de ambiente, dependências e outros serviços.
- Evidências quando necessário.
- Tipo da alteração.
- Referência da tarefa ou card.
- Checklist de padrões, testes, logs/debug e informações sensíveis.

Informe as validações realizadas. Quando algum item não se aplicar, justifique
na descrição; não o marque como executado.

## Referência obrigatória da tarefa

Toda PR deve informar a tarefa ou card relacionado. Substitua o exemplo pelo ID
real da tarefa e inclua o link do card quando disponível:

```markdown
## 🔗 Referências

- **Issue/Card:** ClickUp - 86e2tk3p3
```

O ID deve corresponder ao da branch, preservando o vínculo entre tarefa,
branch, commits e PR.

Antes de integrar, cumpra a [política de revisão e merge](revisao-e-merge.md).

[Voltar ao índice](README.md)
