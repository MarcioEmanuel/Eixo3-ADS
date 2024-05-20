# Especificações do Projeto

<span style="color:red">Pré-requisitos:<a href="01-Documentação de Contexto.md"> Documentação de Contexto</a></span>

O aplicativo será desenvolvido como um aplicativo móvel utilizando o framework React Native, permitindo a compatibilidade com dispositivos iOS e Android. O uso de React Native garantirá uma experiência de usuário consistente e fluída em diferentes dispositivos móveis.
O aplicativo será composto por diversos módulos principais:

•	Cadastro de Usuários: Os usuários poderão se cadastrar no aplicativo para acessar todas as funcionalidades oferecidas.
•	Cálculo Simples: Este módulo permitirá aos usuários inserir os valores disponibilizados pelo fatiador, como comprimento utilizado, área do diâmetro do filamento, diâmetro do filamento, peso estimado e tempo de impressão.

•	Valores de Produção: Aqui, os usuários poderão inserir as despesas de produção, como o tipo de filamento, valor do quilo, preço por kWh, consumo da máquina, depreciação por hora e média de falhas.

•	Retorno de Investimento: Este módulo calculará o tempo necessário para o retorno do investimento com base no valor da máquina, horas de operação diárias, dias de operação por mês e valor a ser adicionado por hora.

•	Custos de Produção: Neste módulo, serão calculados os custos de material, energia, manutenção, falhas, acabamento e fixação (spray).

•	Custos Diversos: Aqui, serão calculados os custos diversos, incluindo o retorno de investimento e outros custos adicionais.

•	Resultado: Por fim, o módulo de resultado apresentará o valor de produção, a porcentagem de lucro, o valor de venda sugerido e a margem de lucro.

Este projeto será desenvolvido com foco na usabilidade, precisão e eficiência, visando proporcionar uma ferramenta completa e indispensável para usuários envolvidos no mundo da impressão 3D.

## Personas

1 - Engenheiro Entusiasta - Rafael Silva:
Rafael é um entusiasta de impressão 3D que é apaixonado por tecnologia e engenharia. Ele adora explorar novos materiais e técnicas de impressão 3D para criar protótipos e projetos pessoais.
Rafael passa muito tempo pesquisando e experimentando diferentes configurações de impressão 3D. Ele está interessado em entender os detalhes técnicos por trás do processo de produção.
Ele deseja um aplicativo que ofereça uma análise detalhada dos custos de produção, incluindo o consumo de filamentos e energia, para otimizar seus projetos e reduzir os custos.

2 - Designer Freelancer - Ana Souza:
Ana é uma designer freelancer que utiliza a impressão 3D como parte integrante de seu trabalho. Ela cria modelos 3D para clientes em uma variedade de setores, desde produtos de consumo até protótipos industriais.
Ana trabalha em diversos projetos simultaneamente e precisa gerenciar prazos apertados. Ela valoriza a eficiência e a precisão em seus processos de trabalho.
Ela procura por um aplicativo que simplifique o cálculo dos custos de produção, oferecendo estimativas precisas e rápidas para incorporar em suas propostas de projeto. Além disso, ela precisa de recursos de acompanhamento de tempo para monitorar o tempo gasto em cada projeto.

3 - Empreendedor Iniciante - Lucas Oliveira:
Lucas é um empreendedor que está começando um pequeno negócio de produtos personalizados feitos em impressora 3D. Ele está animado para transformar suas ideias em produtos tangíveis e lucrativos.
Lucas possui habilidades básicas de design e impressão 3D, mas está aprendendo rapidamente. Ele está sempre em busca de orientação e recursos para aprimorar suas habilidades e expandir seu negócio.
Ele busca um aplicativo intuitivo e fácil de usar que forneça uma visão abrangente dos custos envolvidos na produção de seus produtos. Ele valoriza recursos educacionais e suporte ao cliente para ajudá-lo a resolver desafios específicos relacionados à impressão 3D e ao gerenciamento de custos.

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto.

### Requisitos Funcionais

