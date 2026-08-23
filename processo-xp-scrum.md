# Processo de Desenvolvimento com XP e Scrum

## 1. Organização do processo

Para o desenvolvimento do sistema da AgileTech Solutions, optei por combinar Scrum, XP e Kanban. Entendo que cada um resolve uma parte diferente do problema: o Scrum ajuda a organizar as entregas e os ciclos de trabalho, o XP traz práticas técnicas para o desenvolvimento do software e o Kanban permite visualizar de forma simples o andamento das atividades.

Essa combinação também se aproxima de situações que encontro em projetos de desenvolvimento de software, principalmente quando existe a necessidade de organizar tarefas, revisar código e entregar funcionalidades de forma incremental.

## 2. Quadro Kanban

Criei um quadro no GitHub Projects para representar o fluxo de desenvolvimento da Sprint.

O quadro foi dividido nas seguintes etapas:

- **Todo:** atividades que ainda não foram iniciadas;
- **In Progress:** atividades que estão sendo desenvolvidas;
- **Review:** funcionalidades que passaram pelo desenvolvimento e aguardam revisão;
- **Done:** atividades concluídas.

Foram adicionadas ao quadro as seguintes user stories:

1. Como usuário, quero me cadastrar no sistema para acessar a plataforma.
2. Como usuário, quero fazer login para acessar meus projetos.
3. Como usuário, quero criar um novo projeto para organizar meu trabalho.
4. Como usuário, quero adicionar tarefas a um projeto para acompanhar as atividades.
5. Como usuário, quero visualizar o andamento das tarefas para acompanhar o progresso do projeto.

### Link do GitHub Project

https://github.com/users/Mterra64/projects/4

## 3. Práticas de XP adotadas

### Programação em pares

A programação em pares pode ser utilizada principalmente em funcionalidades mais críticas ou que apresentem maior complexidade. Enquanto um desenvolvedor implementa a solução, o outro acompanha o raciocínio e revisa o código. Em uma equipe remota, isso pode ser feito através do compartilhamento de tela e de ferramentas de comunicação.

### Integração contínua

As alterações devem ser integradas frequentemente ao repositório. Isso reduz o risco de grandes conflitos e permite identificar problemas mais cedo durante o desenvolvimento.

### Refatoração

O código deve ser melhorado continuamente sempre que houver oportunidade de simplificá-lo, sem alterar seu comportamento esperado. A intenção é evitar que pequenas soluções provisórias se transformem em uma base difícil de manter.

### Design simples

A equipe deve implementar a solução mais simples capaz de atender aos requisitos atuais. Funcionalidades que talvez sejam necessárias no futuro não devem aumentar a complexidade do código antes de existir uma necessidade concreta.

### Pequenas entregas

Em vez de concentrar muitas funcionalidades em uma única entrega, o sistema deve evoluir através de incrementos menores. Dessa forma, o Product Owner consegue acompanhar o resultado e fornecer feedback ao longo do desenvolvimento.

### Propriedade coletiva do código

Embora cada pessoa possa trabalhar em tarefas diferentes, o código pertence à equipe. Qualquer desenvolvedor pode propor melhorias ou corrigir problemas, desde que siga os padrões definidos e o processo de revisão.

## 4. Integração entre XP e Scrum

O Scrum será utilizado para organizar o trabalho em Sprints de duas semanas. No início da Sprint, a equipe seleciona as histórias prioritárias junto ao Product Owner e define o objetivo da entrega.

Durante o desenvolvimento dessas histórias, entram as práticas do XP. Programação em pares pode ser utilizada em pontos mais complexos, refatoração e design simples orientam a implementação e a integração contínua mantém as alterações atualizadas no repositório.

O Kanban funciona como uma visão operacional desse processo. Uma história começa em `Todo`, passa para `In Progress` quando o desenvolvimento começa, segue para `Review` quando está pronta para revisão e termina em `Done` após ser considerada concluída.

Assim, considero que Scrum e XP não competem entre si. O Scrum organiza o processo e as entregas, enquanto o XP contribui principalmente para a forma como o software é construído.

## 5. Fluxo de trabalho semanal

A Sprint possui duração de duas semanas.

