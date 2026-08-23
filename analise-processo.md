# Análise do Processo de Desenvolvimento - AgileTech Solutions

## 1. Análise do cenário

A AgileTech Solutions está começando um projeto em um contexto no qual os requisitos ainda não estão totalmente definidos e podem mudar com frequência. Além disso, a equipe é pequena, o cliente participa do processo, mas possui disponibilidade limitada, e existe pressão para que o produto gere valor rapidamente.

Considerando esse cenário, entendo que um processo ágil é mais adequado do que tentar definir todo o sistema antecipadamente. A equipe pode trabalhar com entregas menores, validar decisões ao longo do desenvolvimento e ajustar as prioridades conforme recebe feedback.

Essa forma de trabalhar também evita investir muito tempo detalhando funcionalidades que podem mudar antes mesmo de serem implementadas.

## 2. Os quatro valores do Manifesto Ágil

### Indivíduos e interações mais que processos e ferramentas

Em uma equipe com cinco desenvolvedores e um Product Owner, a comunicação tem bastante impacto no andamento do projeto. Ferramentas e processos continuam sendo importantes, mas não devem criar burocracia desnecessária.

Para a AgileTech, conversas objetivas entre desenvolvedores e Product Owner podem resolver dúvidas mais rapidamente do que depender somente de documentos extensos ou processos rígidos.

### Software em funcionamento mais que documentação abrangente

A empresa possui um histórico de documentação extensa que rapidamente ficava desatualizada. Nesse caso, considero mais importante concentrar esforço na entrega de software funcional.

Isso não significa abandonar a documentação. Informações necessárias para manutenção, decisões técnicas e utilização do sistema devem continuar sendo registradas. A diferença é evitar documentação criada apenas para cumprir etapas do processo e que não acompanha a evolução real do produto.

### Colaboração com o cliente mais que negociação de contratos

O cliente é participativo, mas possui disponibilidade limitada. Por isso, os momentos de contato precisam ser utilizados principalmente para validar prioridades, esclarecer requisitos importantes e avaliar os incrementos entregues.

Com ciclos curtos, o cliente não precisa definir todos os detalhes do produto no início. Ele pode avaliar o que já foi construído e ajudar a direcionar as próximas decisões.

### Responder a mudanças mais que seguir um plano

Esse valor é especialmente relevante para a AgileTech porque os requisitos são vagos e sujeitos a mudanças frequentes.

Um planejamento inicial continua sendo necessário, porém não deve impedir a equipe de adaptar o produto quando surgir uma mudança importante. Trabalhar com Sprints e entregas menores permite revisar prioridades sem precisar reconstruir um planejamento de longo prazo inteiro.

## 3. Por que utilizar uma abordagem ágil em vez de cascata

Em um processo em cascata, existe uma dependência maior da definição antecipada dos requisitos e da execução das etapas de maneira sequencial. Isso pode funcionar em contextos nos quais existe maior estabilidade e previsibilidade.

Na AgileTech acontece praticamente o contrário: os requisitos ainda são vagos, mudanças são esperadas e existe necessidade de demonstrar valor rapidamente.

Se a equipe passasse muito tempo levantando e documentando todos os requisitos antes de iniciar as entregas, parte desse trabalho poderia perder valor quando as necessidades mudassem.

Por isso, considero mais adequado trabalhar de maneira incremental. A equipe desenvolve uma parte do produto, apresenta o resultado, recebe feedback e utiliza o aprendizado obtido para orientar os próximos incrementos.

## 4. Práticas ágeis que adotaria inicialmente

### Sprints curtas

Utilizaria Sprints de duas semanas. Esse período permite criar um objetivo de curto prazo sem deixar a equipe muito tempo trabalhando sem validação.

### Daily Scrum

Uma reunião diária curta ajuda a equipe a compartilhar o que está sendo desenvolvido, identificar impedimentos e perceber dependências entre atividades.

Para uma equipe pequena, manteria essa reunião objetiva para que ela não se transforme em uma reunião longa de status.

### Code Review

Antes de considerar uma alteração concluída, outro desenvolvedor deve revisar o código. Além de ajudar na identificação de problemas, a revisão distribui conhecimento sobre diferentes partes do sistema.

### Integração contínua

Também adotaria integração frequente das alterações. Quanto menor o intervalo entre integrações, menor tende a ser a quantidade de conflitos acumulados e mais cedo alguns problemas podem ser identificados.

## 5. Programação em Pares

Pair programming, ou programação em pares, é uma prática associada ao XP na qual dois desenvolvedores trabalham juntos sobre o mesmo problema.

Tradicionalmente, um assume o papel de **driver**, escrevendo o código, enquanto o outro atua como **navigator**, acompanhando a implementação, analisando decisões e observando possíveis problemas. Esses papéis podem ser alternados durante a atividade.

Entre os benefícios estão a revisão de código acontecendo durante a implementação, a troca de conhecimento, a discussão das decisões técnicas e a possibilidade de identificar erros antes que eles avancem no processo.

## 6. Desafios da programação em pares no EAD

