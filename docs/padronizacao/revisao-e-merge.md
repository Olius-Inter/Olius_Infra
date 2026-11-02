# Revisão e merge

Nenhuma PR pode ser integrada à branch principal sem cumprir todas as etapas
obrigatórias:

```text
PR → CI aprovado → Sonar / Quality Gate aprovado → CodeRabbit executado
   → Mínimo de uma aprovação humana → Merge
```

## Pull Request e CI

Toda alteração deve passar por PR; não é permitido push direto para integrar
alterações na branch principal.

O CI deve executar automaticamente as verificações definidas pelo projeto,
que podem incluir build, testes unitários, testes de integração e outras
validações. A falha de qualquer verificação obrigatória bloqueia o merge.

## Sonar

O Sonar deve analisar qualidade e segurança do código. A PR deve atender ao
Quality Gate definido pelo projeto. Quality Gate reprovado bloqueia o merge.

## CodeRabbit

A execução do CodeRabbit é obrigatória para auxiliar a revisão com análise das
alterações, identificação de possíveis problemas e sugestões de melhoria.

No fluxo do projeto, o CodeRabbit não aprova a PR, não solicita oficialmente
alterações, não realiza merge e não substitui o revisor humano.
Os apontamentos devem ser avaliados durante a revisão.

## Aprovação humana

Toda PR deve receber pelo menos uma aprovação humana antes do merge. O revisor
avalia a implementação, a aderência à tarefa, a arquitetura e as regras do projeto,
podendo aprovar ou solicitar alterações. A decisão final pertence à equipe.

## Checklist para integração

- [ ] PR preenchida com o template e referência da tarefa.
- [ ] Todas as verificações obrigatórias do CI aprovadas.
- [ ] Análise do Sonar concluída com Quality Gate aprovado.
- [ ] CodeRabbit executado e apontamentos avaliados na revisão.
- [ ] Problemas encontrados na revisão corrigidos.
- [ ] Pelo menos uma aprovação humana registrada.

## Configuração necessária no repositório

Para aplicar os bloqueios automaticamente, a administração deve configurar a
proteção da branch principal ou ruleset equivalente, exigir PR, pelo menos uma
aprovação humana e os checks obrigatórios de CI e Sonar, além de garantir a
execução do CodeRabbit.

Os nomes dos checks e os critérios do Quality Gate dependem das integrações
configuradas no projeto. Esta documentação não configura esses serviços.

[Voltar ao índice](README.md)
