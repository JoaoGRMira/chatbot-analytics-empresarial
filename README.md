# API-DOMROCK

<h1 align="center">API 6º Semestre 2024-2 - Equipe Átomo</h1>

<p align="center">
  <a href ="#projeto"> Projeto </a>  •
  <a href ="#proposta"> Proposta </a>  • 
  <a href ="#prototipo"> Protótipo </a>  • 
  <a href ="#backlogs"> Backlog do Produto </a> • 
  <a href ="#sprints">Sprints</a> •
  <a href ="#equipe">Equipe</a> 
  

<br>

<span id="estrutura-branch">
  
## :clipboard: Estrutura da branch
 

  **Introdução ao Gitflow**
    
  O Gitflow é um modelo escalável de gerenciamento de branches para projetos Git. Ele é amplamente utilizado em desenvolvimento de software para gerenciar diferentes linhas de desenvolvimento, tornando os processos de release mais claros e gerenciáveis.
  
  **Branches Principais**
  - **Master:** A branch master armazena o código oficial de release do projeto. Toda nova versão consolidada e testada é mergeada nessa branch e, posteriormente, taggeada com uma versão.
  - **Develop:** A branch develop serve como uma branch de integração para features. Ela contém o estado mais recente das mudanças destinadas à próxima release.
  
  **Branches de Suporte**
  - **Feature:** Branches feature são criadas a partir da branch develop. Cada branch feature é destinada ao desenvolvimento de uma funcionalidade específica ou correções e são mergeadas de volta à develop quando a funcionalidade está completa.
  - **Release:** Branches release são criadas a partir da branch develop. Estas branches são preparações para uma nova release de produção. Permitem ajustes finais e correções de bugs que não são enviadas à branch develop durante esse período. Quando a release está pronta para ser lançada, ela é mergeada em master e develop.
  - **Hotfix:** Branches hotfix são criadas a partir da branch master. São usadas para correções rápidas em releases de produção. Uma vez completadas, elas são mergeadas tanto em master quanto em develop para garantir que as correções sejam integradas em futuras releases.
  
  **Fluxo de Trabalho**
  - **Desenvolvimento de Features:**
  Inicia-se criando uma branch feature a partir de develop.
  Após a conclusão da feature, realiza-se um pull request para a develop.
  - **Preparação de Release:**
  Cria-se uma branch release a partir de develop.
  Realizam-se testes e ajustes necessários.
  Conclui-se mergeando a release em master e também de volta à develop com incremento de versão.
  - **Correções de Hotfix:**
  Identificado um bug em produção, cria-se uma branch hotfix a partir de master.
  Após a correção, o hotfix é mergeado em master e em develop.
  
  **Tags**
  
  Após uma release ser mergeada em master, uma tag de versão é criada para documentar o ponto de release no histórico do projeto.

<br>

<br>

<span id="estrutura-branch">
  
## :clipboard: Estrutura da branch
 

    Todas as branches que introduzem novas funcionalidades ao projeto devem seguir a estrutura:

    feature/[descricao-da-feature (nome da task)]
    
    Componentes:
      Prefixo "feature/": Indica que a branch está relacionada ao desenvolvimento de uma nova funcionalidade.
      Descrição da Feature: Um nome curto e descritivo, com palavras separadas por traços ("-"). A descrição deve ser clara e indicar a finalidade da branch.
    
    Exemplos:
      feature/criacao-dashboard
      feature/integracao-api-pagamento
      feature/melhoria-performance
    
    OBS: A nomeação do pull request terá que seguir o mesmo padrão da criação da branch.

<br>

<br>

<span id="padroes-commit">
  
## :clipboard: Padrões de commit
 

    Estrutura do Commit:
      <Sprint X> <tipo>: <descrição curta da mudança>
      <Sprint X>: Refere-se ao número da sprint em que a mudança foi implementada.
          Exemplos:  <Sprint I>, <Sprint II>.
  
    <tipo>: Indica o tipo de mudança realizada. 
          Exemplos:
            feat: Adição de uma nova funcionalidade.
            fix: Correção de bugs ou erros.
            chore: Tarefas de manutenção (como atualizações de dependências).
            refactor: Refatoração de código sem alteração de funcionalidade.
  
    <descrição>: Uma breve descrição da mudança realizada.
          Exemplos:
            <Sprint I> feat: adicionar funcionalidade de pesquisa
            <Sprint II> fix: corrigir erro no cálculo de frete
            <Sprint III> chore: atualizar dependências do projeto

