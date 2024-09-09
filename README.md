# API-DOMROCK

<h1 align="center">API 6º Semestre 2024-2 - Equipe Átomo</h1>

<p align="center">
  <a href ="#projeto"> Projeto </a>  •
  <a href ="#proposta"> Proposta </a>  • 
  <a href ="#prototipo"> Protótipo </a>  • 
  <a href ="#backlogs"> Backlog do Produto </a> • 
  <a href ="#equipe">Equipe</a>
    <!--
  <a href ="#stories"> User Stories </a>  •
  <a href ="#bpmn"> BPMN </a>  
  <br>
  <a href ="#modelagem-banco"> Modelagem do Banco de Dados </a>  •
  <a href ="#documentos"> Documentação do Projeto </a>  •
  <a href ="#review">Sprint Reviews</a>  •  --!>
  
</p>

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
| 2    | Média      | Como usuário, quero que o sistema organize os dados de avaliações de maneira clara, associando-os a produtos específicos, para que eu possa ter uma visão estruturada das opiniões de consumidores. | 3 | 1      | RF1                  |
| 3    | Alta       | Como usuário, quero que o bot utilize inteligência artificial para entender a satisfação dos clientes com base nas avaliações e me forneça insights concisos sobre o feedback, para que eu possa tomar decisões mais informadas. | 8 | 1      | RF2                  |
| 4    | Baixa      | Como usuário, quero que o bot armazene informações de forma eficiente, para que o sistema seja rápido ao consultar e retornar dados quando solicitado. | 2 | 1      | RF3                  |
| 5    | Alta       | Como usuário, quero poder interagir com o bot fazendo perguntas sobre avaliações de produtos e receber respostas claras e diretas, baseadas nas opiniões dos clientes, para facilitar minha análise. | 5 | 2      | RF1                  |
| 6    | Média      | Como usuário, quero acessar o bot através de uma interface web amigável, onde posso digitar perguntas de forma simples e receber respostas naturais, para que minha experiência de uso seja fácil e eficiente. | 3 pontos | 2      | RF3                  |
| 7    | Alta       | Como usuário, quero que o bot consulte a base de dados de maneira rápida e me forneça informações precisas, para que eu possa tomar decisões sobre quais produtos merecem mais ou menos investimento. | 8 | 2      | RF1                  |
| 8    | Baixa      | Como usuário, quero que o bot combine as respostas com base nos dados armazenados para fornecer insights mais precisos sobre o desempenho de cada produto, para que eu tenha uma visão mais completa. | 2 | 2      | RF2                  |
| 9    | Alta       | Como usuário, quero que o bot me forneça respostas rápidas e precisas com base em diferentes fontes de dados, independentemente do modelo de IA usado, para que eu confie nos resultados apresentados. | 5 | 3      | RF2                  |
| 10   | Média      | Como usuário, quero que o sistema seja ajustado com base nos feedbacks e nas interações reais, para que o bot evolua e forneça respostas mais consistentes e valiosas ao longo do tempo. | 3 | 3      | RF3                  |
| 11   | Alta       | Como usuário, quero uma interface intuitiva e fácil de usar, com respostas organizadas e de fácil leitura, para que eu possa obter insights de forma prática e sem dificuldades técnicas. | 8 | 3      | RNF1                 |


<br>



# :rocket: Sprint 1

<details>
  <summary><strong>:page_facing_up: Sprint 1 - Detalhes</strong></summary>

  <br>

  <details>
    <summary><strong>Critérios de Aceitação</strong></summary>

    <br>

    <table>
      <tr>
        <th>User Story</th>
        <th>Critérios de Aceitação</th>
      </tr>
      <tr>
        <td><strong>User Story 1</strong></td>
        <td>- O bot deve processar comentários de clientes automaticamente.<br>- Relatórios gerados devem ser legíveis e organizados.<br>- Suporte a diferentes formatos de comentários.<br>- Relatórios devem refletir a opinião geral sobre o produto.</td>
      </tr>
      <tr>
        <td><strong>User Story 2</strong></td>
        <td>- Sistema deve categorizar avaliações por produto.<br>- Dados estruturados e fáceis de acessar.<br>- Múltiplas avaliações associadas a produtos em um painel.</td>
      </tr>
      <tr>
        <td><strong>User Story 3</strong></td>
        <td>- O bot deve usar IA para interpretar satisfação dos clientes.<br>- Sistema deve fornecer insights concisos.<br>- IA deve evitar respostas imprecisas.</td>
      </tr>
      <tr>
        <td><strong>User Story 4</strong></td>
        <td>- Sistema deve armazenar informações de forma eficiente.<br>- Tempo de resposta ao consultar dados: inferior a 2 segundos.<br>- Dados armazenados devem ser recuperados sem perda.</td>
      </tr>
    </table>

  </details>

  <br>

  <details>
    <summary><strong>Backlog - Sprint 1</strong></summary>

    <br>

    <table>
      <tr>
        <th>Rank</th>
        <th>User Story</th>
        <th>Estimativa</th>
        <th>Sprint</th>
      </tr>
      <tr>
        <td>1</td>
        <td>User Story 1</td>
        <td>5 pontos</td>
        <td>1</td>
      </tr>
      <tr>
        <td>2</td>
        <td>User Story 2</td>
        <td>3 pontos</td>
        <td>1</td>
      </tr>
      <tr>
        <td>3</td>
        <td>User Story 3</td>
        <td>8 pontos</td>
        <td>1</td>
      </tr>
    </table>

  </details>

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
