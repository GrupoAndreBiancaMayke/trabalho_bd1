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
Um anúncio de serviço deverá conter o nome, tipo do serviço, descrição do serviço, preço, horários disponíveis, localização, contato e modos de pagamento. Um usuário poderá iniciar uma conversa com o prestador de serviço caso esteja interessado no trabalho e os serviços poderão ser filtrados por categoria/tipo, avaliação dos clientes, distância, avaliação e preço.
O horário, data, preço, local e o modo de pagamento do serviço serão combinados pelo chat e, após a obtenção de todas as informações, o prestador de serviço deverá preencher o agendamento e enviar para a confirmação do usuário. Assim, a confirmação de agendamento será composta pelas informações principais do atendimento, como o nome do contratante, a localização, o preço que foi combinado, o horário e data marcadas para a realização do serviço e a descrição do mesmo. Notificações de lembrete e confirmação de serviços poderão ser realizadas via email, telefone ou pelo próprio sistema, sendo opcional para o usuário.
Um serviço será avaliado pelo usuário após a conclusão do mesmo, servindo de parâmetro para o ranqueamento de avaliação.
 

### 4.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
<p align="center">
  <img width="356" height="725" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Tela%20Login.png?raw=true "Contratei Servicos">
</p>

![Arquivo PDF do Protótipo Balsamiq feito para o Sistema de Contratação de Serviços](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/TelasSistemaContratacaodeServicos.pdf?raw=true "Sistema de Contratação de Serviços")


#### 4.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    
> Os "clientes" precisam inicialmente dos seguintes relatórios:
* Relatório que informe quais prestadores de serviço oferecem serviços nas cidades dos clientes.
* Relatatório de usuários prestadores de serviço incluindo as seguintes informações: nome do usuário, nome do serviço, descrição, catergoria, preço e contato.
* Relatório de serviços agendados para um determinado dia incluindo as seguintes informações: nome do cliente, descrição do serviço, data, hora e localização.
* Relatório contendo as avaliações e comentários recebidos por um determinado serviço.
* Relatório que informe as informações de contato de um cliente incluindo: nome do cliente, cidade, bairro, endereço e número. 
 
#### 4.2 TABELA DE DADOS DO SISTEMA:

![Tabela de dados do Sistema de Contratação de Serviços](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/TabelasdedadosdoSistemadeContratacaodeServicos.xlsx?raw=true "Tabela - Sistema de Contratação de Serviços")
    
### 5.MODELO CONCEITUAL<br>
* Notação Entidade Relacionamento
        
<p align="center">
  <img width="980" height="539" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Modelo_Conceitual.PNG?raw=true "Modelo Conceitual")
</p>
      
* Notação UML

<p align="center">
  <img width="746" height="527" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/notacao_UML.jpg
</p>
        
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]

