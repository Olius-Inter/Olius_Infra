# Como contribuir

Todas as contribuições devem seguir os [padrões de desenvolvimento](docs/padronizacao/README.md).

1. Identifique a tarefa ou card relacionado à alteração.
2. Crie uma [branch](docs/padronizacao/branches.md) com o ID obrigatório da tarefa.
3. Desenvolva a alteração e execute as validações locais aplicáveis.
4. Registre as alterações em [commits padronizados](docs/padronizacao/commits.md).
5. Abra uma [Pull Request](docs/padronizacao/pull-requests.md) para a branch principal, preenchendo o template e a referência da tarefa.
6. Aguarde CI, Sonar e CodeRabbit; corrija os problemas identificados na revisão.
7. Obtenha pelo menos uma aprovação humana e cumpra a [política de merge](docs/padronizacao/revisao-e-merge.md).

Não integre alterações diretamente na branch principal.

Este repositório ainda não define comandos de build ou testes. Registre na PR as
validações executadas e justifique os itens que não se aplicarem à alteração.
