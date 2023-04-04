
<img src='/img/logo.png' alt='logo da empresa' width='50px' heidth='50px'/>

<<<<<<< HEAD
# *FIBONACCI MANAGEMENT SYSTEMs*
=======
# *FIBONACCI MANAGEMENT SYSTEMas*
>>>>>>> 006e91641d038e90d6d62a1fd9b63747c258819a

# PROJETO DE SOFTWARE

## *Stakeholders*
|Amara Liz Egler Cardoso|programadora|aammaaraalliizzx@gmail.com|
|Laís Amaro da Luz batista|Gerente de Projeto|laisamaroluz@gmail.com|
|Emylly Samylly César Gritti|Designer de Interface com o Usuário|cesaremylly@gmail.com|
|João Phelipe de Souza Barbosa|Analista de Requisitos|joaophelipesouza0516@gmail.com|
|Kauan Richard Moreira de Andrade|Analista de Testes|stokentin@gmail.com|

# Sumário

* [RESUMO DO PROJETO](#resumo-do-projeto)
* [INTRODUÇÃO](#introdução)
  * [PROPÓSITO DESTE DOCUMENTO](#propósito-deste-documento)
  * [ESCOPO DO PROJETO](#escopo-do-projeto)
  * [CONCEPÇÃO DO SISTEMA](#concepção-do-sistema)
  * [CONVENÇÕES, TERMOS E ABRIVEAÇÕES](#convenções-termos-e-abreviações)
* [DESCRIÇÃO GERAL](#descrição-geral)
  * [USUÁRIOS DO SISTEMA](#usuários-do-sistema)
  * [ABRANGÊNCIA E SISTEMAS SIMILARES](#abrangência-e-sistemas-similares)
  * [SUPOSIÇÕES E DEPENDÊNCIAS](#suposições-e-dependências)
* [ESTUDO DE VIABILIDADE](#estudo-de-viabilidade)
  * [VIABILIDADE TÉCNICA](#viabilidade-técnica)
  * [VIABILIDADE ECONÔMICA](#viabilidade-econômica)
  * [VIABILIDADE ORGANIZACIONAL](#viabilidade-organizacional)
* [METODOLOGIA ADOTADA NO DESENVOLVIMENTO](#metodologia-adotada-no-desenvolvimento)
* [REQUISITOS DO SOFTWARE](#requisitos-do-software)
  * [REQUISITOS FUNCIONAIS](#requisitos-funcionais)
  * [REQUISITOS NÃO FUNCIONAIS](#requisitos-não-funcionais)
* [PROTOTIPAGEM](#prototipagem)
* [DIAGRAMA DE CASOS DE USO](#diagrama-de-casos-de-uso)
  * [ESPECIFICAÇÃO DOS CASOS DE USO](#descrição--especificação-dos-casos-de-uso)
* [DIAGRAMA DE CLASSES](#diagrama-de-classes)
* [DIAGRAMA DE SEQUÊNCIAS](#diagrama-de-sequências)
* [ DIAGRAMA DE ATIVIDADES](#diagrama-de-atividades)
* [REFERÊNCIAS](#referências)


# RESUMO DO PROJETO
| ITEM | DESCRIÇÃO|
|:---|:---|
| NOME DO PROJETO | Fibonacci Management System |
| GERENTE DO PROJETO | Wagner Ferreira |
| PRINCIPAL OBJETIVO | Auxiliar o sistema de ensino através de ferramentas síncronas e assíncronas que serão usadas por funcionários e alunos da instituição de ensino. |
| BENEFÍCIOS ESPERADOS |* Melhor acompanhamento pedagógico;<br/>* Redução da evasão escolar;<br/>* Aumento do número de matrículas;<br/>* Redução da inadimplência escolar;<br/>* Automatização dos processos financeiross|
| INÍCIO E TÉRMINO PREVISTOS | 14/03/2023 - 07/12/2023 |

[ [INÍCIO](#fibonacci-management-system) ]

# INTRODUÇÃO

## PROPÓSITO DESTE DOCUMENTO

Este documento destina-se aos clientes, engenheiros, gerentes e demais stakeholders deste projeto. O propósito deste documento é apresentar a descrição dos serviços e funções que o sistema **_Fibonacci Management System_** deve prover, bem como as suas restrições de operação e propriedades gerais, a fim de ilustrar uma descrição detalhada do sistema para um auxílio durante as etapas de análise, projeto e testes. O documento especifica todos os requisitos funcionais e não funcionais do sistema e contém a prototipagem, além de diagramas UML que foram construídos levando-se em conta as funcionalidades identificadas durante a fase de concepção do sistema.

## CONCEPÇÃO DO SISTEMA

Foram usados três métodos para que pudessem ser obtidos os requisitos do sistema:
* Entrevista:
  * Discussões individuais de um representante da equipe com José de Arimatéia, diretor da Escola Fibonacci.
* Consulta com especialista:
  * Gustavo, coordenador de pós-graduação do curso de Ciências Contábeis da Universidade Federal orientou na concepção do sistema devido sua experiência em trabalhar em cursos semipresenciais e ser um dos consultores da empresa;
  * Alex Sandro Gomes, professor do Centro de Informática da Universidade Federal orientou na análise de requisitos devido a sua grande experiência em desenvolvimento de software educativo;
  * Silvio Zanchetti, coordenador do curso on-line ITUC/AL, foi outro entrevistado;
  * Manasses dos Santos Silva, responsável pelo treinamento dos funcionários do laboratório HEXAL BRASIL.
* Prototipação:
  * Representações das interfaces gráficas com diferentes níveis de fidelidade, aprovadas pela empresa contratante.



## CONVENÇÕES, TERMOS E ABREVIAÇÕES

Para evitar interpretações incorretas deste documento, algumas convenções e termos específicos são descritos a seguir:

* EaD: Eaducação a Distância
* Moodle: Ambiente Virtual que hospedará os cursos oferecidos
* Exame Final: Avaliação destinada aos estudantes que obtiveram média anual inferior à 60 pontos

[ [INÍCIO](#fibonacci-management-system) ]

# DESCRIÇÃO GERAL

## ESCOPO DO PROJETO

### NO ESCOPO

O projeto consiste na construção de uma ferramenta para gerenciamento de aprendizado *(Learning Management System - LMS)*, que possa atender os requisitos da Escola Fibonacci, no fator de educação à distância. O projeto visa auxiliar o sistema de ensino através de ferramentas síncronas e assíncronas que serão usadas por funcionários e alunos da instituição de ensino.
O escopo do **produto** pode ser consultado nos [requisitos do software](#requisitos-do-software)

### FORA DO ESCOPO

Não fazem parte do escopo do projeto:
* Instalação e configuração do ambiente tecnológico do cliente;
* Treinamento de instalação, configuração, administração e  utilização do sistema;
* Integração com quaisquer sistemas ou base de dados do ambiente tecnológico do cliente.

## Usuários do sistema
|USUÁRIO|DESCRIÇÃO|
|:---|:---|
|**Usuário Padrão:**|Realizam as tarefas comuns a todos os usuários, tal como: logar e enviar mensagens. Todos demais usuários estendem as funcionalidades do UsuárioPadrão|
|**Administrador:**|Responsáveis pelo gerenciamento das entidades pertinentes à instituição e pela alocação de outros administradores|
|**Coordenador:**|Responsáveis pela aprovação de disciplinas, turmas e matrículas realizadas pela secretaria do curso, além de ser responsável pela alocação da secretaria|
|**Secretaria:**|Responsáveis pelo cadastramento de disciplinas e turmas, pela alocação de professores e monitores de um curso e matrículas dos alunos|
|**Professor:**|Responsáveis pela criação do programa da disciplina através de ferramentas de planejamento e criação de atividades|
|**Aluno:**|Seguem o programa da disciplina criada pelo professor, tendo como apoio ferramentas de comunicação, tal como: chat e fórum|

## Abrangência e sistemas similares

### Abrangência:

O sistema irá conter ferramentas para construção de um plano de aulas que esteja de acordo com os objetivos e metodologia de uma turma ministrada pelo professor. O professor através de ferramentas (como Chat, Fórum, Base de Documentos) irá montar o programa desta disciplina que deverá ser seguido pelo aluno usuário do sistema. O professor terá a liberdade de criar atividades (textos e questionários) e determinar prazos a serem cumpridos pelos alunos. Serão armazenadas as resoluções dos alunos para serem corrigidas pelo professor posteriormente, gerando estatísticas do desempenho de cada aluno e da turma. O sistema também irá prover o gerenciamento das entidades que compõem a instituição e os usuários do sistema.

Dentre as ferramentas de comunicação do sistema existirão as assíncronas, como Chat, onde poderão ser feitas reuniões, discussões, explicações conjuntas ou qualquer outra atividade de comunicação. O Fórum consiste na ferramenta síncrona usada para os mesmos fins do Chat.

Das ferramentas de planejamento podemos citar:

* **Avaliações e Exercícios:** serão criadas tarefas a serem entregues pelos alunos nos determinados prazos;

* **Anúncios:** espaço para criação de avisos e informes aos alunos de uma determinada turma;

* **Manipulação de Arquivos:** haverá um diretório onde podem ser acumulados arquivos de diversos tipos pelos usuários;

* **Planejamento de Aulas:** planejamento de uma aula estruturada com leituras e exercícios.

### Sistemas similares:

No cenário atual da universidade se encontra um sistema que é responsável por realizar tal tarefa, denominado Virtus, porém o sistema não atende todas as necessidades, não sendo considerado satisfatório pela maioria dos usuários.

No cenário nacional encontram-se três sistemas que se destacam:

**AulaNet:** é um ambiente de software baseado na Web, desenvolvido no Laboratório de Engenharia de Software - LES - do Departamento de Informática da PUC-Rio, para administração, criação, manutenção e participação em cursos à distância.
WebAula: é um produto formado por soluções integradas de gerenciamento de aprendizagem, conhecimento e conteúdos on-line, resultado de uma joint venture entre as empresas Zargon e Poliedro.

**TelEduc:** é um ambiente para a criação, participação e administração de cursos na Web. Ele foi concebido tendo como alvo o processo de formação de professores para informática educativa, baseado na metodologia de formação contextualizada desenvolvida por pesquisadores do Nied (Núcleo de Informática Aplicada à Educação) da Unicamp.

No cenário internacional os sistemas de maior porte são:

**WebCT:** O WebCT é um programa que possibilita a criação de ambientes educacionais na Internet, desenvolvido pela University of British Columbia - Canadá. Ele permite a colocação do conteúdo de um curso na Internet pelo professor e, em seguida, o cadastro os alunos que participarão daquele curso. O objetivo principal é possibilitar a interação entre tais sujeitos através de ferramentas de trabalho em grupo, tais como: fóruns de discussão, chat, palestras on-line, além de facilitar a comunicação professor-aluno, através da publicação de notas e gabaritos de avaliações.

**Blackboard:** é um sistema de autoria extremamente amigável, desenvolvido para ser utilizado por educadores e profissionais interessados em aplicar as novas tecnologias interativas da rede na educação, contribuindo para a metodologia de ensino presencial e potencializando o processo de ensino e aprendizagem a distância.

## Suposições e dependências
O sistema necessita de um servidor web para sua hospedagem.

Os usuários devem utilizar um computador com a seguinte configuração mínima:

* Processador Dual Core 2GHz ou superior
* 2Gb de memória RAM
* 5Gb de armazenamento em disco
* Para uso do sistema é preciso ter instalado o Java SE versão 8 e o MySql versão 8.0.28.

# ESTUDO DE VIABILIDADE

Uma vez definidos a necessidade para o sistema e seus requisitos de negócio, é possível compreender melhor o projeto do sistema proposto para elaborar o estudo de viabilidade com os seguintes destaques:

## Viabilidade Técnica
Os colaboradores da empresa contratante possuem bastante experiência com aplicações desta natureza, os analistas também estão familiarizados com esta área de aplicação comercial, porém o sistema utiliza uma tecnologia nova, com a qual os analistas e programadores não estão familiarizados. No que se refere ao tamanho do sistema, trata-se de um projeto de médio porte, com baixo nível de complexidade, que não será integrado a outros sistemas, limitando-se a atender a demanda da escola no que se refere à EaD, que, atualmente possui 1.000 alunos matriculados. Conclui-se que o projeto possui viabilidade técnica, em virtude dos baixos riscos identificados.

## Viabilidade Econômica

Foi realizada uma análise de custo-benefício, e, mesmo com estimativas conservadoras do retorno sobre o investimento e dos benefícios totais, este projeto é viável economicamente. Após a implantação, espera-se uma melhoria na qualidade dos serviços prestados e aumento da capacidade de vagas da unidade escolar.

## Viabilidade Organizacional

Do ponto de vista organizacional, este projeto apresenta baixo risco. Os diretores e coordenadores da instituição demonstram forte interesse no projeto. Espera-se que os professores e alunos aprovem a implantação do sistema, visto que atualmente a escola não possui uma ferramenta específica para o controle das informações, o que está provocando enormes transtornos para a instituição.


[ [INÍCIO](#fibonacci-management-system) ]

# Metodologia Adotada no Desenvolvimento


[ [INÍCIO](#fibonacci-management-system) ]

# Requisitos do Software

A especificação dos requisitos deste documento deve seguir as recomendações da norma IEEE Std-830-1998, levando em conta as recomentações do documento de [características dos requisitos](caracteristicas_requisitos.md).

## Requisitos Funcionais

A tabela a seguir contém a relação dos Requisitos Funcionais elicitados, com as colunas: identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
:---|:---|:---|
|RF-001 |Nome do Requisito | Descreva aqui as informações sobre o requisito |
|RF-002 | Nome do Requisito | Descreva aqui as informações sobre o segundo requisito |


## Requisitos Não Funcionais
A tabela a seguir contém a relação com os Requisitos Não Funcionais identificados, contendo identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
|:---|:---|:---|
|RNF-001 |Nome do Requisito |Descreva aqui as informações sobre o requisito |
|RNF-002 |Nome do Requisito |Descreva aqui as informações sobre o segundo requisito |


[ [INÍCIO](#fibonacci-management-system) ]


# Prototipagem

[Protótipo criado no FIGMA em 2022 por estudantes](https://www.figma.com/file/iNC7wyX9zP7Kmn3BhiCFGf/Fals6Hood-(Prot%C3%B3tipo-criado-por-estudantes-em-2022)?node-id=0%3A1&t=B16hgeZP3MSURCCa-1)

![Imagem do Protótipo](/img/home.png)

[ [INÍCIO](#fibonacci-management-system) ]


# Diagrama de Casos de Uso


![Diagrama de Casos de Uso](/img/use_case_placas.png)

## Descrição / Especificação dos Casos de Uso

### UC-01 - Cadastrar Professor

|UC-01 - Cadastrar Professor|           
|:---|
|**Descrição/Objetivo:** Permite a inclusão de novos professores no Sistema|
|**Atores: Administrador**|
|**Pré-condições:** O usuário precisa estar cadastrado e logado|
|**Pós-condições:** Será apresentada uma mensagem confirmando a realização do cadastro|
|**FLUXO PRINCIPAL / BÁSICO:**|
|1. O usuário seleciona a opção cadastrar professor|
|2. Os dados do professor são inseridos|
|3. O usuário clica em salvar|
|4. Um novo ID é gerado |
|5. É apresentada uma mensagem confirmando a realização do cadastro|
|**FLUXOS ALTERNATIVOS / EXCESSÕES:** |
|**A1: Campo obrigatório não preenchido** |
|1. Uma mensagem será apresentada para o usuário, informando que existe(m) campos obrigatórios que não foram preenchidos |
|2. O cursor será posicionado no primeiro campo obrigatório que não foi preenchido |
|**A2: Data de nascimento inválida** |
|1. Uma mensagem será apresentada para o usuário, informando que a data informáda não é válida|
|2. O cursor será posicionado para o campo data|


## Matriz de Rastreabilidade


| REQUISITO |UC-01|UC-02|UC-03|UC-04|UC-05|UC-06|UC-07|UC-08|UC-09| UC-10|     
|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
|RF-001|X| | | | | | | | | |
|RF-002| |X| |X| | | | | | |

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Classes

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Sequências

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Atividades


# REFERÊNCIAS

Esta subseção apresenta as referências aos documentos que utilizamos no auxílio à construção deste documento.
* [UML](https://www.omg.org/spec/UML/2.5/About-UML/)
* [Práticas para Especificação de Requisitos IEEE-830](https://ieeexplore.ieee.org/document/720574)