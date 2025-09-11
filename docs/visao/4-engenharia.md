# 4 **Engenharia de Requisitos**

## 4.1 **Atividades e Técnicas de ER**

### **Elicitação e Descoberta**

Foca na **identificação e coleta** **inicial de requisitos** por meio da interação com stakeholders, usuários e outras fontes.

- **Entrevistas**: faremos entrevistas livres com os stakeholders para elicitação dos requisitos, utilizando técnicas como brainstorming e análise de tarefas.

- **Brainstorming**: será utilizada na reunião com os stakeholders ou entre os desenvolvedores.

- **Análise de Tarefas**: será utilizada para fazer a delimitação de tarefas/requisitos com os stakeholders e os desenvolvedores.

- **Introspecção**: será utilizada para elicitar requisitos de acordo com o que os desenvolvedores esperam para a solução a ser desenvolvida.

---

### **Análise e Consenso**

Envolve o **refinamento e a consolidação** dos requisitos elicitados. Busca-se eliminar ambiguidades, resolver conflitos, priorizar e garantir que os requisitos sejam completos, consistentes e **alinhados com os objetivos do negócio**.

- **Entrevistas**: para garantir consentimento entre partes interessadas do projeto acerca dos requisitos da solução.

- **Negociação**: será utilizada nas entrevistas para chegar a um acordo sobre os requisitos.

- **Análise de Custo/Benefício**: será utilizada para chegar a um acordo sobre os requisitos com os stakeholders e os desenvolvedores.

---

### **Declaração de Requisitos**

É a **documentação formal** dos requisitos analisados, utilizando linguagem clara e estruturada. O foco é especificar "o quê" o sistema deve fazer, garantindo rastreabilidade.

- **User Stories**: Será utilizada a técnica de narrativas de usuários (user stories), que descrevem **funcionalidades sob a perspectiva do usuário**.

- **Documento de Visão de Produto**: documento de visão para declarar os requisitos e disponibilizar para a equipe e o cliente.

---

### **Representação de Requisitos**

Foca na **modelagem visual ou textual** dos requisitos para facilitar o entendimento e a comunicação.

- **Prototipação**: A técnica de representação informal prototipação será utilizada para permitir às partes interessadas fornecer feedbacks intermediários.

---

### **Verificação e Validação de Requisitos**

Garante a **qualidade dos requisitos**. A verificação assegura que os requisitos estão **corretamente especificados** (completos, não ambíguos), enquanto a validação confere se **atendem às reais necessidades** do cliente.

1. **Definition of Ready (DoR):** A técnica de DoR delimita quando um requisito está preparado para ser trabalhado. Para que seja considerado como Ready, serão levadas em consideração se:

   1. O requisito está representado por uma história de usuário?

   2. O requisito possui critérios de aceitação orientados por *Behavior Driven Development (BDD)* e testes?

   3. O requisito está consoante com a granularidade dos demais?

   4. O requisito foi estimado?

   5. O requisito agrega valor e está associado a algum dos objetivos específicos da solução?

   6. As dependências do requisitos estão mapeadas (se houver)?

2. **Definition of Done (DoD):** A técnica de DoD demonstra qualidade do requisito produzido. Para que seja considerado como Done, deve atender ao seguinte:

   1. Entrega de Valor

      1. O trabalho realizado entrega um incremento funcional e observável ao produto?

      2. A entrega está claramente rastreada à sua origem? (A descrição do Pull Request ou da tarefa cita a US, RN ou O.E. correspondente?)

   2. Cobertura dos Requisitos

      1. Todos os cenários (sucesso, falha e alternativos) descritos nos Critérios de Aceite (*Behavior Driven Development*) foram implementados e são demonstráveis?

   3. Qualidade de Testes

      1. Foi criado o teste unitário necessário para a nova funcionalidade?

      2. Os fluxos principais foram validados manualmente em um ambiente de teste, confirmando o comportamento esperado?

   4. Revisão por Pares (Code Review)

      1. O Pull Request (PR) foi revisado e aprovado por, pelo menos, um outro membro da equipe?

      2. A revisão de código validou os critérios essenciais?

         1. Conformidade: O código segue os padrões estabelecidos?

         2. Lógica: A implementação atende corretamente aos requisitos?

         3. Legibilidade: O código é claro, bem nomeado e de fácil manutenção?

         4. Segurança: Não há dados sensíveis (senhas, tokens) expostos no código?

   5. Padrões de Código

      1. O código segue os padrões de codificação e o guia de estilo definidos pelo projeto, utilizando a extensão Conventional Commits do Visual Studio Code?

      2. A extensão Ruff do Visual Studio Code foi executada e não aponta erros?

   6. Documentação

      1. A documentação técnica foi devidamente atualizada? (Ex: README.md, comentários em lógicas complexas, novas variáveis de ambiente).

