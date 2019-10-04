# TRABALHO BANCO DE DADOS:  Sistema de Contratação de Serviços
Trabalho desenvolvido durante a disciplina de BD1

# Sumário

### 1. COMPONENTES<br>
Integrantes do grupo<br>
André Luiz Coelho Silva: andrelcs@me.com<br>
Bianca Albuquerque da Silva: biancaalbuquerqs@gmail.com<br>
Mayke Willans Christo Pereira: maykewillians3@gmail.com<br>   

### 2.INTRODUÇÃO E MOTIVAÇAO<br>

> De acordo com dados divulgados pelo Instituto Brasileiro de Geografia e Estatística (IBGE), em setembro de 2019, a taxa de desemprego no Brasil ficou em 11,8% no trimestre encerrado em agosto, atingindo 12,6 milhões de pessoas. O resultado representou uma estabilidade frente ao último ano e pode ser justificado devido ao aumento do número de trabalhadores por conta própria e sem carteira assinada. O trabalho por conta própria chegou a 24,3 milhões de pessoas, o que representa uma alta de 4,7% (mais 1,1 milhão de pessoas) em relação ao mesmo período de 2018. Já o número de empregados sem carteira de trabalho assinada atingiu o recorde de 11,8 milhões de pessoas, o que representa um crescimento anual de 5,9% (mais 661 mil pessoas). 
Baseado nisso, os trabalhos autônomos têm se tornado uma opção extremamente viável para a população, e assim, aplicativos sob demanda como o iFood, Rappi, 99 e Uber, que atuam em problemas usuais e comuns, oferecendo praticidade e vantagem em relação a preços e comodidade, estão se tornando cada vez mais importantes no dia a dia.
Tendo em vista tais aspectos, o presente trabalho tem o objetivo de, através de um sistema informatizado, estimular o trabalho autônomo e promover a divulgação de pequenos serviços.
 

### 3.MINI-MUNDO<br>

> Os clientes desejam um sistema informatizado que promova a divulgação de pequenos serviços domésticos. O sistema deve fazer o cadastro de usuários, seja ele um prestador de serviço, alguém que esteja a procura de um serviço ou até ambos, certificando que os clientes são maiores de idade, e posteriormente permitirá a comunicação entre eles. O cadastro deverá ser validado solicitando ao usuário documentos de comprovação por meio de fotos.
Um anúncio de serviço deverá conter o nome, tipo do serviço, descrição do serviço, preço, horários disponíveis, localização, contato e modos de pagamento. Um usuário poderá iniciar uma conversa com o prestador de serviço caso esteja interessado no trabalho e os serviços poderão ser filtrados por categoria/tipo, avaliação dos clientes, distância, avaliação, preço e disponibilidade.
O horário, data, preço, local e o modo de pagamento do serviço serão combinados pelo chat e, após a obtenção de todas as informações, o prestador de serviço deverá preencher o agendamento e enviar para a confirmação do usuário. Assim, a confirmação de agendamento será composta pelas informações principais do atendimento, como o nome do contratante, a localização, o preço que foi combinado, o horário e data marcadas para a realização do serviço e a descrição do mesmo. Notificações de lembrete e confirmação de serviços poderão ser realizadas via email, telefone ou pelo próprio sistema, sendo opcional para o usuário.
Um serviço será avaliado pelo usuário após a conclusão do mesmo, servindo de parâmetro para o ranqueamento de avaliação.
 

### 4.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
<p align="center">
  <img width="356" height="725" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Tela%20Login.png?raw=true "Contratei Servicos">
</p>

![Arquivo PDF do Protótipo Balsamiq feito para o Sistema de Contratação de Serviços](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/TelasSistemaContratacaodeServicos.pdf?raw=true "Sistema de Contratação de Serviços")


#### 4.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    a) O sistema proposto poderá fornecer quais tipos de relatórios e informaçes? 
    b) Crie uma lista com os 5 principais relatórios que poderão ser obtidos por meio do sistema proposto!
    
