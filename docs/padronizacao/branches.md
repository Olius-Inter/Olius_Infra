# Branches

Todas as branches de desenvolvimento devem seguir:

```text
<tipo>/<id-da-tarefa>-<descricao-curta>
```

O ID da tarefa é obrigatório. A descrição deve ser curta, objetiva e usar palavras
separadas por hífen.

## Tipos permitidos e exemplos

| Tipo | Exemplo |
| --- | --- |
| `feat` | `feat/86e2tk3p3-login-oauth` |
| `fix` | `fix/86e2tk3p3-erro-calculo-carrinho` |
| `hotfix` | `hotfix/86e2tk3p3-corrigir-crash-prod` |
| `docs` | `docs/86e2tk3p3-atualizar-readme` |
| `refactor` | `refactor/86e2tk3p3-reorganizar-api` |
| `test` | `test/86e2tk3p3-testes-login` |
| `chore` | `chore/86e2tk3p3-atualizar-dependencias` |
| `perf` | `perf/86e2tk3p3-otimizar-consulta` |
| `security` | `security/86e2tk3p3-corrigir-autenticacao` |

`hotfix` é exclusivo de branches e segue as mesmas exigências de PR, revisão e
merge. `style` é um tipo de commit, mas não consta entre os tipos de branch permitidos.

Use na PR o mesmo ID da tarefa informado na branch.

[Voltar ao índice](README.md)