| ID     | Descrição do Requisito  | Prioridade |
|--------|-----------------------------------------|----|
| RF - 001 | Cadastro de Usuários: Permitir registro com nome, e-mail e senha. | ALTA | 
| RF-002 | Cálculo de Custos de Produção:Permitir inserção de custos de materiais, energia, mão de obra, etc. Opções de moedas e unidades. | ALTA |
| RF-003 | Cálculo de Retorno de Investimento (ROI): Inserir custo inicial e recorrente para calcular tempo de retorno. Considerar depreciação e desgaste dos equipamentos. | ALTA |
| RF-004 | Cálculo de Valores de Venda: Permitir determinação de preços com base em custos e ROI. Fornecer orientações sobre preços competitivos. | ALTA |
| RF-005 | Interface Intuitiva: Interface amigável e adaptada para dispositivos móveis. Facilidade de navegação e entrada de dados. | MEDIO |


### Requisitos não Funcionais

|ID     | Descrição do Requisito  | Prioridade |
|-------|-------------------------|----|
|RNF-001| Segurança: Garantir segurança de dados com criptografia e autenticação. Conformidade com regulamentações de privacidade. | ALTA | 
|RNF-002| Desempenho: Responsividade rápida, com carregamento mínimo. Capacidade de lidar com carga de usuários sem degradação significativa. |  MÉDIA | 
|RNF-003| Compatibilidade: Compatibilidade com diferentes dispositivos e sistemas operacionais. Testes em várias resoluções para experiência consistente. |  MÉDIA | 
|RNF-004| Disponibilidade: Acesso contínuo, com tempo de inatividade mínimo. |  MÉDIA | 
|RNF-005| Precisão dos Cálculos: Garantir precisão e confiabilidade nos resultados. |  ALTA |

## Histórias de Usuários

Com base na análise das personas forma identificadas as seguintes histórias de usuários:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Rafael Silva | análise detalhada dos custos de produção | otimizar seus projetos e reduzir os custos |
|Ana Souza | aplicativo que simplifique o cálculo dos custos de produção| Monitorar tempo e custo  de produção |
|Lucas Oliveira|aplicativo intuitivo e fácil de usar| gerenciamento de custos |

## Modelagem do Processo de Negócio 

### Análise da Situação Atual

Com a popularização da impressora 3d muitos entusiastas começaram a comprar a sua própria, deixando assim de ser um produto voltado aos distribuidores e empresas á algo que possa ser usado por qualquer pessoa. Mesmo sendo para uso pessoal há a necessidade de calcular gastos, sejam eles com materiais ou energia no geral. Por ser um mercado relativamente novo, não existe aplicativos intuitivos ao público-geral que possam auxiliar aqueles com carência de conhecimento nesses calculos que demandão conhecimento mais aprofundado. Nosso aplicativo foca em ajudar a todos nesse meio, possibilitando praticidade e o principal de tudo, cálculos precisos e corretos.

### Descrição Geral da Proposta

Nossa proposta é bem clara, buscamos possibilitar a todos ter ciência sobre os custos finais de cada produção de sua impressora 3d. Esse dados variam claramente de usuário para usuário que terá que manualmente inserir os dados de custos locais, como kiloWatts por hora (energia), valor do material e dados gerais de custos do modelo de sua impressora.

### Processo 1 – COLETANEA DE DADOS LOCAIS DO USUÁRIO

Temos como meta criar uma padronização para esses dados sensíveis, criando assim uma padronização com templates de modelos de impressoras, gastos por empresas de energia, ou padrão de materiais baseados em banco de dados de lojas afiliadas. O proceso inicial demanda que o usuário tenha conhecimento sobre seus gastos em materiais, gasto de energia por hora de sua impressora e quanto é cobrado o kWs pela empresa de energia responável por sua residência.

![Processo 1](img/DADOS-USUÁRIO.png)

### Processo 2 – INPUT DE DADOS E ALTERAÇÃO DE DADOS