> Os "clientes" precisam inicialmente dos seguintes relatórios:
* Relatório que informe quais prestadores de serviço oferecem serviços nas cidades dos clientes.
* Relatatório de usuários prestadores de serviço incluindo as seguintes informações: nome do usuário, nome do serviço, descrição, catergoria, preço e contato.
* Relatório de serviços agendados para um determinado dia incluindo as seguintes informações: nome do cliente, descrição do serviço, data, hora e localização.
* Relatório contendo as avaliações e comentários recebidos por um determinado serviço.
* Relatório que informe as informações de contato de um cliente incluindo: nome do cliente, cidade, bairro, endereço e número. 
 
#### 4.2 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    e deve ser criada antes do modelo conceitual
    c) Após criada esta tabela não deve ser modificada, pois será comparada com os resultados finais na conclusão do trabalho
    
![Tabela de dados do Sistema de Contratação de Serviços](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/TabelasSistemaContratacaodeServicos.xlsx?raw=true "Tabela - Sistema de Contratação de Serviços")
    
### 5.MODELO CONCEITUAL<br>
    A) NOTACAO ENTIDADE RELACIONAMENTO 
        * Para nosso prótótipo limitaremos o modelo conceitual nas 6 principais entidades do escopo
        * O protótipo deve possui no mínimo duas relações N para N
        * o mínimo de entidades do modelo conceitual será igual a 5
        
<p align="center">
  <img width="701" height="547" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/modelo_conceitual.png?raw=true "Modelo Conceitual")
</p>
      
    
    B) NOTACAO UML (Caso esteja fazendo a disciplina de analise)
    C) QUALIDADE 
        Garantir que a semântica dos atributos seja clara no esquema
        Criar o esquema de forma a garantir a redução de informação redundante, possibilidade de valores null, 
        e tuplas falsas
    
        
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]

#### 5.2 Descrição dos dados 
    
    USUARIO: Tabela que armazena as informações relativas ao cadastro dos usuários no Sistema.
    codigo: campo que armazena o número do código de cada usuário cadastrado no sistema.
    nome_usuario: campo que armazena o nome de usuário de cada cliente cadastrado no sistema.
    email: campo que armazena o endereço de email de cada usuario.
    sexo: campo que armazena o sexo de cada usuario cadastrado no sistema.
    senha: campo que armazena a senha cadastrada pelo usuairo.
    nome_completo: campo que armazena o nome completo do cliente.
    data_nascimento: campo que armazena a data de nascimento do cliente.
    cpf: campo que armazena o número de Cadastro de Pessoa Física para cada usuário cadastrado no Sistema.
    data_cadastro: campo que armazena a data em que o usuário se cadastrou no Sistema.
    
    SERVICO: Tabela que armazena as informações relativas ao serviços anunciados no Sistema.
    codigo: campo que armazena o 
    nome: campo que armazena o nome do serviço anunciado no Sistema.
    descricao: campo que armazena a descrição de cada serviço anunciado no Sistema.
    preco: campo que armazena a preço de cada serviço anunciado no Sistema. 
    dias_disponiveis: campo que armazena os dias que o prestador do serviço tem disponivel para realizar o serviço.
    horarios_disponiveis: campo que armazena os horarios que o prestador de serviço tem disponivel para realizar o serviço.
    modo_pagamento: campo que armazena o modo de pagamento de cada serviço.
    data_publicacao: campo que armazena a data em que o anuncio do serviço foi publicado.
    
    TELEFONE: Tabela que armazena as informações relativas aos telefones dos usuários cadastrados no Sistema.
    codigo: campo que armazena o codigo de cada usuário.
    telefone: campo que armazena o numero de telefone de cada usuário.
    
    ENDERECO: Tabela que armazena as informações relativas aos endereços de cada usuário cadastrado no Sistema.
    codigo: campo que armazena o codigo do endereço do usuário.
    codigo_usuario: campo que armazena o número do código de cada usuário cadastrado.
    cep: campo que armazena o número do CEP de cada usuário.
    bairro: campo que armazena o nome do bairro de cada usuário.
    endereco: campo que armazena o endereço de cada usuário.
    numero: campo que armazena o numero da casa de cada usuário.
    complemento: campo que armazena o complemento do endereço de cada usuário.
    cidade: campo que armazena a cidade de cada usuário.
    
    MODO_PAGAMENTO: Tabela que armazena os tipos de pagamento possíveis.
    codigo: campo que armazena o codigo de cada tipo de pagamento.
    modo: campo que armazena a descrição do modo de pagamento.
    
    LOCAL_AGENDADO: Tabela que armazena as informações relativas aos locais que os clientes agendaram os serviços.
    codigo_agendamento: campo que armazena o codigo de cada agendamento cadastrado.
    codigo_endereco: campo que armazena o codigo de cada endereço cadastrado.
    
    AVALIACOES: Tabela que armazena as informações relativas as avaliações feitas pelos clientes ao fim de cada serviço.
    codigo_servico: campo que armazena o codigo de cada serviço cadastrado no sistema.
    avaliacao: campo que armazena as avaliações feitas pelos clientes sobre o serviço contratado.
    comentarios: campo que armazena os comentários que cada cliente faz sobre o serviço contratado.
    
    AGENDAMENTO: Tabela que armazena as informações relativas ao agendamneto da contratação de um serviço.
    Cod_agendamento: campo que armazena o codigo de agendamento.
    Cod_servico: campo que armazena o codigo do serviço contratado.
    Cod_cliente: campo que armazena o codigo do cliente que contratou o serviço.
    Cod_prestador: campo que armazena o codigo do prestador do serviço.
    data_agendada: campo que armazena a data em que o serviço vai ser realizado.
    hora_agendada: campo que armazena o horario em que o serviço vai ser realizado.
 