#### 5.2 Descrição dos dados 
    
    USUARIO: Tabela que armazena as informações relativas ao cadastro dos usuários no Sistema.
    cod_usuario: campo que armazena o número do código de cada usuário cadastrado no sistema.
    nome_usuario: campo que armazena o nome de usuário de cada cliente cadastrado no sistema.
    email: campo que armazena o endereço de email de cada usuario.
    sexo: campo que armazena o sexo de cada usuario cadastrado no sistema.
    senha: campo que armazena a senha cadastrada pelo usuairo.
    nome_completo: campo que armazena o nome completo do cliente.
    data_nascimento: campo que armazena a data de nascimento do cliente.
    cpf: campo que armazena o número de Cadastro de Pessoa Física para cada usuário cadastrado no Sistema.
    data_cadastro: campo que armazena a data em que o usuário se cadastrou no Sistema.

    SERVICO: Tabela que armazena as informações relativas ao serviços anunciados no Sistema.
    cod_servico: campo que armazena o codigo do serviço.
    cod_prestador: campo que armazena o código do prestador de determinado serviço.
    nome_servico: campo que armazena o nome do serviço anunciado no Sistema.
    descricao: campo que armazena a descrição de cada serviço anunciado no Sistema.
    preco: campo que armazena a preço de cada serviço anunciado no Sistema. 
    modo_pagamento: campo que armazena o modo de pagamento de cada serviço.
    data_publicacao: campo que armazena a data em que o anuncio do serviço foi publicado.

    CONTATO: Tabela que armazena as informações relativas aos telefones dos usuários cadastrados no Sistema.
    cod_usuario: campo que armazena o codigo de cada usuário.
    telefone: campo que armazena o numero de telefone de cada usuário.

    ENDERECO: Tabela que armazena as informações relativas aos endereços de cada usuário cadastrado no Sistema.
    cod_endereco: campo que armazena o codigo do endereço do usuário.
    cod_usuario: campo que armazena o número do código de cada usuário cadastrado.
    cep: campo que armazena o número do CEP de cada usuário.
    endereco: campo que armazena o endereço de cada usuário.
    numero_casa: campo que armazena o numero da casa de cada usuário.
    bairro: campo que armazena o codigo do nome do bairro de cada usuário.
    cidade: campo que armazena o codigo do nome da cidade de cada usuário.

    MODO_PAGAMENTO: Tabela que armazena os tipos de pagamento possíveis.
    cod_modo: campo que armazena o codigo de cada tipo de pagamento.
    modo_pagamento: campo que armazena a descrição do modo de pagamento.

    AVALIACOES: Tabela que armazena as informações relativas as avaliações feitas pelos clientes ao fim de cada serviço.
    cod_servico: campo que armazena o codigo de cada serviço cadastrado no sistema.
    avaliacoes_recebidas: campo que armazena as avaliações feitas pelos clientes sobre o serviço contratado.
    comentarios_recebidos: campo que armazena os comentários que cada cliente faz sobre o serviço contratado.

    AGENDAMENTO: Tabela que armazena as informações relativas ao agendamneto da contratação de um serviço.
    cod_agendamento: campo que armazena o codigo de agendamento.
    cod_servico: campo que armazena o codigo do serviço contratado.
    cod_cliente: campo que armazena o codigo do cliente que contratou o serviço.
    cod_endereco: campo que armazena o codigo do endereço que será realizado o serviço.
    data_agendada: campo que armazena a data em que o serviço vai ser realizado.
    hora_agendada: campo que armazena o horario em que o serviço vai ser realizado.

    CIDADE: Tabela que armazena o nome de cada cidade.
    codigo: campo que armazena o numero do codigo de cada cidade.
    nome: campo que armazena o nome da cidade.

    BAIRRO: Tabela que armazena o nome de cada bairro.
    codigo: campo que armazena o numero do codigo de cada bairro.
    nome: campo que armazena o nome do bairro.

#### 5.3 Principais fluxos de informação e principais tabelas do sistema 

> Os principais fluxos de dados de informação e, ainda, conterão mais dados no sistema ContrateiServiços são as tabelas USUARIO, SERVICO e AGENDAMENTO. As principais tabelas no sistema são USUARIO, SERVICO, AGENDAMENTO, ENDERECO e TELEFONE.

### 6	MODELO LÓGICO<br>
        
<p align="center">
  <img width="837" height="498" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Modelo_Logico.PNG "Modelo Lógico"
</p> 

### 7	MODELO FÍSICO<br>

<p align="center">
  <img width="267" height="383" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Modelo_Fisico.PNG?raw=true "Modelo Fisico">
</p> 

![Arquivo txt do Modelo Fisico feito para o Sistema de Contratação de Serviços](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/ModeloFisico?raw=true "Modelo Fisico")

