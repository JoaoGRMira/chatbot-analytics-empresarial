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

<span id="projeto">
  
## :clipboard: O Projeto

> **Status do Projeto: Em andamento** 

- O projeto consiste no desenvolvimento de um chatbot baseado em Inteligência Artificial generativa, voltado para a análise de dados comerciais e feedbacks de clientes. O principal objetivo é facilitar a interpretação dos dados qualitativos (comentários e depoimentos de consumidores) sem a necessidade de utilizar dashboards complexos ou gráficos. O chatbot será capaz de responder perguntas específicas sobre o desempenho de produtos e a opinião dos consumidores, oferecendo respostas em linguagem natural e de forma clara, objetiva e direta.

<br>

<span id="proposta">
  
## :dart: Proposta

**Requisitos Funcionais**
- RF1: Consulta de descrições de produtos:  
    - Permitir que os usuários consultem descrições detalhadas dos produtos disponíveis.
- RF2: Análise de sentimento dos produtos:  
    - Realizar análise de sentimento nas avaliações dos produtos para identificar percepções positivas, negativas e neutras.
- RF3: Análise de avaliações dos produtos:  
    - Oferecer insights sobre as avaliações dos produtos, incluindo médias e tendências ao longo do tempo.
- RF4: Análise de perfis de consumo por Idade e por Sexo:  
    - Examinar padrões de consumo e preferências de produtos com base na faixa etária dos usuários e com o sexo dos usuários.
- RF5: Análise de Preferências por Região e por Categoria:  
    - Consultar a variação nas escolhas de produtos com base na localização dos usuários e explorar as melhores opções em categorias específicas, com informações sobre os produtos mais vendidos e avaliações, auxiliando os clientes na tomada de decisões informadas na hora da compra.


<br>
 
> **Requisitos Não Funcionais**
- RNF1 - BD Vetorial ChromaDB 
- RNF2 - Modelos LLM: llama3-8b-8192 - LLM de geração de texto, sentence-transformers/all-MiniLM-L6-v2 - LLM para geração de embeddings 
- RNF3 - Framework Langchain 
- RNF4 - Vídeo-tutorial 

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

| Rank | Prioridade | User Story                                                                                                                                                                                                                                                                     | Estimativa (Planning Poker) | Sprint | Requisito do Parceiro |
| ---- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------- | ------ | --------------------- |
| 1    | Alta       | Como gerente de analytics, quero que o chatbot organize os dados de avaliações, associando-os a produtos específicos, para que eu possa ter uma visão estruturada das opiniões dos consumidores e assim possa criar estratégias sobre quais produtos devo investir.            | 5                           | 1      | RF3                   |
| 2    | Alta       | Como gerente de analytics, quero interagir com o chatbot com perguntas relacionadas a avaliações de produtos e receber respostas claras e diretas, baseadas nas reviews dos clientes, para diminuir o tempo gasto com análises manuais.                                        | 3                           | 1      | RF3, RNF2             |
| 3    | Alta       | Como gerente de analytics, quero que o chatbot seja treinado com base nos dados de reviews armazenados para fornecer insights precisos sobre o desempenho dos produtos, para que eu tenha uma visão estratégica de quais medidas tomar com base nas opiniões dos consumidores. | 2                           | 1      | RF3, RNF1             |
| 4    | Média      | Como gerente de analytics, quero que o chatbot entenda e processe os comentários dos clientes para gerar análises relevantes, para que eu possa avaliar a opinião geral sobre um produto e tomar decisões administrativas sobre eles.                                          | 5                           | 2      | RF2                   |
| 5    | Média      | Como gerente de analytics, quero que o chatbot seja ágil e preciso na hora de fornecer respostas para que eu receba resultados confiáveis sobre os produtos avaliados.                                                                                                         | 3                           | 2      | RNF1, RNF2            |
| 6    | Baixa      | Como gerente de analytics, quero acessar o chatbot através de uma interface web amigável, onde posso digitar perguntas sobre produtos de forma simples e receber respostas naturais relacionadas às avaliações.                                                                | 8                           | 3      | RF3, RNF3             |
| 7    | Baixa      | Como gerente de analytics, quero que o chatbot examine padrões de consumo e preferências de produtos com base na faixa etária e sexo dos usuários.                                                                                                                             | 2                           | 3      | RF4                   |
| 8    | Baixa      | Como gerente de analytics, quero consultar a variação nas escolhas de produtos por região e categoria, fornecendo informações sobre os produtos mais vendidos e avaliados para ajudar na tomada de decisões.                                                                   | 5                           | 3      | RF5                   |


<br>

<span id="sprints">
  
## :rocket: Entrega das Sprints