#### 5.3 Principais fluxos de informação e principais tabelas do sistema     
    a) Quais os principais fluxos de dados de informação no sistema em densenvolvimento (mínimo 3)
    b) Quais as tabelas que conterão mais dados no sistema em densenvolvimento (mínimo 3)
    c) informe quais as 5 principais tabelas do sistema em densenvolvimento.

### 6	MODELO LÓGICO<br>
        a) inclusão do modelo lógico do banco de dados
        b) verificação de correspondencia com o modelo conceitual 
        (não serão aceitos modelos que não estejam em conformidade)
        
![Alt text](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/modelo_logico.png?raw=true "Modelo Lógico")

### 7	MODELO FÍSICO<br>
        a) inclusão das instruções de criacão das estruturas DDL 
        (criação de tabelas, alterações, etc..) 

<p align="center">
  <img width="326" height="574" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Modelo_Fisico.png?raw=true "Modelo Fisico">
</p> 
        
>## Marco de Entrega 01 em:<br>
        
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físico
        (Drop para exclusão de tabelas + create definição de para tabelas e estruturas de dados + insert para dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>
#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas

#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.

#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho

>## Marco de Entrega 02 em:<br>

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>
#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)<br>
#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho

#### 9.10	SUBCONSULTAS (Mínimo 3)<br>


#### 9.11 Relatórios e Gráficos 
    a)análises e resultados provenientes do banco de dados

>## Marco de Entrega 03 em:<br>

### 10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO FINAL (Mínimo 6 e Máximo 10)<br>
#### a) Pontos Chave do MINI-MUNDO
#### b) 5 principais tabelas/fluxos do sistema
#### c) Perguntas que podem ser respondidads com o sistema proposto
#### d) Modelo Conceitual
#### e) Modelo Lógico
#### f) Relatórios e Gráficos mais importantes para o sistema (mínimo 5) 
#### --> Tempo de apresentação 10 minutos


### 11 Backup completo do banco de dados postgres 
    a) deve ser realizado no formato "backup" 
        (Em Dump Options #1 Habilitar opções Don't Save Owner e Privilege)
    b) antes de postar o arquivo no git o mesmo deve ser testado/restaurado por outro grupo de alunos/dupla
    c) informar aqui o grupo de alunos/dupla que realizou o teste.

>## Marco de Entrega 04 em:<br>


### 12  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
    
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/
#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

    
### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. <strong>Caso existam arquivos com conteúdos sigilosos<strong>, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário do git "profmoisesomena", para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://www.sis4.com/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")