>## Marco de Entrega 01 em:<br>
        
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físico
        (Drop para exclusão de tabelas + create definição de para tabelas e estruturas de dados + insert para dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
        
 <p align="center">
 <img width="1052" height="572"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/insert%20tabelas.PNG?raw=true "Dados Tabela  Usuario">
</p> 

![Arquivo txt do Insert aplicado nas tabelas de banco de dados](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/insert%20dos%20dados?raw=true "Insert nas Tabelas")
        

### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
   * SELECT * FROM USUARIO; //falta colocar o codigo do endereco no insert e no drive
   <p align="center">
 <img width="1170" height="670"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_usuario.png?raw=true "Dados Tabela  Usuario">
</p> 

   * SELECT * FROM SERVICO;
   <p align="center">
 <img width="961" height="429"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_servico.PNG?raw=true "Dados Tabela  Servico">
</p> 
     
   * SELECT * FROM CONTATO;
   <p align="center">
 <img width="603" height="779"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_contato.png?raw=true "Dados Tabela Contato">
</p> 
     
   * SELECT * FROM ENDERECO; 
   <p align="center">
 <img width="937" height="598"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_endereco.png?raw=true "Dados Tabela Endereco">
</p> 
     
   * SELECT * FROM MODO_PAGAMENTO;
   <p align="center">
 <img width="439" height="114"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_modo_pagamento.PNG?raw=true "Dados Tabela Modo Pagamento">
</p> 
     
   * SELECT * FROM AVALIACOES; 
   <p align="center">
 <img width="767" height="398"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_avaliacoes.PNG?raw=true "Dados Tabela Avaliacoes">
</p> 
     
   * SELECT * FROM AGENDAMENTO;
   <p align="center">
 <img width="962" height="619"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_agendamento.PNG?raw=true "Dados Tabela Agendamento">
</p> 
     
   * SELECT * FROM BAIRRO; 
   <p align="center">
 <img width="469" height="621"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_bairro.PNG?raw=true "Dados Tabela Dias disponiveis">
</p> 
     
   * SELECT * FROM CIDADE;
   <p align="center">
 <img width="405" height="272"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_cidade.PNG?raw=true "Dados Tabela Servico dias">
</p> 
     

#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>

* SELECT nome_completo FROM usuario WHERE sexo = 'F';
<p align="center">
  <img width="309" height="415" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/SELECT%20WHERE1.PNG?raw=true "Filtro Where 1"
</p> 

* SELECT nome, descricao FROM servico WHERE preco < 100;
<p align="center">
  <img width="571" height="178" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/SELECT%20WHERE2.PNG?raw=true "Filtro Where 2"
</p> 

* SELECT bairro, endereco FROM endereco WHERE cidade = 'Vitoria'; /*mexer nessa*/
<p align="center">
  <img width="520" height="195" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/SELECT%20WHERE3.PNG?raw=true "Filtro Where 3"
</p> 

* SELECT avaliacoes_recebidas, comentarios_recebidos FROM avaliacoes WHERE avaliacoes_recebidas >= 3;
<p align="center">
  <img width="725" height="365" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/SELECT%20WHERE4.PNG?raw=true "Filtro Where 4"
</p> 

#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas
    
#### Operadores Lógicos  

* SELECT nome, descricao FROM servico WHERE preco IS NOT NULL; 
<p align="center">
  <img width="564" height="223" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20L%C3%93GICOS1.PNG?raw=true "OPERADORES LÓGICOS 1"
</p>

* SELECT nome_completo FROM usuario WHERE data_nascimento >= '1990/01/01' AND data_nascimento <= '1999/12/31';
<p align="center">
  <img width="176" height="223" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20L%C3%93GICOS2.PNG?raw=true "OPERADORES LÓGICOS 2"
</p>

* SELECT nome, descricao FROM servico WHERE preco < 100 AND data_publicacao >= '2019/01/01';
<p align="center">
  <img width="557" height="192" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20L%C3%93GICOS3.PNG?raw=true "OPERADORES LÓGICOS 3"
</p>

* SELECT bairro, endereco FROM endereco WHERE cidade = 'Serra' OR cidade = 'Vila Velha'; /*mexer nessa*/
<p align="center">
  <img width="561" height="523" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20L%C3%93GICOS4.PNG?raw=true "OPERADORES LÓGICOS 4"
</p>

* SELECT bairro, endereco FROM endereco WHERE codigo_usuario IS NOT NULL; /*mexer nessa*/
<p align="center">
  <img width="537" height="619" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20L%C3%93GICOS5.PNG?raw=true "OPERADORES LÓGICOS 5"
</p>

#### Operadores Aritméticos

* SELECT nome, descricao, preco * 0.1 AS Desconto FROM servico;
<p align="center">
  <img width="944" height="323" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20ARITM%C3%89TICOS1.PNG?raw=true "OPERADORES ARITMÉTICOS 1"
</p>
 
* SELECT nome, descricao, preco * 0.9 AS "Preço com desconto" FROM servico WHERE preco * 0.9 < 90;
<p align="center">
  <img width="851" height="180" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20ARITM%C3%89TICOS2.PNG?raw=true "OPERADORES ARITMÉTICOS 2"
</p>
 
* SELECT nome, descricao, preco * 1.05 AS "Preço com inflação de 5%" FROM servico;
<p align="center">
  <img width="906" height="415" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20ARITM%C3%89TICOS3.PNG?raw=true "OPERADORES ARITMÉTICOS 3"
</p>      

#### Campos Renomeados

* SELECT nome_completo AS Nome, nome_usuario AS Login FROM usuario;
<p align="center">
  <img width="734" height="618" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CAMPOS%20RENOMEADOS1.PNG?raw=true "CAMPOS RENOMEADOS 1"
</p>

* SELECT COUNT( * ) AS Qtd_usuarios FROM usuario;
<p align="center">
  <img width="111" height="74" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CAMPOS%20RENOMEADOS2.PNG?raw=true "CAMPOS RENOMEADOS 2"
</p>

* SELECT nome_completo AS Nome, AGE(CURRENT_DATE,data_nascimento) AS Idade FROM usuario;
<p align="center">
  <img width="665" height="621" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CAMPOS%20RENOMEADOS3.PNG?raw=true "CAMPOS RENOMEADOS 3"
</p>

#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.
 
 
#### Operadores Like e Datas

* SELECT nome_completo FROM usuario WHERE nome_completo ILIKE 'm%';
<p align="center">
 <img width="168" height="179"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS1.PNG?raw=true "OPERADORES LIKE E DATAS 1">
</p> 

* SELECT nome_completo FROM usuario WHERE nome_completo LIKE '%a';
<p align="center">
 <img width="181" height="405"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS2.PNG?raw=true "OPERADORES LIKE E DATAS 2">
</p> 

* SELECT nome_completo, email FROM usuario WHERE email LIKE '%yahoo%';
<p align="center">
 <img width="632" height="112"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS3.PNG?raw=true "OPERADORES LIKE E DATAS 3">
</p> 

* SELECT telefone FROM contato WHERE telefone LIKE '(27)%';
<p align="center">
 <img width="149" height="510"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS4.PNG?raw=true "OPERADORES LIKE E DATAS 4">
</p> 

* SELECT nome_usuario FROM usuario WHERE nome_usuario LIKE '_______';
<p align="center">
 <img width="127" height="334"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS5.PNG?raw=true "OPERADORES LIKE E DATAS 5">
</p> 

* SELECT telefone FROM contato WHERE telefone LIKE '(28)%';
<p align="center">
 <img width="137" height="287"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS6.PNG?raw=true "OPERADORES LIKE E DATAS 6">
</p> 

* SELECT nome_completo, email FROM usuario WHERE email LIKE '%hotmail%';
<p align="center">
 <img width="643" height="365"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS7.PNG?raw=true "OPERADORES LIKE E DATAS 7">
</p> 

#### Operadores Like e Datas
* SELECT nome_completo, CURRENT_DATE-(data_cadastro) AS "Dias no sistema" FROM USUARIO;
<p align="center">
 <img width="678" height="622"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS8.PNG?raw=true "OPERADORES LIKE E DATAS 8">
</p> 

* SELECT nome, descricao FROM servico WHERE CURRENT_DATE-data_publicacao < 180;
<p align="center">
 <img width="840" height="330"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS9.PNG?raw=true "OPERADORES LIKE E DATAS 9">
</p> 

* SELECT COUNT( * ) AS "Quantidade de servicos nos ultimos 6 meses" FROM servico WHERE CURRENT_DATE-data_publicacao < 180;
<p align="center">
 <img width="317" height="78"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS10.PNG?raw=true "OPERADORES LIKE E DATAS 10">
</p> 

* SELECT codigo_servico, COUNT( * ) AS Qtd_Agendamentos_ultimos_3meses FROM agendamento WHERE CURRENT_DATE-data < 91 GROUP BY codigo_servico;
<p align="center">
 <img width="552" height="400"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS11.PNG?raw=true "OPERADORES LIKE E DATAS 11">
</p> 

* SELECT nome, CURRENT_DATE-data_publicacao AS Tempo_no_sistema FROM servico;
<p align="center">
 <img width="712" height="400"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/OPERADORES%20LIKE%20E%20DATAS12.PNG?raw=true "OPERADORES LIKE E DATAS 12">
</p> 

#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

* UPDATE servico SET modo_pagamento = 002 WHERE codigo = 009;
<p align="center">
 <img width="706" height="124"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/ATUALIZACAO_E_EXCLUSAO1.PNG?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 1">
</p> 

* UPDATE agendamento SET data = '2019/11/06'  WHERE codigo = 20;
<p align="center">
 <img width="992" height="544"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/ATUALIZACAO_E_EXCLUSAO2.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 2">
</p>

* DELETE FROM agendamento WHERE codigo_prestador = 17;
<p align="center">
 <img width="1021" height="544"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/ATUALIZACAO_E_EXCLUSAO3.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 3">
</p>

* INSERT INTO agendamento VALUES (020,    002, 016, 017, 016, '2019/11/05', 009);

* DELETE FROM agendamento WHERE codigo = 19;
<p align="center">
 <img width="1021" height="544"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/ATUALIZACAO_E_EXCLUSAO4.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 4">
</p>

* INSERT INTO agendamento VALUES (019, 009, 015, 005, 015, '2019/11/07',001);

* UPDATE servico SET modo_pagamento = 001 WHERE codigo = 009;
<p align="center">
 <img width="989" height="544"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/ATUALIZACAO_E_EXCLUSAO5.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 5">
</p>

* UPDATE contato SET telefone = '(27) 3354-1204' WHERE codigo = 012;
<p align="center">
 <img width="459" height="564"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/ATUALIZACAO_E_EXCLUSAO6.png "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 6">
</p>

#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br> /*mexer nessas*/
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        
* SELECT nome AS "Nome Servico", usuario.nome_completo AS "Nome Cliente", prestador.nome_completo AS "Nome Prestador", hora,data FROM servico INNER JOIN usuario_servico ON (usuario_servico.codigo_usuario = servico.codigo) INNER JOIN usuario ON (usuario_servico.codigo_usuario = usuario.codigo) INNER JOIN agendamento ON (agendamento.codigo = usuario.codigo) INNER JOIN usuario AS prestador ON (prestador.codigo = agendamento.codigo_prestador);
<p align="center">
 <img width="926" height="259"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CONSULTAS_COM_JUN%C3%87%C3%83O_E_ORDENA%C3%87%C3%83O1.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 1">
</p>

* SELECT DISTINCT cidade, servico.nome FROM usuario INNER JOIN endereco ON (usuario.codigo = endereco.codigo_usuario) INNER JOIN usuario_servico AS us ON (usuario.codigo = us.codigo_usuario) INNER JOIN servico ON (us.codigo_servico = servico.codigo);
<p align="center">
 <img width="629" height="400"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CONSULTAS_COM_JUN%C3%87%C3%83O_E_ORDENA%C3%87%C3%83O2.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 2">
</p>

* SELECT usuario.nome_completo AS "Prestador", servico.nome AS "Nome do servico", COUNT( * ) AS "Quantidade de agendamentos feitos" FROM usuario INNER JOIN agendamento ON (usuario.codigo = agendamento.codigo_prestador) INNER JOIN servico ON (agendamento.codigo_servico = servico.codigo) GROUP BY usuario.nome_completo, servico.nome ORDER BY COUNT( * ) DESC; 
<p align="center">
 <img width="815" height="447"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CONSULTAS_COM_JUN%C3%87%C3%83O_E_ORDENA%C3%87%C3%83O3.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 3">
</p>

* SELECT nome, descricao, avaliacoes_recebidas, comentarios_recebidos FROM servico INNER JOIN avaliacoes ON (servico.codigo = avaliacoes.cod_servico);
<p align="center">
 <img width="908" height="489"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CONSULTAS_COM_JUN%C3%87%C3%83O_E_ORDENA%C3%87%C3%83O4.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 4">
</p>

* SELECT servico.nome, telefone, min(avaliacoes_recebidas) AS "Menor avaliacao", max(avaliacoes_recebidas) AS "Maior avaliacao" FROM servico INNER JOIN avaliacoes ON (servico.codigo = avaliacoes.cod_servico) INNER JOIN usuario_servico ON (servico.codigo = usuario_servico.codigo_servico) INNER JOIN usuario ON (usuario.codigo = usuario_servico.codigo_usuario) INNER JOIN contato ON (usuario.codigo = contato.codigo) GROUP BY servico.nome, telefone;
<p align="center">
 <img width="876" height="366"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CONSULTAS_COM_JUN%C3%87%C3%83O_E_ORDENA%C3%87%C3%83O5.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 5">
</p>

* SELECT cidade, COUNT(cidade) AS "Qtd de servicos na cidade" FROM usuario INNER JOIN endereco ON (usuario.codigo = endereco.codigo_usuario) INNER JOIN usuario_servico ON (usuario.codigo = usuario_servico.codigo_usuario) INNER JOIN servico ON (servico.codigo = usuario_servico.codigo_servico) GROUP BY cidade ORDER BY COUNT(cidade);
<p align="center">
 <img width="657" height="260"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/CONSULTAS_COM_JUN%C3%87%C3%83O_E_ORDENA%C3%87%C3%83O6.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 6">
</p>

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