No início da primeira semana é realizado o Sprint Planning, no qual o Product Owner apresenta as prioridades e a equipe define quais histórias serão trabalhadas.

Durante a Sprint são realizadas reuniões Daily curtas para acompanhar o andamento das atividades e identificar impedimentos. O quadro Kanban é atualizado conforme o trabalho avança.

Durante o desenvolvimento são aplicadas práticas de XP, como design simples, programação em pares quando necessária, integração contínua e refatoração.

Antes de uma funcionalidade ser considerada concluída, ela passa pela etapa de Review. Essa etapa representa a revisão técnica do trabalho realizado e ajuda a manter a qualidade do código.

Ao final da segunda semana são realizadas a Sprint Review e a Sprint Retrospective. Na Review, o incremento é apresentado e o Product Owner pode fornecer feedback. Na Retrospective, a equipe analisa o próprio processo e identifica melhorias para a próxima Sprint.

## 6. Cronograma da Sprint de duas semanas

| Momento | Atividade | Duração aproximada | Participantes | Práticas relacionadas |
|---|---|---:|---|---|
| Dia 1 | Sprint Planning | 2 horas | Product Owner e desenvolvedores | Planejamento e pequenas entregas |
| Dias 2 a 5 | Desenvolvimento | Durante o dia | Desenvolvedores | Design simples, pair programming, refatoração e integração contínua |
| Dias 2 a 10 | Daily Scrum | 15 minutos | Equipe de desenvolvimento | Acompanhamento e identificação de impedimentos |
| Dia 5 | Verificação do andamento da Sprint | 30 minutos | Equipe | Revisão do quadro e integração contínua |
| Dias 6 a 9 | Continuação do desenvolvimento e revisão | Durante o dia | Desenvolvedores | Pair programming, refatoração, revisão e integração contínua |
| Dia 10 | Sprint Review | 1 hora | Product Owner e desenvolvedores | Apresentação do incremento e feedback |
| Dia 10 | Sprint Retrospective | 45 minutos | Equipe | Análise do processo e definição de melhorias |

## 7. Entregas esperadas

Ao final da Sprint, espera-se possuir um incremento funcional do sistema com as histórias priorizadas concluídas ou em condição de serem demonstradas.

Para esta Sprint, as entregas estão relacionadas às funcionalidades iniciais de acesso e gerenciamento de projetos, como cadastro, autenticação e início da organização das atividades do usuário.

Também é esperado que o código esteja integrado ao repositório, revisado e suficientemente simples para permitir evolução nas próximas Sprints.

## 8. Scrum x Kanban

| Aspecto | Scrum | Kanban |
|---|---|---|
| Organização | Trabalho dividido em Sprints | Fluxo contínuo de trabalho |
| Planejamento | Realizado principalmente no início da Sprint | Pode ocorrer continuamente |
| Papéis | Define responsabilidades como Product Owner, Scrum Master e Developers | Não exige papéis específicos |
| Mudanças | Normalmente evita mudanças que comprometam o objetivo durante a Sprint | Permite repriorização mais contínua |
| Acompanhamento | Sprint Backlog e eventos do Scrum | Visualização das atividades em um quadro |
| Limite de trabalho | Relacionado à capacidade e ao planejamento da Sprint | Pode utilizar limites explícitos de trabalho em progresso (WIP) |
| Quando usar | Quando existe benefício em trabalhar com ciclos e objetivos definidos | Quando existe necessidade de acompanhar e otimizar um fluxo contínuo |
| Combinação | Scrum pode organizar os ciclos de entrega | Kanban pode visualizar o fluxo das atividades dentro da Sprint |

## 9. Considerações finais

Para o cenário da AgileTech Solutions, considero adequada a combinação das três abordagens. O Scrum fornece uma estrutura para planejamento, acompanhamento e entrega. O XP complementa esse processo com práticas diretamente ligadas à construção e qualidade do software. O Kanban torna o estado das atividades visível para toda a equipe.

Essa estrutura também permite adaptação. Como os requisitos podem mudar, trabalhar com ciclos curtos e entregas menores reduz o impacto dessas mudanças e permite que o feedback do cliente seja incorporado nas próximas decisões de desenvolvimento.
