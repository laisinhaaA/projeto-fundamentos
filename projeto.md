
<img src='/img/logo.png' alt='logo da empresa' width='50px' heidth='50px'/>

# *LA CHEF*

# PROJETO DE SOFTWARE

## *Stakeholders*
|NOME|CARGO|E-MAIL|
|:---|:---|:---|
|Amara Liz Egler Cardoso|Programadora|aammaaraalliizzx@gmail.com|
|Laís Amaro da Luz|Gerente de Projeto|laisamaroluz@gmail.com|
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
| NOME DO PROJETO | LA CHEF RESTAURANT |
| GERENTE DO PROJETO | Laís Amaro da Luz |
| PRINCIPAL OBJETIVO | Apresentação e avaliação das empresas filiadas espalhadas pela França |
| BENEFÍCIOS ESPERADOS |* Acompanhamento do feedback dos clientes;<br/>* Satisfação dos clientes;<br/>* Melhorias abdicadas por meio dos feedbacks;<br/>* Divulgação do restaurante;<br/> |
| INÍCIO E TÉRMINO PREVISTOS | 14/03/2023 - 07/12/2023 |

[ [INÍCIO](#la-chef-restaurant) ]

# INTRODUÇÃO

## PROPÓSITO DESTE DOCUMENTO

Este documento destina-se aos clientes, engenheiros, gerentes e demais stakeholders deste projeto. O propósito deste documento é apresentar a descrição dos serviços e funções que o sistema **_La Chef Restaurant_** deve prover, bem como as suas restrições de operação e propriedades gerais, a fim de ilustrar uma descrição detalhada do sistema para um auxílio durante as etapas de análise, projeto e testes. O documento especifica todos os requisitos funcionais e não funcionais do sistema e contém a prototipagem, além de diagramas UML que foram construídos levando-se em conta as funcionalidades identificadas durante a fase de concepção do sistema.

## CONCEPÇÃO DO SISTEMA

Para que fosse obtido os requisitos que a empresa desejava foram utilizados os seguintes métodos:
* Entrevista:
  * Foram realizadas reuniões e discussões com um representante da equipe e com representantes da equipe do restaurante La Chef.
* Consulta com especialista:
  * Wagner da Silva Ferreira Filho que atualmente é professor no IFRO Campus Vilhena. Possui graduação em Tecnologia em Sistemas de Informação - Faculdade de Tecnologia do Vale do Araguaia, especialização em Ciência da Computação - Faculdades Unidas do Vale do Araguaia. Orientação devido suas experiência nas áreas de Tecnologia da Informação e Sistemas Operacionais;
  * Bruno Rover Dal Prá, atualmente é professor no IFRO Campus Vilhena, possui graduação em Engenharia da Computação pela Universidade Tuiuti do Paraná, mestrado em Desenvolvimento de Tecnologia pelo LACTEC (Instituto de Tecnologia para o Desenvolvimento). Orientação devido sua experiência em programação de computadores, desenvolvimento de tecnologia e gestão da tecnologia, e banco de dados;
  * Valeria Arenhart, Orientação nas áreas de empreendedorismo.
* Prototipação:
  * Representações das interfaces gráficas com diferentes níveis de fidelidade, aprovadas pela empresa contratante.



## CONVENÇÕES, TERMOS E ABREVIAÇÕES

Para evitar interpretações incorretas deste documento, algumas convenções e termos específicos são descritos a seguir:

* IFRO: Instituto Federal de Rondônia;
* UML: Linguagem de Modelagem Unificada;
* Site: Local na internet identificado por um nome de domínio.

[ [INÍCIO](#fibonacci-management-system) ]

# DESCRIÇÃO GERAL

## ESCOPO DO PROJETO

### NO ESCOPO

O projeto tem como proposta a elaboração de um site para a avaliação de pratos de comida que o restaurante ‘La Chef’ irá servir, os clientes poderão colaborar com sua avaliação (que será de uma à cinco estrelas) e com comentários para poderem relatar sua experiência. Dessa forma, a empresa terá um parâmetro de como está o funcionamento, apresentação e avaliação sobre o seu restaurante, assim podendo buscar melhorias para melhor atender e agradar seus clientes.
O escopo do **produto** pode ser consultado nos [requisitos do software](#requisitos-do-software)

### FORA DO ESCOPO

Não fazem parte do escopo do projeto:
* Pedido de refeição e delivery;
* Mostrar a receita dos pratos;
* Efetuar reserva no restaurante.

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
|RF-001 | Adicionar feedback | o sistema deve possibilitar a inserção de feedback/comentário dos clientes.  |
|RF-002 | Editar feedback | o sistema deve possibilitar edições nos feedbacks/comentários |
|RF-003 | Mostrar ranking | o sistema deve possibilitar que os pratos mais bem avaliados sejam sugeridos |
|RF-004 | Adicionar cupom | o sistema deve possibilitar que seja adicionado à compra em restaurante fisico, caso a meta de feedbacks do site seja alcançada, um desconto no valor total do próximo pedido em um restaurante filiado |
|RF-005 | Enviar Notificação | o sistema deve possibilitar o envio de mensagens informativas com novidades  ou notícias referentes ao site|
|RF-006 | Cadastrar cliente | o sistema deve possibilitar o cadastro de novos clientes no sistema |
|RF-007 | Alterar dados | o sistema deve possibilitar que o usuário faça alteração de seus dados pré cadastrados |
|RF-008 | Permitir a busca de  pratos do restaurante | o sistema deve possibilitar a pesquisa dos pratos presentes no menu |
|RF-009 | Permitir acesso dos feedbacks já feitos | o sistema deve permitir que seja apresentado, quando requisitado, os feedback já feito por um determinado usuário |
|RF-010 | Permitir que o cliente cadastre mais de uma conta | o sistema deve ter a disponibilidade da criação de contas alternativas do mesmo ip |
|RF-011 | Exibir avaliações | o sistema deve permitir que seja possível visualizar quantas avaliações o usuário possui | 
|RF-012 | Postar fotos | o sistema deve permitir que o cliente adicione fotos ao seu comentário |
|RF-013 | Apagar comentários | o sistema deve permitir que o usuario delete seu comentário, caso deseje |
|RF-014 | Entrar em contato com a empresa | o sistema deve possibilitar que o usuario entre em contato, por via de um chat, com a empresa |
|RF-015 | Realizar cadastro para ser um franqueado | o sistema deve possibilitar que a pessoa interessada em abrir uma loja franqueada, possa adquirir informações sobre e entrar em contato com os donos da empresa |
|RF-016 | Avaliar por localização | o sistema deve possibilitar que o usuario possa mostrar em que restaurante comeu, realizando a avaliação no restaurante que visitou |
|RF-017 | Favoritar produtos | o sistema deve possibilitar que o cliente favorite seus pratos prediletos |
|RF-018 | Avaliar atendimento | o sistema deve possibilitar que o cliente avalie, além dos pratos, o atendimento onde degustaram o mesmo |
|RF-019 | Demonstrar lista de desejos | o sistema deverá permitir e mostrar ao cliente sua lista de pratos que ainda deseja experimentar ou avaliar em uma proxima ida ao restaurante |
|RF-020 | Exibir valores | o sistema deve permitir que o usuario visualize, caso deseje, o valor de determinado prato |


## Requisitos Não Funcionais
A tabela a seguir contém a relação com os Requisitos Não Funcionais identificados, contendo identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
|:---|:---|:---|
|RNF-001 | Fotos com boa qualidade | o sistema deve conter fotos com boa qualidade dos produtos catalogados|
|RNF-002 | Organização do sistema | o sistema deve ser um site organizado, para maior compreensão dos usuários |
|RNF-003 | Compatibilidade | o site deve ser compativel com os sistemas operacionais: iOS, Android e Windows |
|RNF-004 | Requisitos legais | o sistema deverá atender às normas legais, tais como padrões, leis, etc |
|RNF-005 | Internet de qualidade | possui uma rede de internet que faça o site funcionar de forma rápida, com cerca de 15 Mbps para que funcione sem gerar demoras |
|RNF-006 | Privacidade | o site não deve mostrar aos outros usuários dados pessoais como: CPF, endereço e telefone de outros usuários |
|RNF-007 | Backup | o sistema deve realizar backup automaticamente à meia noite  |
|RNF-008 | Suporte | o site deve fornecer uma parte dedidcada para retirar duvidas e solucionar problemas |
|RNF-009 | Design flexivel | o site deve ser flexivel em questões de design, como quebra de linha devido a redução de tela, entre outros |
|RNF-010 | Manutenção | o site deve se manter atualizado e reparado constantemente |


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
