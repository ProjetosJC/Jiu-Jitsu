# 2 Solução Proposta

## 2.1 **Objetivos do Produto**

Nossa solução visa automatizar o processo de entrada e saída de membros da Gracie Barra, gerando dados valiosos para o negócio como: quantidade de alunos, professores e aulas registradas e frequência dos membros. Para além disso, temos por objetivo melhorar a visão geral do gestor sobre o negócio por meio de relatórios semanais e mensais. A ferramenta será voltada para:

1. Realizar a gestão de membros da academia;

2. Automatizar o registro de entrada e saída de alunos e professores;

3. Gerar relatórios semanais e mensais de frequência;

Os itens acima concatenam nos seguintes **Objetivos Específicos (O.E)**:

1. **Facilitar o gerenciamento da empresa;**

2. **Facilitar a gestão de aulas e alunos, trazendo profissionalismo ao negócio;**

3. **Reduzir a perda de informações.**

   

## 2.2 **Características da Solução**

As caractéristicas da solução proposta, até o momento, incluem:

- Reconhecimento facial integrado ao controlador Intelbras

- Cadastro completo de alunos e professores

- Registro automático de presença

- Sistema de graduações com histórico e certificados

- Dashboard com estatísticas de frequência

- Painel para exibição em TV com nomes de presentes e próxima aula

- Exportação de dados e relatórios em PDF, Excel e CSV

## 2.3 **Tecnologias a Serem Utilizadas**

### **Backend**

   - Python (FastAPI ou Django)

### **Frontend**

   - HTML5/CSS3/JavaScript e React.js

### **Banco de Dados**

   - PostgreSQL

### **Integração**

   - Intelbras SDK \- Protocolo nativo SS 3542 MF W

   - TCP/IP Protocol \- Comunicação com controlador

   - WebSocket \- Eventos em tempo real

   - REST API \- Integração externa

### **Deploy**

   - Docker \+ Hospedagem, com possibilidade de rodar em servidor local

### **DevOps**

   - Docker, GitHub Actions \- CI/CD

   - Nginx \- Proxy reverso (opcional)

---

## 2.4 **Pesquisa de Mercado e Análise Competitiva**

### Análise do Mercado

No mercado atual, existem soluções genéricas de controle de acesso e sistemas de gestão de academias, mas poucos são voltados especificamente para as academias de Jiu-Jitsu. As soluções concorrentes costumam ser caras, complexas ou não atendem às necessidades específicas desse nicho, sendo somente para controle de entrada/saída.

Nossa solução visa atender as necessidades específicas do nicho de Jiu-Jitsu, proporcionando controle sobre frequência do aluno, progressão de faixas de acordo com a quantidade de aulas ministradas e atendidas, descrição da aula que está sendo ministrada no momento, assim como qual o docente responsável e os alunos participantes naquele horário. Além disso, uma análise dos dados coletados será feita semanalmente para auxiliar na gestão.

## 2.5 **Análise de Viabilidade**

**Viabilidade Técnica:** O projeto é tecnicamente viável, pois a integração com o controlador facial Intelbras SS 3542 MF W pode ser realizada por meio de comunicação via rede local. As tecnologias a serem utilizadas (Python, React, PostgreSQL) são bem documentadas e de fácil manutenção.

**Viabilidade de Prazo:** Considerando um desenvolvimento incremental, com entregas quinzenais em sprints, o MVP pode ser entregue em até X meses, com incrementos contínuos até Y meses para o sistema completo.

**Viabilidade Financeira:** A solução utiliza ferramentas open source, e o time de desenvolvimento será composto por dois graduandos de Engenharia de Software voluntários, o que reduz drasticamente o custo. O hardware já está adquirido, restando apenas o investimento de tempo para aprendizado, desenvolvimento, teste e integração.

**Viabilidade de Mercado:** O sistema atende uma demanda real e recorrente de academias de artes marciais, com possibilidade de personalização para outras unidades e esportes, o que abre portas para reuso e expansão comercial.

## 2.6 **Impacto da Solução**

A solução trará maior organização, confiabilidade nos registros de presença e redução de tarefas manuais. Permitirá decisões estratégicas baseadas em dados, aumento da profissionalização da academia e melhor experiência para alunos e professores. Além disso, também reduzirá significativamente a carga mental de trabalho relacionada a trabalhos operacionais.

---

## Historico de Versão
| Data       | Versão | Descrição                                     | Autor(es)   | Revisor(es) |
| ---------- | ------ | --------------------------------------------- | ----------- | ----------- |
| 07/08/2025 | 1.0    | Desafios de Projeto e Segmentação de Clientes | João Marcos | Christopher |