3. **Feedback**: Será utilizada a técnica de feedback com as partes interessadas para manter um backlog de produto verificado e validado de acordo com as necessidades da solução.

---

### **Organização e Atualização de Requisitos**

Garante que o backlog e os requisitos da solução estejam organizados e devidamente atualizados conforme o andamento do projeto.

- **MoSCoW**: será utilizada a técnica de priorização de requisitos MoSCoW (Must Have, Should Have, Could Have, Won't Have), com objetivo de gerar o **Produto Mínimo Viável** (MVP).

- **Matriz de priorização**: Foi utilizada a técnica matriz de priorização para definir os requisitos do MVP, considerando esforço técnico e MoSCoW.

- **Feedback**: Conforme o feedback do cliente, os requisitos foram sendo atualizados, para garantir entregas de valor.

---

## 4.2 **Engenharia de Requisitos e o Kanban/XP**

| Fase do Fluxo (Kanban) | Atividades ER                      | Prática                                                                       | Técnica                                                                                                             | Resultado Esperado                                                                                        |
| :--------------------- | :--------------------------------- | :---------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------------- |
| Backlog                | Elicitação e Descoberta            | Coleta contínua de ideias e necessidades.                                     | Brainstorming, Análise de feedback, PBB (Product Backlog Building).                                                 | Lista de funcionalidades e necessidades em alto nível, aguardando análise.                                |
| Análise / Refinamento  | Análise e Consenso                 | Priorização e detalhamento dos requisitos.                                    | Priorização (ICE, MoSCoW, Matriz de Valor vs. Esforço), Story Mapping, Escrita de User Story.                       | Backlog ordenado por prioridade; itens mais altos na lista são detalhados.                                |
|                        | Declaração de Requisitos           | Definição clara do que precisa ser feito.                                     | User Stories com Critérios de Aceitação (Ex: formato Gherkin), Definição de Preparado (DoR \- Definition of Ready). | Histórias de usuário bem definidas, com escopo claro e prontas para serem puxadas para o desenvolvimento. |
|                        | Verificação e Validação (Inicial)  | Garantia de que a história de usuário entrega valor.                          | Revisão da história (pelo outro membro da equipe), Prototipagem/Mockups.                                            | Confirmação de que o requisito é valioso e compreendido por todos antes do desenvolvimento.               |
| Em Desenvolvimento     | Representação de Requisitos        | Orientação visual e técnica para a equipe.                                    | Storyboards, Diagramas de fluxo, TDD (Test-Driven Development).                                                     | Código sendo desenvolvido com um guia claro sobre o comportamento esperado da funcionalidade.             |
|                        | Verificação e Validação (Contínua) | Garantia de que a implementação está correta.                                 | Pair Programming (Programação em Par), Revisão de Código (Code Review).                                             | Incremento de software que atende aos critérios da história e aos padrões de qualidade.                   |
| Teste / Validação      | Verificação e Validação (Final)    | Confirmação de que o requisito foi atendido.                                  | Execução de testes de aceitação (manuais ou automatizados), Revisão informal da funcionalidade.                     | Funcionalidade implementada confirmada como correta e aderente aos critérios de aceitação.                |
|                        |                                    | Verificação dos critérios de "Pronto".                                        | Checklist de Definição de Pronto (DoD \- Definition of Done).                                                       | Garantia de que todos os passos de qualidade foram cumpridos antes da entrega.                            |
| Concluído              | Organização e Atualização          | Manutenção do backlog com base no trabalho finalizado e no feedback recebido. | Atualização do backlog (adição de novas ideias, ajuste de prioridades).                                             | Backlog reflete o estado atual do projeto e os aprendizados do desenvolvimento.                           |
|                        | Validação (Pós-entrega)            | Obtenção de feedback sobre a funcionalidade entregue.                         | Apresentação assíncrona (vídeo, ambiente de homologação), Coleta de feedback do cliente/usuário.                    | Funcionalidade validada em uso real, gerando insights para o backlog.                                     |

<font size="3"><p style="text-align: center"> Fonte: Elaborado pelos autores ([João Marcos](https://github.com/JJOAOMARCOSS) e [Christopher](https://github.com/wChrstphr), 2025)</p></font>

---

## Historico de Versão
| Data       | Versão | Descrição                                     | Autor(es)   | Revisor(es) |
| ---------- | ------ | --------------------------------------------- | ----------- | ----------- |
| 07/08/2025 | 1.0    | Desafios de Projeto e Segmentação de Clientes | João Marcos | Christopher |