<br>

<br>

<span id="projeto">
  
## :clipboard: O Projeto

> **Status do Projeto: Em andamento** 

- Desenvolver um chat bot baseado em IA generativa para que possa receber perguntas, buscar a resposta na base de dados de comentários de clientes e apresentar na forma de linguagem natural.

<br>

<span id="proposta">
  
## :dart: Proposta

> **Requisitos Funcionais**
- Desenvolver um pipeline de processamento de dados para banco de vetor;
- Desenvolver um agente para engenharia de prompt em LLM;
- Desenvolver uma interface de chatbot integrado com agente de LLM

<br>
 
> **Requisitos Não Funcionais**
- Um vídeo tutorial para demonstrar como usar para usuários que não tem domínio 
de tecnologia.

<br>

<span id="prototipo">
  
## :bulb: Protótipo

**:link: Clique no link abaixo para visualizar o modelo do projeto.**  
> [Protótipo do Projeto](https://www.figma.com/design/B490w2vCnTEs1Prt3qC2bE/API-6?node-id=1902-502433&node-type=CANVAS)

<br>

<span id="backlogs">
  
## 🗓️ Backlog do Produto

<span id="backlog-do-produto">

<br> 

| Rank | Prioridade | User Story | Estimativa (Planning Poker) | Sprint | Requisito do Parceiro |
|------|------------|----------------------------------------|--------------------------------|--------|-----------------------|
| 1    | Alta       | Como usuário do sistema, quero que o bot entenda e processe os comentários dos clientes para gerar relatórios relevantes, para que eu possa avaliar a opinião geral sobre um produto. | 5 | 1      | RF1                  |
| 2    | Alta      | Como usuário, quero que o sistema organize os dados de avaliações de maneira clara, associando-os a produtos específicos, para que eu possa ter uma visão estruturada das opiniões de consumidores. | 3 | 1      | RF1                  |
| 3    | Alta       | Como usuário, quero que o bot utilize inteligência artificial para entender a satisfação dos clientes com base nas avaliações e me forneça insights concisos sobre o feedback, para que eu possa tomar decisões mais informadas. | 8 | 1      | RF2                  |
| 4    | Alta      | Como usuário, quero que o bot armazene informações de forma eficiente, para que o sistema seja rápido ao consultar e retornar dados quando solicitado. | 2 | 1      | RF3                  |
| 5    | Média       | Como usuário, quero poder interagir com o bot fazendo perguntas sobre avaliações de produtos e receber respostas claras e diretas, baseadas nas opiniões dos clientes, para facilitar minha análise. | 5 | 2      | RF1                  |
| 6    | Média      | Como usuário, quero acessar o bot através de uma interface web amigável, onde posso digitar perguntas de forma simples e receber respostas naturais, para que minha experiência de uso seja fácil e eficiente. | 3 | 2      | RF3                  |
| 7    | Média       | Como usuário, quero que o bot consulte a base de dados de maneira rápida e me forneça informações precisas, para que eu possa tomar decisões sobre quais produtos merecem mais ou menos investimento. | 8 | 2      | RF1                  |
| 8    | Média      | Como usuário, quero que o bot combine as respostas com base nos dados armazenados para fornecer insights mais precisos sobre o desempenho de cada produto, para que eu tenha uma visão mais completa. | 2 | 2      | RF2                  |
| 9    | Baixa       | Como usuário, quero que o bot me forneça respostas rápidas e precisas com base em diferentes fontes de dados, independentemente do modelo de IA usado, para que eu confie nos resultados apresentados. | 5 | 3      | RF2                  |
| 10   | Baixa      | Como usuário, quero que o sistema seja ajustado com base nos feedbacks e nas interações reais, para que o bot evolua e forneça respostas mais consistentes e valiosas ao longo do tempo. | 3 | 3      | RF3                  |
| 11   | Baixa       | Como usuário, quero uma interface intuitiva e fácil de usar, com respostas organizadas e de fácil leitura, para que eu possa obter insights de forma prática e sem dificuldades técnicas. | 8 | 3      | RNF1                 |


<br>

<span id="sprints">
  
## :rocket: Sprint 1

<details>
  <summary><strong>:page_facing_up: Sprint 1 - Detalhes</strong></summary>

  <br>

  ## :pushpin: Critérios de Aceitação

  ## User Story 1
  - **Descrição:** Como usuário do sistema, quero que o bot entenda e processe os comentários dos clientes para gerar relatórios relevantes, para que eu possa avaliar a opinião geral sobre um produto.
  - **Critérios de Aceitação:**
    - O bot deve processar comentários de clientes automaticamente.
    - Relatórios gerados devem ser legíveis e organizados.
    - Suporte a diferentes formatos de comentários.
    - Relatórios devem refletir a opinião geral sobre o produto.

  ## User Story 2
  - **Descrição:** Como usuário, quero que o sistema organize os dados de avaliações de maneira clara, associando-os a produtos específicos, para que eu possa ter uma visão estruturada das opiniões de consumidores.
  - **Critérios de Aceitação:**
    - O sistema deve categorizar as avaliações por produto.
    - Os dados devem ser estruturados e fáceis de acessar.
    - Deve ser possível associar múltiplas avaliações a um produto em um painel.

  ## User Story 3
  - **Descrição:** Como usuário, quero que o bot utilize inteligência artificial para entender a satisfação dos clientes com base nas avaliações e me forneça insights concisos sobre o feedback, para que eu possa tomar decisões mais informadas.
  - **Critérios de Aceitação:**
    - O bot deve usar IA para interpretar a satisfação dos clientes.
    - O sistema deve fornecer insights concisos e acionáveis.
    - A IA deve evitar respostas imprecisas.

  ## User Story 4
  - **Descrição:** Como usuário, quero que o bot armazene informações de forma eficiente, para que o sistema seja rápido ao consultar e retornar dados quando solicitado.
  - **Critérios de Aceitação:**
    - O sistema deve armazenar informações de forma eficiente.
    - O tempo de resposta ao consultar dados deve ser inferior a 2 segundos.
    - Os dados armazenados devem ser recuperados sem perda.

  <br>

  ## Backlog - Sprint 1

  - **User Story 1:** 5 pontos (Prioridade: Alta)
  - **User Story 2:** 3 pontos (Prioridade: Média)
  - **User Story 3:** 8 pontos (Prioridade: Alta)


</details>



<br>

<details>
<span id="equipe">

  ## :clipboard: Equipe

<br>

|Nome|Função|GitHub|
| -------- |-------- |-------- |
|**Thiago Bueno**|Scrum Master|[![](https://bit.ly/3f9Xo0P)](https://github.com/TjBueno)|
|**Elisa Carvalho**|Product Owner|[![](https://bit.ly/3f9Xo0P)](https://github.com/elisadsc)|
|**Rebeca Gama**|Developer Team|[![](https://bit.ly/3f9Xo0P)](https://github.com/RebecaGama)|
|**João Gabriel**|Developer Team|[![](https://bit.ly/3f9Xo0P)](https://github.com/JoaoGRMira)|
|**Diane Alves**|Developer Team|[![](https://bit.ly/3f9Xo0P)](https://github.com/Diane-Moreno)|
|**Rita Hecht**|Developer Team|[![](https://bit.ly/3f9Xo0P)](https://github.com/ritahecht)|
|**Nicholas Guilherme**|Developer Team|[![](https://bit.ly/3f9Xo0P)](https://github.com/NicholasGui29)|
|**Víctor Henrique**|Developer Team|[![](https://bit.ly/3f9Xo0P)](https://github.com/ViktorHenrique)|
|**William da Silva**|Developer Team|[![](https://bit.ly/3f9Xo0P)](https://github.com/William2819/William2819)|
</details>
<br>
