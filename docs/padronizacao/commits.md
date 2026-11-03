# Commits

Todos os commits devem seguir o padrão Conventional Commits:

```text
<tipo>(<escopo>): <descrição curta>
```

O tipo identifica a natureza da alteração. O escopo identifica a área afetada e
deve ser usado quando relevante. Sem escopo: `<tipo>: <descrição curta>`.
A descrição deve resumir a alteração de forma objetiva.

## Tipos permitidos

| Tipo | Utilização |
| --- | --- |
| `feat` | Nova funcionalidade |
| `fix` | Correção de bug |
| `docs` | Documentação |
| `style` | Formatação ou estilo sem mudança de comportamento |
| `refactor` | Refatoração sem correção de bug ou nova funcionalidade |
| `test` | Adição ou alteração de testes |
| `chore` | Manutenção, configurações, build ou dependências |
| `perf` | Melhoria de desempenho |
| `security` | Alterações relacionadas à segurança |

`hotfix` é exclusivo para branches. Para um commit de correção urgente, utilize
o tipo correspondente à alteração, como `fix` ou `security`.

## Exemplos

```text
feat(auth): adiciona fluxo de login
fix(cart): corrige cálculo do valor total
docs(readme): atualiza instruções de instalação
style(frontend): ajusta formatação dos componentes
refactor(api): reorganiza camada de serviços
test(auth): adiciona testes de autenticação
chore(ci): configura workflow do GitHub Actions
perf(database): otimiza consulta de produtos
security(auth): corrige validação de sessão
```

[Voltar ao índice](README.md)