<details>
  <summary><strong> Sprint 1 </strong></summary>

  ## :dart: MVP
  Nesta sprint, focamos em entregar o MVP do nosso chatbot, permitindo consultas diretas sobre as avaliações de produtos da base de dados do Hugging Face. 

  <br>

  ## :dart: DoR + Critérios de Aceitação
  **USER STORY 1**
  - **Descrição:** Como usuário do sistema, quero que o bot entenda e processe os comentários dos clientes para gerar relatórios relevantes, para que eu possa avaliar a opinião geral sobre um produto.
  - **Critérios de Aceitação:**
    - O bot deve processar comentários de clientes automaticamente.
    - Relatórios gerados devem ser legíveis e organizados.
    - Suporte a diferentes formatos de comentários.
    - Relatórios devem refletir a opinião geral sobre o produto.

  <br>
  
   **USER STORY 2**
  - **Descrição:** Como usuário, quero que o sistema organize os dados de avaliações de maneira clara, associando-os a produtos específicos, para que eu possa ter uma visão estruturada das opiniões de consumidores.
  - **Critérios de Aceitação:**
    - O sistema deve categorizar as avaliações por produto.
    - Os dados devem ser estruturados e fáceis de acessar.
    - Deve ser possível associar múltiplas avaliações a um produto em um painel.

  <br>
  
  **USER STORY 3**
  - **Descrição:** Como usuário, quero que o bot armazene informações de forma eficiente, para que o sistema seja rápido ao consultar e retornar dados quando solicitado.
  - **Critérios de Aceitação:**
    - O sistema deve armazenar informações de forma eficiente.
    - O tempo de resposta ao consultar dados deve ser inferior a 2 segundos.
    - Os dados armazenados devem ser recuperados sem perda.

  <br>
  
  ## :dart: Entrega
  [Clique aqui e assista ao vídeo da entrega no YouTube](https://www.youtube.com/watch?v=dKhNMwNdgP8&t=16s)

  <br>

</details>

<br>

<details>
  <summary><strong> Sprint 2 </strong></summary>

  ## :dart: MVP
  ... 

  <br>
  
  ## :dart: Entrega
  [Clique aqui e assista ao vídeo da entrega no YouTube]()

  <br>

</details>



<br>

 
## 👥 Scrum Team

<details>

<summary><strong>Membros</strong></summary>

<span id="equipe">

<br>

| Nome                   | Função         | GitHub                                                                    |
| ---------------------- | -------------- | ------------------------------------------------------------------------- |
| **Thiago Bueno**       | Scrum Master   | [![](https://bit.ly/3f9Xo0P)](https://github.com/TjBueno)                 |
| **Elisa Carvalho**     | Product Owner  | [![](https://bit.ly/3f9Xo0P)](https://github.com/elisadsc)                |
| **Rebeca Gama**        | Developer Team | [![](https://bit.ly/3f9Xo0P)](https://github.com/RebecaGama)              |
| **João Gabriel**       | Developer Team | [![](https://bit.ly/3f9Xo0P)](https://github.com/JoaoGRMira)              |
| **Diane Alves**        | Developer Team | [![](https://bit.ly/3f9Xo0P)](https://github.com/Diane-Moreno)            |
| **Rita Hecht**         | Developer Team | [![](https://bit.ly/3f9Xo0P)](https://github.com/ritahecht)               |
| **Nicholas Guilherme** | Developer Team | [![](https://bit.ly/3f9Xo0P)](https://github.com/NicholasGui29)           |
| **Víctor Henrique**    | Developer Team | [![](https://bit.ly/3f9Xo0P)](https://github.com/ViktorHenrique)          |
</details>
<br>
<details>
  <summary><strong>:page_facing_up: Estrutura do Código</strong></summary>
<br>  
<span id="gitflow">
  
## :chart_with_upwards_trend: Gitflow
 

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

 <img src="https://github.com/atomofatec/API-DOMROCK/blob/main/img/gitflow.png">

<br>

<br>

<span id="estrutura-branch">
  
## :bookmark_tabs: Estrutura da branch
 

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
  
## :black_nib: Padrões de commit
 

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

</details>



<details>

<summary><strong>:page_facing_up: DoR </strong></summary>

## :white_check_mark: (Definition of Ready - DoR)
<br>

**Para que uma tarefa seja considerada pronta para ser desenvolvida, ela deve atender aos seguintes critérios:**
  
1. Documentação Completa:
   - Requisitos funcionais e não-funcionais devem estar documentados e acessíveis. 
   - Especificações técnicas e de design devem estar detalhadas. 
2. História de Usuário Validada: 
   - Cada tarefa deve estar vinculada a uma história de usuário específica (exemplo: backlog do produto), com a descrição do problema que resolve e o benefício para o usuário final. 
3. Dependências Identificadas: 
   - Todas as dependências com outras tarefas, ferramentas ou recursos devem estar mapeadas e resolvidas. 
4. Design e Layout Definidos: 
   - Para tarefas relacionadas à interface, o design deve estar aprovado e disponível. 
5. Alinhamento com a Sprint: 
   - A tarefa deve estar dentro do escopo da sprint (Sprint 2) e estar de acordo com as prioridades estabelecidas (urgente, alta, normal, baixa). 
6. Estimativa de Tempo: 
   - A tarefa deve ter uma estimativa de tempo de desenvolvimento e testes definida pela equipe. 
</details>

<br>

 