Buscar uma forma de auto completar os dados do usuário, com base em outros dados fornecidos consientemente por outros usuários, assim buscando agilizar o trabalho manual. O processo é necessário, seria ele o que faz o aplicativo funcionar da forma que deveria é possível tambem alterar esses dados a qualquyer momento, assim buscando diferentes resultados.

![Processo 2](img/INPUT-REVISAO-DADOS.png)

### Processo 3 – RESULTADOS

Solicitar ao usuário que compartilhasse os resultados e dados para que possamos melhorar nossa tecnologia. Mostra o resultados dos dados inseridos anteriormente.

![Processo 2](img/RESULTADOS.png)

## Indicadores de Desempenho

![Indicadores de Desempenho](img/INDICADORES-DE-DESEMPENHO.png)

Obs.: todas as informações para gerar os indicadores devem estar no diagrama de classe a ser apresentado a posteriori.

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto deverá ser entregue até o final do semestre |
|02| Não pode ser desenvolvido um módulo de backend        |

## Diagrama de Casos de Uso

![Indicadores de Desempenho](img/DIAGRAMA-CLASSES-DE-USO.png)

# Matriz de Rastreabilidade

| Requisitos                          | Cadastro de Usuários | Cálculo de Custos de Custo | Cálculo de ROI | Cálculo de Valores de Venda | Interface Intuitiva |
|-------------------------------------|-----------------------|---------------------------------|------------------|------------------------------|---------------------|
| RF-001: Cadastro de Usuários       |          X            |   X                              |  X                |     X                         |         X            |
| RF-002: Cálculo de Custos          |                       |                X                |         X         |               X               |                     |
| RF-003: Cálculo de ROI             |                       |                 X                |         X        |                X              |                     |
| RF-004: Cálculo de Valores de Venda |                       |               X                  |       X           |              X              |                     |
| RF-005: Interface Intuitiva         |                       |                                 |                  |                              |         X         |




# Gerenciamento de Projeto

De acordo com o PMBoK v6 as dez áreas que constituem os pilares para gerenciar projetos, e que caracterizam a multidisciplinaridade envolvida, são: Integração, Escopo, Cronograma (Tempo), Custos, Qualidade, Recursos, Comunicações, Riscos, Aquisições, Partes Interessadas. Para desenvolver projetos um profissional deve se preocupar em gerenciar todas essas dez áreas. Elas se complementam e se relacionam, de tal forma que não se deve apenas examinar uma área de forma estanque. É preciso considerar, por exemplo, que as áreas de Escopo, Cronograma e Custos estão muito relacionadas. Assim, se eu amplio o escopo de um projeto eu posso afetar seu cronograma e seus custos.

## Gerenciamento de Tempo

Com diagramas bem organizados que permitem gerenciar o tempo nos projetos, o gerente de projetos agenda e coordena tarefas dentro de um projeto para estimar o tempo necessário de conclusão.

![Diagrama de rede simplificado notação francesa (método francês)](img/02-diagrama-rede-simplificado.png)

O gráfico de Gantt ou diagrama de Gantt também é uma ferramenta visual utilizada para controlar e gerenciar o cronograma de atividades de um projeto. Com ele, é possível listar tudo que precisa ser feito para colocar o projeto em prática, dividir em atividades e estimar o tempo necessário para executá-las.

![Gráfico de Gantt](img/02-grafico-gantt.png)

## Gerenciamento de Equipe

O gerenciamento adequado de tarefas contribuirá para que o projeto alcance altos níveis de produtividade. Por isso, é fundamental que ocorra a gestão de tarefas e de pessoas, de modo que os times envolvidos no projeto possam ser facilmente gerenciados. 

![Simple Project Timeline](img/02-project-timeline.png)

## Gestão de Orçamento

| Recursos                    |        R$         |
|----------------------------------------------------------|-----------------------------------------------------|
| Tempo dos Alunos            |       0,00        |
| Acesso a Tecnologia         |       0,00        |
| Conhecimento dos Alunos     |       0,00        |
| Supervisão dos Professores  |       0,00        |
| Feedback de Usuários        |       0,00        |
| **TOTAL**                   |    **0,00**      |
