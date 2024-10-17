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
    Permitir que os usuários consultem descrições detalhadas dos produtos disponíveis.
- RF2: Análise de sentimento dos produtos:  
    Realizar análise de sentimento nas avaliações dos produtos para identificar percepções positivas, negativas e neutras.
- RF3: Análise de avaliações dos produtos:  
    Oferecer insights sobre as avaliações dos produtos, incluindo médias e tendências ao longo do tempo.
- RF4: Análise de perfis de consumo por Idade e por Sexo:  
    Examinar padrões de consumo e preferências de produtos com base na faixa etária dos usuários e com o sexo dos usuários.
- RF5: Análise de Preferências por Região e por Categoria:  
    Consultar a variação nas escolhas de produtos com base na localização dos usuários e explorar as melhores opções em categorias específicas, com informações sobre os produtos mais vendidos e avaliações, auxiliando os clientes na tomada de decisões informadas na hora da compra.


<br>
 
> **Requisitos Não Funcionais**
- RNF1: BD Vetorial ChromaDB, FAISS ou outro
- RNF2: Modelos LLM de uso público do Huggingface
- RNF3: Framework Langchain
- RNF4: Vídeo-tutorial

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
| 2    | Alta      | Como usuário, quero que o sistema organize os dados de avaliações, associando-os a produtos específicos, para que eu possa ter uma visão estruturada das opiniões de consumidores. | 3 | 1      | RF1                  |
| 3    | Alta      | Como usuário, quero que o bot armazene informações de forma eficiente, para que o sistema seja rápido ao consultar e retornar dados quando solicitado. | 2 | 1      | RNF1                  |
| 4    | Média       | Como usuário, quero poder interagir com o bot fazendo perguntas sobre avaliações de produtos e receber respostas claras e diretas, baseadas nas opiniões dos clientes, para facilitar minha análise. | 5 | 2      | RF1                  |
| 5    | Média      | Como usuário, quero acessar o bot através de uma interface web amigável, onde posso digitar perguntas de forma simples e receber respostas naturais, para que minha experiência de uso seja fácil e eficiente. | 3 | 2      | RF3                  |
| 6    | Média       | Como usuário, quero que o bot consulte a base de dados de maneira rápida e me forneça informações precisas, para que eu possa tomar decisões sobre quais produtos merecem mais ou menos investimento. | 8 | 2      | RF2                  |
| 7    | Média      | Como usuário, quero que o bot combine as respostas com base nos dados armazenados para fornecer insights mais precisos sobre o desempenho de cada produto, para que eu tenha uma visão mais completa. | 2 | 2      | RF2                  |
| 8    | Baixa       | Como usuário, quero que o bot me forneça respostas rápidas e precisas com base em diferentes fontes de dados, independentemente do modelo de IA usado, para que eu confie nos resultados apresentados. | 5 | 3      | RF2                  |
| 9   | Baixa      | Como usuário, quero que o sistema seja ajustado com base nos feedbacks e nas interações reais, para que o bot evolua e forneça respostas mais consistentes e valiosas ao longo do tempo. | 3 | 3      | RF3                  |
| 10   | Baixa       | Como usuário, quero uma interface intuitiva e fácil de usar, com respostas organizadas e de fácil leitura, para que eu possa obter insights de forma prática e sem dificuldades técnicas. | 8 | 3      | RNF1                 |


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

<br>

  
## Equipe

<details>

<summary><strong>Equipe</strong></summary>

<span id="equipe">

  ## :clipboard: Scrum Team

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