No contexto de um curso a distância, aplicar pair programming exatamente da forma presencial pode ser mais difícil.

Os participantes podem possuir horários diferentes, problemas de conexão e disponibilidade limitada. Também existe a dificuldade de manter duas pessoas conectadas durante períodos longos apenas para trabalhar sobre o mesmo código.

Outro ponto é que a comunicação remota pode ser menos natural. Em uma sala física, apontar um trecho do código ou trocar rapidamente quem está utilizando o computador é simples. Remotamente, isso depende das ferramentas utilizadas.

Por isso, considero que a prática pode ser mantida, mas precisa ser adaptada.

## 7. Adaptações para equipes remotas

### Pair programming remoto por compartilhamento de tela

Uma possibilidade é definir períodos específicos para programação em pares através de uma chamada com compartilhamento de tela.

Não seria necessário utilizar essa prática durante todo o desenvolvimento. Ela poderia ser reservada para funcionalidades mais complexas, investigação de bugs ou decisões técnicas importantes.

Os papéis de driver e navigator continuariam existindo e poderiam ser alternados durante a sessão.

### Desenvolvimento individual seguido de revisão colaborativa

Quando não for possível conciliar os horários, uma alternativa é trabalhar de maneira assíncrona.

Um desenvolvedor implementa uma pequena alteração e envia um Pull Request. Outro integrante revisa o código, registra comentários e discute as decisões antes da integração.

Essa alternativa não reproduz completamente a programação em pares, porque a colaboração não acontece simultaneamente, mas preserva parte importante da ideia: compartilhar conhecimento e evitar que uma implementação seja analisada somente pela pessoa que a escreveu.

## 8. Dificuldades essenciais de Brooks

Brooks apresenta quatro dificuldades essenciais relacionadas ao desenvolvimento de software: **complexidade, conformidade, mutabilidade e invisibilidade**.

Todas podem aparecer no desenvolvimento da AgileTech, mas considero que algumas possuem impacto mais direto no cenário apresentado.

### Complexidade

Conforme funcionalidades, regras e relações entre componentes são adicionadas, compreender o sistema se torna mais difícil.

Na AgileTech, essa dificuldade pode ser reduzida através de pequenas entregas, design simples, refatoração e revisão de código. A ideia é evitar adicionar complexidade antes que ela seja realmente necessária.

### Conformidade

O software precisa se adaptar a elementos externos, como regras do negócio, tecnologias, integrações e necessidades dos usuários.

Mesmo que a equipe tenha uma arquitetura bem definida, ela não controla todas essas condições. A comunicação frequente com o Product Owner e a validação incremental ajudam a identificar essas restrições antes que elas provoquem mudanças maiores.

### Mutabilidade

Considero a mutabilidade uma das dificuldades mais relevantes para este caso.

O software está sujeito a mudanças constantes porque as necessidades do negócio e dos usuários evoluem. O próprio cenário informa que os requisitos da AgileTech são vagos e mudam frequentemente.

Sprints curtas, backlog priorizado, refatoração e entregas incrementais permitem incorporar mudanças gradualmente, em vez de tratá-las como uma exceção ao planejamento.

### Invisibilidade

Software não possui uma representação física natural que permita observar facilmente toda sua estrutura e seu estado.

Uma maneira prática de reduzir parte dessa dificuldade é tornar o trabalho mais visível. O uso de um quadro Kanban permite que a equipe e o Product Owner observem quais atividades ainda estão pendentes, quais estão em desenvolvimento, quais estão em revisão e quais foram concluídas.

Essa representação não elimina a invisibilidade inerente ao software, mas melhora a visualização do processo de desenvolvimento.

## 9. Como os métodos ágeis ajudam a mitigar essas dificuldades

Os métodos ágeis não eliminam as dificuldades essenciais descritas por Brooks. O que eles podem fazer é reduzir parte do impacto delas sobre o projeto.

A complexidade pode ser controlada através de design simples, refatoração e desenvolvimento incremental. A conformidade pode ser tratada através de comunicação e validação frequentes. A mutabilidade é melhor absorvida quando o planejamento ocorre em ciclos curtos. Já a invisibilidade pode ser parcialmente reduzida com ferramentas visuais, incrementos demonstráveis e acompanhamento frequente do trabalho.

Para a AgileTech, considero especialmente importante evitar a tentativa de prever todo o produto desde o início. Como existe incerteza, trabalhar em ciclos menores permite que as decisões sejam tomadas com base no conhecimento disponível naquele momento e revisadas conforme o projeto evolui.

## Conclusão

A principal vantagem da abordagem ágil neste cenário não é simplesmente desenvolver mais rápido, mas conseguir aprender e adaptar o desenvolvimento sem perder completamente o trabalho já realizado.

A combinação de ciclos curtos, comunicação, revisão de código, integração contínua e participação do Product Owner cria um processo mais compatível com uma startup que ainda está descobrindo e refinando seu produto.

O planejamento continua existindo, assim como documentação e processos. A diferença é que eles passam a apoiar a entrega do software, em vez de se tornarem o objetivo principal do projeto.
