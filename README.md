# TRABALHO BANCO DE DADOS:  Sistema de Contratação de Serviços
Trabalho desenvolvido durante a disciplina de Banco de Dados I

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
* Relatório que informe a quantidade de serviços realizados nas cidades dos clientes.
* Relatório que informe o número total de serviços agendados dos prestadores incluindo as seguintes informações: nome do serviço, descrição, categoria, preço e contato.
* Relatório de serviços agendados para um determinado dia incluindo as seguintes informações: nome do cliente, descrição do serviço, data, hora e localização.
* Relatório contendo as avaliações e comentários recebidos por um determinado serviço.
* Relatório que informe as informações de contato de um usuário incluindo: nome do cliente, cidade, bairro, endereço e número.  
 
#### 4.2 TABELA DE DADOS DO SISTEMA:

![Tabela de dados do Sistema de Contratação de Serviços](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/TabelasdedadosdoSistemadeContratacaodeServicos.xlsx?raw=true "Tabela - Sistema de Contratação de Serviços")
    
### 5.MODELO CONCEITUAL<br>
* Notação Entidade Relacionamento
        
<p align="center">
  <img width="965" height="551" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/ModeloConceitual.PNG?raw=true "Modelo Conceitual")
</p>
      
* Notação UML

<p align="center">
  <img width="746" height="527" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/notacao_UML.jpg
</p>
        
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Kaio Fabio, Renato Lopes]
    [Grupo02]: [Vinicius]

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
    codigo_endereco: campo que armazena o codigo do endereco do usuario.

    SERVICO: Tabela que armazena as informações relativas ao serviços anunciados no Sistema.
    codigo: campo que armazena o codigo do serviço.
    codigo_prestador: campo que armazena o código do prestador de determinado serviço.
    nome: campo que armazena o nome do serviço anunciado no Sistema.
    descricao: campo que armazena a descrição de cada serviço anunciado no Sistema.
    preco: campo que armazena a preço de cada serviço anunciado no Sistema. 
    codigo_modo_pagamento: campo que armazena o modo de pagamento de cada serviço.
    data_publicacao: campo que armazena a data em que o anuncio do serviço foi publicado.

    CONTATO: Tabela que armazena as informações relativas aos telefones dos usuários cadastrados no Sistema.
    codigo_usuario: campo que armazena o codigo de cada usuário.
    telefone: campo que armazena o numero de telefone de cada usuário.

    ENDERECO: Tabela que armazena as informações relativas aos endereços de cada usuário cadastrado no Sistema.
    codigo: campo que armazena o codigo do endereço do usuário.
    cep: campo que armazena o número do CEP de cada usuário.
    endereco: campo que armazena o endereço de cada usuário.
    numero: campo que armazena o numero da casa de cada usuário.
    codigo_bairro: campo que armazena o codigo do nome do bairro de cada usuário.
    codigo_cidade: campo que armazena o codigo do nome da cidade de cada usuário.

    MODO_PAGAMENTO: Tabela que armazena os tipos de pagamento possíveis.
    codigo: campo que armazena o codigo de cada tipo de pagamento.
    modo: campo que armazena a descrição do modo de pagamento.

    AVALIACOES: Tabela que armazena as informações relativas as avaliações feitas pelos clientes ao fim de cada serviço.
    codigo_servico: campo que armazena o codigo de cada serviço cadastrado no sistema.
    avaliacao: campo que armazena as avaliações feitas pelos clientes sobre o serviço contratado.
    comentario: campo que armazena os comentários que cada cliente faz sobre o serviço contratado.

    AGENDAMENTO: Tabela que armazena as informações relativas ao agendamneto da contratação de um serviço.
    codigo: campo que armazena o codigo de agendamento.
    codigo_servico: campo que armazena o codigo do serviço contratado.
    codigo_cliente: campo que armazena o codigo do cliente que contratou o serviço.
    codigo_endereco: campo que armazena o codigo do endereço que será realizado o serviço.
    data: campo que armazena a data em que o serviço vai ser realizado.
    hora: campo que armazena o horario em que o serviço vai ser realizado.

    CIDADE: Tabela que armazena o nome de cada cidade.
    codigo: campo que armazena o numero do codigo de cada cidade.
    nome: campo que armazena o nome da cidade.

    BAIRRO: Tabela que armazena o nome de cada bairro.
    codigo: campo que armazena o numero do codigo de cada bairro.
    nome: campo que armazena o nome do bairro.

#### 5.3 Principais fluxos de informação e principais tabelas do sistema 

> Os principais fluxos de dados de informação e, ainda, conterão mais dados no sistema ContrateiServiços são as tabelas USUARIO, SERVICO e AGENDAMENTO. As principais tabelas no sistema são USUARIO, SERVICO, AGENDAMENTO, ENDERECO e CONTATO.

### 6	MODELO LÓGICO<br>
        
<p align="center">
  <img width="938" height="514" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Modelologico.PNG?raw=true "Modelo Lógico"
</p> 

### 7	MODELO FÍSICO<br>

<p align="center">
  <img width="218" height="422" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Modelo_Fisico.png?raw=true "Modelo Fisico">
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
 <img width="1069" height="510"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/insert_tabelas.PNG?raw=true "Dados Tabela  Usuario">
</p> 

![Arquivo txt do Insert aplicado nas tabelas de banco de dados](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/insert%20dos%20dados)

![Arquivo .SQL do Insert aplicado nas tabelas de banco de dados](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/ContrateiServicos.sql)        

### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
   * SELECT * FROM USUARIO; 
   <p align="center">
 <img width="1170" height="670"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_usuario.png?raw=true "Dados Tabela  Usuario">
</p> 

   * SELECT * FROM SERVICO;
   <p align="center">
 <img width="1154" height="361"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_servico.png?raw=true "Dados Tabela  Servico">
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
 <img width="422" height="626"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_Bairro.PNG?raw=true "Dados Tabela Dias disponiveis">
</p> 
     
   * SELECT * FROM CIDADE;
   <p align="center">
 <img width="405" height="265"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/todos_os_dados_tabela_Cidade.PNG?raw=true "Dados Tabela Servico dias">
</p> 
     
#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>

**Seleciona e exibe todos os nomes na tabela Usuário do sexo feminino:**
* SELECT nome_completo FROM usuario WHERE sexo = 'F';
<p align="center">
  <img width="158" height="359" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Select%20Where1.PNG?raw=true "Filtro Where 1"
</p> 

**Seleciona e exibe todos os nomes, descrições da tabela Serviço onde o preço dos serviços são menores que 100:**
* SELECT nome, descricao FROM servico WHERE preco < 100;
<p align="center">
  <img width="784" height="321" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Select%20Where2.PNG?raw=true "Filtro Where 2"
</p> 

**Seleciona e exibe o nome e a descrição do servico que o preço não tem valor igual a zero:**
* SELECT nome, descricao FROM servico WHERE preco <> 0; 
<p align="center">
  <img width="528" height="191" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Select%20Where3.PNG?raw=true "Filtro Where 3"
</p> 

**Seleciona e exibe todos as avaliações e comentários recebidos da tabela Avaliacoes onde a avaliação recebida é maior ou igual a 3:**
* SELECT avaliacao, comentario FROM avaliacoes WHERE avaliacao >= 3;
<p align="center">
  <img width="577" height="325" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Select%20Where4.PNG?raw=true "Filtro Where 4"
</p> 

#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas
    
#### Operadores Lógicos  

**Consulta nas tabelas com Operadores Lógicos:**
* SELECT nome, descricao FROM servico WHERE preco < 100 AND preco > 50 ; 
<p align="center">
  <img width="519" height="132" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Logicos1.PNG?raw=true "OPERADORES LÓGICOS 1"
</p>

**Seleciona e exibe todos os nomes da tabela Usuário onde a data de nascimento de cada usuário está entre 01/01/1990 e 31/12/1999:**
* SELECT nome_completo FROM usuario WHERE data_nascimento >= '1990/01/01' AND data_nascimento <= '1999/12/31';
<p align="center">
  <img width="153" height="195" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Logicos2.PNG?raw=true "OPERADORES LÓGICOS 2"
</p>

**Seleciona e exibe todos os nomes e descrição de serviços na tabela Servico onde o preco dos mesmos é menor que 100 e a data de publicação deles é igual a 01/01/2019:**
* SELECT nome, descricao FROM servico WHERE preco < 100 AND data_publicacao >= '2019/01/01';
<p align="center">
  <img width="784" height="292" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Logicos3.PNG?raw=true "OPERADORES LÓGICOS 3"
</p>

**Seleciona e exibe todos os bairros e endereços da tabela Endereco onde a cidade das mesmas é Vila Velha ou Serra:**
* SELECT endereco FROM endereco WHERE codigo_cidade = 3 OR codigo_cidade = 2;
<p align="center">
  <img width="209" height="475" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Logicos4.PNG?raw=true "OPERADORES LÓGICOS 4"
</p>

**Seleciona e exibe todos os bairros e endereços da tabela Endereço onde o codigo dos usuarios não é nulo:**
* SELECT comentario FROM avaliacoes WHERE comentario IS NOT NULL;
<p align="center">
  <img width="413" height="355" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Logicos5.PNG?raw=true "OPERADORES LÓGICOS 5"
</p>

#### Operadores Aritméticos

**Seleciona e exibe o nome, a descrição e o valor de 10% de desconto dos serviços:**
* SELECT nome, descricao, preco * 0.1 AS Desconto FROM servico;
<p align="center">
  <img width="922" height="355" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Aritmeticos1.PNG?raw=true "OPERADORES ARITMÉTICOS 1"
</p>
 
**Seleciona e exibe o nome, a descrição e o valor total com 10% de desconto dos serviços:** 
* SELECT nome, descricao, preco * 0.9 AS "Preço com desconto" FROM servico WHERE preco * 0.9 < 90;
<p align="center">
  <img width="906" height="323" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Aritmeticos2.PNG?raw=true "OPERADORES ARITMÉTICOS 2"
</p>
 
**Seleciona e exibe o nome, a descrição e o preço com inflação de 5%:**
* SELECT nome, descricao, preco * 1.05 AS "Preço com inflação de 5%" FROM servico;
<p align="center">
  <img width="899" height="355" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Aritmeticos3.PNG?raw=true "OPERADORES ARITMÉTICOS 3"
</p>      

#### Campos Renomeados

**Seleciona e exibe o nome e o login dos usuários:**
* SELECT nome_completo AS Nome, nome_usuario AS Login FROM usuario;
<p align="center">
  <img width="723" height="620" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Campos_Renomeados1.PNG?raw=true "CAMPOS RENOMEADOS 1"
</p>

**Seleciona e exibe a quantidade de usuários:**
* SELECT COUNT( * ) AS Qtd_usuarios FROM usuario;
<p align="center">
  <img width="85" height="58" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Campos_Renomeados2.PNG?raw=true "CAMPOS RENOMEADOS 2"
</p>

**Seleciona e exibe o nome e a idade dos usuários:**
* SELECT nome_completo AS Nome, AGE(CURRENT_DATE,data_nascimento) AS Idade FROM usuario;
<p align="center">
  <img width="632" height="620" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Campos_Renomeados3.PNG?raw=true "CAMPOS RENOMEADOS 3"
</p>

#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.
 
 
#### Operadores Like e Datas

**Seleciona e exibe o nome completo dos usuários que iniciam com M:**
* SELECT nome_completo FROM usuario WHERE nome_completo ILIKE 'm%';
<p align="center">
 <img width="131" height="147"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data1.PNG?raw=true "OPERADORES LIKE E DATAS 1">
</p> 

**Seleciona e exibe o nome completo dos usuários que terminam com A:**
* SELECT nome_completo FROM usuario WHERE nome_completo LIKE '%a';
<p align="center">
 <img width="143" height="317"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data2.PNG?raw=true "OPERADORES LIKE E DATAS 2">
</p> 

**Seleciona e exibe o nome completo e o email dos usuários que possuem contas no yahoo:**
* SELECT nome_completo, email FROM usuario WHERE email LIKE '%yahoo%';
<p align="center">
 <img width="599" height="84"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data3.PNG?raw=true "OPERADORES LIKE E DATAS 3">
</p> 

**Seleciona e exibe o telefone dos usuários com DDD 27:**
* SELECT telefone FROM contato WHERE telefone LIKE '(27)%';
<p align="center">
 <img width="95" height="406"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data4.PNG?raw=true "OPERADORES LIKE E DATAS 4">
</p> 

**Seleciona e exibe o login dos usuários que possuem 7 caracteres:**
* SELECT nome_usuario FROM usuario WHERE nome_usuario LIKE '_______';
<p align="center">
 <img width="81" height="254"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data5.PNG?raw=true "OPERADORES LIKE E DATAS 5">
</p> 

**Seleciona e exibe o telefone dos usuários que possuem DD 28:**
* SELECT telefone FROM contato WHERE telefone LIKE '(28)%';
<p align="center">
 <img width="91" height="228"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data6.PNG?raw=true "OPERADORES LIKE E DATAS 6">
</p> 

**Seleciona e exibe o nome completo e o email dos usuários que possuem conta hotmail:**
* SELECT nome_completo, email FROM usuario WHERE email LIKE '%hotmail%';
<p align="center">
 <img width="603" height="289"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data7.PNG?raw=true "OPERADORES LIKE E DATAS 7">
</p> 

#### Operadores Like e Datas

**Seleciona o nome dos usuário e mostra a quanto tempo ele estão cadastrados no sistema:**
* SELECT nome_completo, CURRENT_DATE-(data_cadastro) AS "Dias no sistema" FROM usuario;
<p align="center">
 <img width="677" height="627"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data8.PNG?raw=true "OPERADORES LIKE E DATAS 8">
</p> 

**Seleciona e exibe o nome e a descrição dos serviços que estão com menos de 180 dias cadastrados no sistema:**
* SELECT nome, descricao FROM servico WHERE CURRENT_DATE-data_publicacao < 180;
<p align="center">
 <img width="760" height="227"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data9.PNG?raw=true "OPERADORES LIKE E DATAS 9">
</p> 

**Exibe a quantidade de serviços que foram cadastrados nos ultimos 6 meses:**
* SELECT COUNT( * ) AS "Quantidade de servicos nos ultimos 6 meses" FROM servico WHERE CURRENT_DATE-data_publicacao < 180;
<p align="center">
 <img width="264" height="60"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data10.PNG?raw=true "OPERADORES LIKE E DATAS 10">
</p> 

**Seleciona e exibe o codigo do serviço que foi agendado nos ultimos 3 meses:**
* SELECT codigo_servico, COUNT( * ) AS Qtd_Agendamentos_ultimos_3meses FROM agendamento WHERE CURRENT_DATE-data < 91 GROUP BY codigo_servico;
<p align="center">
 <img width="510" height="320"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data11.PNG?raw=true "OPERADORES LIKE E DATAS 11">
</p> 

**Seleciona e exibe o nome de todos os serviços e o tempo que eles estão cadastrados no sistema:**
* SELECT nome, CURRENT_DATE-data_publicacao AS Tempo_no_sistema FROM servico;
<p align="center">
 <img width="705" height="321"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Operadores_Like_e_Data12.PNG?raw=true "OPERADORES LIKE E DATAS 12">
</p> 

#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

**Atualização o modo de pagamento do servico com codigo número 009 na tabela Serviço:**
* UPDATE servico SET codigo_modo_pagamento = 002 WHERE codigo = 009;
<p align="center">
 <img width="987" height="506"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Atualizacao_e_Exclusao1.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 1">
</p> 

**Atualização a data de agendamento do serviço com o código número 20:**
* UPDATE agendamento SET data = '2019/11/06'  WHERE codigo = 20;
<p align="center">
 <img width="987" height="506"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Atualizacao_e_Exclusao2.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 2">
</p>

**Exclusão dos dados da tabela de agendamento onde o código do prestador é igual a 17:**
* DELETE FROM agendamento WHERE codigo = 20;
<p align="center">
 <img width="995" height="492"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Atualizacao_e_Exclusao3.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 3">
</p>

**Insere novamente os dados na tabela agendamento que foi excluido:**
* INSERT INTO agendamento VALUES (020,    002, 016, 016, '2019/11/05', '15h00');

**Exclusão dos dados da tabela de agendamento onde o código do prestador é igual a 19:**
* DELETE FROM agendamento WHERE codigo = 19;
<p align="center">
 <img width="995" height="492"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Atualizacao_e_Exclusao4.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 4">
</p>

**Insere novamente os dados na tabela agendamento que foi excluido:**
* INSERT INTO agendamento VALUES (019, 009, 015, 015, '2019/11/07','9h00');

**Atualização o modo de pagamento do servico com codigo número 009 na tabela Serviço:**
* UPDATE servico SET codigo_modo_pagamento = 001 WHERE codigo = 009;
<p align="center">
 <img width="989" height="506"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Atualizacao_e_Exclusao5.png?raw=true "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 5">
</p>

**Atualização do telefone na tabela contato do usuário com o código número 20:**
* UPDATE contato SET telefone = '(27) 3354-1204' WHERE codigo_usuario = 012;
<p align="center">
 <img width="605" height="484"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Atualizacao_e_Exclusao6.png "ATUALIZAÇÃO E EXCLUSÃO DE DADOS 6">
</p>

#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br> 
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        
**Faz a junção de todas as tabelas:**
* SELECT cliente.nome_completo AS nome_cliente, contato.telefone, endereco, endereco.numero, bairro.nome as bairro, cidade.nome as cidade, servico.nome as servico, modo as pagamento, MAX(avaliacao) AS Avaliacao_maxima FROM agendamento INNER JOIN servico ON (agendamento.codigo_servico = servico.codigo) INNER JOIN usuario AS cliente ON (agendamento.codigo_cliente = cliente.codigo) INNER JOIN endereco ON (agendamento.codigo_endereco = endereco.codigo) INNER JOIN cidade ON (endereco.codigo_cidade = cidade.codigo) INNER JOIN bairro ON (endereco.codigo_bairro = bairro.codigo) INNER JOIN contato ON (cliente.codigo = contato.codigo_usuario) INNER JOIN modo_pagamento ON (servico.codigo_modo_pagamento = modo_pagamento.codigo) INNER JOIN avaliacoes ON (avaliacoes.codigo_servico = servico.codigo) GROUP BY cliente.nome_completo, contato.telefone, endereco, endereco.numero, bairro.nome, cidade.nome, servico.nome, modo;
<p align="center">
 <img width="996" height="468"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Consulta_Juncao_todas_as_Tabelas.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 1">
</p>

**Faz junção das tabelas Serviço, Usuário e Agendamento. Mostrando o nome do serviço que será prestado, o dia e a hora do agendamento, nome do cliente e nome do prestador:**
* SELECT nome AS "Nome Servico", usuario.nome_completo AS "Nome Cliente", prestador.nome_completo AS "Nome Prestador", hora,data FROM servico  INNER JOIN usuario ON (servico.codigo_prestador = usuario.codigo) INNER JOIN agendamento ON (agendamento.codigo_cliente = usuario.codigo) INNER JOIN usuario AS prestador ON (prestador.codigo = servico.codigo_prestador);
<p align="center">
 <img width="922" height="360"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Consulta_com_Juncao1.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 2">
</p>

**Faz junção das tabelas Cidade, Usuário, Serviço. Mostrando o nome da cidade que estão localizado os prestadores de serviço e o nome dos serviços:**
* SELECT cidade.nome AS "Nome cidade", servico.nome FROM usuario INNER JOIN endereco ON (usuario.codigo_endereco = endereco.codigo) INNER JOIN servico ON (usuario.codigo = servico.codigo_prestador) INNER JOIN cidade ON (cidade.codigo = endereco.codigo_cidade);
<p align="center">
 <img width="628" height="404"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Consulta_com_Juncao2.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 3">
</p>

**Faz junção das tabelas Serviço, Usuário e Agendamento. Mostrando a quantidade de agendamentos por prestador de serviço:**
* SELECT usuario.nome_completo AS "Prestador", servico.nome AS "Nome do servico", COUNT( * ) AS "Quantidade de agendamentos feitos" FROM usuario INNER JOIN servico ON (usuario.codigo = servico.codigo_prestador) INNER JOIN agendamento ON (agendamento.codigo_servico = servico.codigo) GROUP BY usuario.nome_completo, servico.nome ORDER BY COUNT( * ) DESC;
<p align="center">
 <img width="821" height="400"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Consulta_com_Juncao3.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 4">
</p>

**Faz junção das tabelas Serviço e Avaliações. Mostrando o nome do serviço, a descrição e as avaliações recebidas:**
* SELECT nome, descricao, avaliacao, comentario FROM servico INNER JOIN avaliacoes ON (servico.codigo = avaliacoes.codigo_servico);
<p align="center">
 <img width="914" height="481"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Consulta_com_Juncao4.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 5">
</p>

**Faz junção das tabelas Avaliações, Usuário e Contato. Mostrando o nome do serviço, telefone do prestador, a menor avaliação recebida, a maior avaliação recebida e a média de avaliações recebidas:**
* SELECT servico.nome, telefone, min(avaliacao) AS "Menor avaliacao", max(avaliacao) AS "Maior avaliacao" FROM servico INNER JOIN avaliacoes ON (servico.codigo = avaliacoes.codigo_servico) INNER JOIN usuario ON (usuario.codigo = servico.codigo_prestador) INNER JOIN contato ON (usuario.codigo = contato.codigo_usuario) GROUP BY servico.nome, telefone;
<p align="center">
 <img width="851" height="364"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Consulta_com_Juncao5.PNG?raw=true "JUNÇÃO E ORDENAÇÃO 6">
</p>

>## Marco de Entrega 02 em:<br>

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>

**Exibe a quantidade de usuários por sexo:**
* SELECT sexo, COUNT(  *  ) AS "Quantidade"  FROM usuario GROUP BY sexo; 
<p align="center">
  <img width="418" height="105" src= https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Group_by1.PNG?raw=true "Consulta Group by 1"
</p> 
 
 **Exibe a quantidade de usuários por cidade:**
 * SELECT cidade.nome, COUNT( * ) AS "Quantidade" FROM endereco INNER JOIN cidade ON (cidade.codigo = endereco.codigo_cidade) GROUP BY cidade.nome;
<p align="center">
  <img width="710" height="289" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Group_by2.PNG?raw=true "Consulta Group by 2"
</p> 
 
 **Exibe a quantidade de usuários por bairro:**
 * SELECT bairro.nome, COUNT( * ) AS “Quantidade” FROM endereco INNER JOIN bairro ON (bairro.codigo = endereco.codigo_bairro) GROUP BY bairro.nome;
<p align="center">
  <img width="629" height="620" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Group_by3.PNG?raw=true "Consulta Group by 3"
</p> 
 
 **Exibe a quantidade de avaliações que foram feitas em cada nota:**
 * SELECT avaliacao, COUNT( * ) AS "Quantidade" FROM avaliacoes GROUP BY avaliacao ORDER BY avaliacao DESC; 
<p align="center">
  <img width="518" height="163" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Group_by4.PNG?raw=true "Consulta Group by 4"
</p> 
 
 **Exibe a média de preço dos serviço cadastrados no sistema:**
 * SELECT AVG(NULLIF(preco,0)) AS "Media de precos" FROM servico;
<p align="center">
  <img width="119" height="58" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Group_by5.PNG?raw=true "Consulta Group by 5"
</p> 
 
 **Exibe o código do serviço e a quantidade de agendamento realizada para os mesmos:**
 * SELECT codigo_servico, COUNT ( * ) AS qtd_agendamentos FROM agendamento GROUP BY codigo_servico;
<p align="center">
  <img width="562" height="355" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Group_by6.PNG?raw=true "Consulta Group by 6"
</p> 
 
#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)<br>
 
 **Exibe o nome completo dos usuários que não são prestadores de serviço:**
 * SELECT nome_completo FROM usuario LEFT OUTER JOIN servico ON (usuario.codigo = servico.codigo_prestador) WHERE codigo_prestador IS NULL;  
<p align="center">
  <img width="179" height="405" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Left_e_Right_join2.PNG?raw=true "Consulta Left e Right Join 2"
</p>

**Exibe o nome dos serviços que não tem avaliação:**
* SELECT nome AS nome_servico, descricao FROM servico LEFT OUTER JOIN avaliacoes ON (servico.codigo = avaliacoes.codigo_servico) WHERE codigo_servico IS NULL; 
<p align="center">
  <img width="615" height="63" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Left_e_Right_Join3.PNG?raw=true "Consulta Left e Right Join 3"
</p>
 
 **Exibe o nome completo e endereço dos usuários:**
 * SELECT usuario.nome_completo, endereco.cep FROM usuario LEFT OUTER JOIN endereco ON (usuario.codigo_endereco = endereco.codigo); 
<p align="center">
  <img width="744" height="595" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Left_e_Right_join1.PNG?raw=true "Consulta Left e Right Join 1"
</p>
 
 **Exibe o nome completo dos usuários que prestam algum tipo de serviço:**
 * SELECT usuario.nome_completo, servico.nome FROM usuario  RIGHT OUTER JOIN servico ON (usuario.codigo = servico.codigo_prestador); 
<p align="center">
  <img width="601" height="325" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Left_e_Right_Join4.PNG?raw=true "Consulta Left e Right Join 4"
</p>

#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho

**Exibe a View com os nomes e endereços dos usuários cadastrados no sistema:**
* CREATE VIEW nome_e_endereco_usuario AS SELECT usuario.nome_completo, endereco.endereco AS rua, endereco.numero AS numero_casa, bairro.nome AS nome_bairro, cidade.nome AS nome_cidade FROM usuario INNER JOIN endereco ON (usuario.codigo_endereco = endereco.codigo) INNER JOIN bairro ON (endereco.codigo_bairro = bairro.codigo) INNER JOIN cidade ON (endereco.codigo_cidade = cidade.codigo); 
<p align="center">
  <img width="939" height="616" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/View1.PNG?raw=true "Criar View 1"
</p>

**Exibe a View com os nomes dos usuários e telefone dos mesmos:**
* CREATE VIEW nome_e_contato AS SELECT nome_completo, telefone FROM usuario INNER JOIN contato ON (usuario.codigo = contato.codigo_usuario); 
<p align="center">
  <img width="689" height="619" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/View2.PNG?raw=true "Criar View 2"
</p>

**Exibe a View com os nomes dos serviços e preço dos mesmos:**
* CREATE VIEW servicos_e_precos  AS SELECT nome, preco FROM servico;  
<p align="center">
  <img width="847" height="313" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/View3.PNG?raw=true "Criar View 3"
</p>

**Exibe a View com os nomes dos serviços e as avaliações de cada serviço:**
* CREATE VIEW servico_e_avaliacao  AS SELECT servico.nome, avaliacao FROM servico INNER JOIN avaliacoes ON (servico.codigo = avaliacoes.codigo_servico); 
<p align="center">
  <img width="802" height="325" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/View4.PNG?raw=true "Criar View 4"
</p>

**Exibe a View com nome do usuário e o email do mesmo:**
* CREATE VIEW contato_eletronico_usuario AS SELECT nome_completo, email, nome_usuario FROM usuario; 
<p align="center">
  <img width="606" height="626" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/View5.PNG?raw=true "Criar View 5"
</p>

**Exibe a View com os dados cadastrias de cada usuário, contendo: nome, data de nascimento, cpf nome de usuario e email:**
* CREATE VIEW dados_cadastrais AS SELECT nome_completo AS "Nome Completo", data_nascimento,cpf, nome_usuario, email FROM usuario; 
<p align="center">
  <img width="879" height="622" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/View6.PNG?raw=true "Criar View 6"
</p>

#### 9.10	SUBCONSULTAS (Mínimo 3)<br>

**Exibe o nome completo e o email de cada usuário que tenha o código na tabela Serviço:**
* SELECT nome_completo, email FROM usuario WHERE codigo IN (SELECT codigo_prestador FROM servico); 
<p align="center">
  <img width="602" height="319" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Subconsulta1.PNG?raw=true "Subconsulta 1"
</p>
 
 **Exibe o nome do serviço que tem a maior avaliação registrada na tabela de Avaliações:**
 * SELECT nome AS "Nome Servico" FROM servico INNER JOIN avaliacoes ON (servico.codigo = avaliacoes.codigo_servico) WHERE avaliacao IN (SELECT MAX(avaliacao) FROM avaliacoes); 
<p align="center">
  <img width="88" height="173" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Subconsulta2.PNG?raw=true "Subconsulta 2"
</p>
 
 **Exibe o endereço, o número e o CEP do usuário que tenha o código da cidade de Vitória:**
 * SELECT endereco, numero, cep FROM endereco WHERE codigo_cidade IN (SELECT codigo FROM cidade WHERE nome <> 'Vitoria'); 
<p align="center">
  <img width="843" height="559" src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Subconsulta3.PNG?raw=true "Subconsulta 3"
</p>

#### 9.11 Relatórios e Gráficos 
    a)análises e resultados provenientes do banco de dados
    
**Relatório 1: Informar a quantidade de serviços realizados nas cidades dos clientes.**

- SELECT count(cidade.nome) AS qtd_de_servico_na_cidade,cidade.nome AS nome_da_cidade FROM usuario INNER JOIN servico ON (usuario.codigo = servico.codigo_prestador) INNER JOIN agendamento ON (usuario.codigo = agendamento.codigo_cliente) INNER JOIN usuario_endereco AS ue ON (usuario.codigo = ue.codigo_usuario) INNER JOIN endereco ON (ue.codigo_endereco = endereco.codigo) INNER JOIN cidade ON (cidade.codigo = endereco.codigo_cidade) group by cidade.nome;
 <p align="center">
 <img width="412" height="159"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Relatorio1.PNG?raw=true "Grafico 1">
</p> 

- SELECT count(cidade.nome) AS qtd_de_servico_na_cidade,cidade.nome AS nome_da_cidade FROM usuario INNER JOIN servico ON (usuario.codigo = servico.codigo_prestador) INNER JOIN agendamento ON (usuario.codigo = agendamento.codigo_cliente) INNER JOIN usuario_endereco AS ue ON (usuario.codigo = ue.codigo_usuario) INNER JOIN endereco ON (ue.codigo_endereco = endereco.codigo) INNER JOIN cidade ON (cidade.codigo = endereco.codigo_cidade) group by cidade.nome; 
                              
* Serviços Realizados por Cidade;

 <p align="center">
 <img width="646" height="467"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Grafico1.PNG?raw=true "Grafico 1">
</p> 

**Relatório 2: Informar o número total de serviços agendados dos prestadores incluindo as seguintes informações: nome do serviço, descrição, categoria, preço e contato.**

- SELECT nome_completo AS nome_prestador, nome AS nome_servico, descricao, preco FROM usuario INNER JOIN servico ON (usuario.codigo = servico.codigo_prestador);
 <p align="center">
 <img width="806" height="341"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Relatorio2.PNG?raw=true "Grafico 1">
</p> 

- SELECT servico.nome, COUNT( * ) AS qtd_agendamentos FROM agendamento INNER JOIN servico ON (servico.codigo = agendamento.codigo_servico) GROUP BY servico.nome; 
                              
* Total de Agendamento por serviço;

 <p align="center">
 <img width="850" height="457"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Grafico2.PNG?raw=true "Grafico 2">
</p> 

**Relatório 3: Informar serviços agendados para um determinado dia incluindo as seguintes informações: nome do cliente, descrição do serviço, data, hora e localização.**

- SELECT nome_completo AS nome_cliente, servico.nome AS "servico_contratado", agendamento.data,agendamento.hora, cidade.nome AS nome_da_cidade FROM usuario INNER JOIN usuario_endereco AS ue ON (usuario.codigo = ue.codigo_usuario) INNER JOIN servico ON (usuario.codigo = servico.codigo_prestador) INNER JOIN agendamento ON (usuario.codigo = agendamento.codigo_cliente) INNER JOIN endereco ON (ue.codigo_endereco = endereco.codigo) INNER JOIN cidade ON (cidade.codigo = endereco.codigo_cidade);
 <p align="center">
 <img width="683" height="288"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Relatorio3.PNG?raw=true "Grafico 1">
</p> 

- SELECT COUNT( * ) AS qtd_agendamento, nome_completo AS nome_cliente FROM usuario INNER JOIN usuario_endereco AS ue ON (usuario.codigo = ue.codigo_usuario) INNER JOIN servico ON (usuario.codigo = servico.codigo_prestador) INNER JOIN agendamento ON (usuario.codigo = agendamento.codigo_cliente) INNER JOIN endereco ON (ue.codigo_endereco = endereco.codigo) INNER JOIN cidade ON (cidade.codigo = endereco.codigo_cidade) GROUP BY nome_cliente; 
                              
* Serviços Contratados por Usuário;

 <p align="center">
 <img width="741" height="461"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Grafico3.PNG?raw=true "Grafico 3">
</p> 

**Relatório 4: Informar avaliações e comentários recebidos para um determinado serviço.**

- SELECT nome AS nome_do_servico, avaliacao, comentario FROM avaliacoes INNER JOIN servico ON (servico.codigo = avaliacoes.codigo_servico);
 <p align="center">
 <img width="652" height="349"          src=https://raw.githubusercontent.com/GrupoAndreBiancaMayke/trabalho_bd1/master/images/Relatorio4.PNG?raw=true "Grafico 1">
</p> 

- SELECT avaliacao, COUNT( * ) AS qtd_de_avaliacoes FROM avaliacoes GROUP BY avaliacao ORDER BY avaliacao DESC; 
                              
* Avaliações Realizadas;

 <p align="center">
 <img width="580" height="459"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Grafico4.PNG?raw=true "Grafico 4">
</p> 

**Relatório 5: Informar as informações de contato de um usuário incluindo: nome do cliente, cidade, bairro, endereço e número.**

- SELECT nome_completo AS nome_cliente,endereco AS rua, bairro.nome AS nome_do_bairro, endereco.numero AS numero_casa,cidade.nome AS nome_da_cidade, email, telefone FROM usuario INNER JOIN usuario_endereco AS ue ON (usuario.codigo = ue.codigo_usuario) INNER JOIN endereco ON (ue.codigo_endereco = endereco.codigo) INNER JOIN cidade ON (cidade.codigo = endereco.codigo_cidade) INNER JOIN bairro ON (bairro.codigo = endereco.codigo_bairro) INNER JOIN contato ON (usuario.codigo = contato.codigo_usuario);
 <p align="center">
 <img width="1106" height="629"          src=https://raw.githubusercontent.com/GrupoAndreBiancaMayke/trabalho_bd1/master/images/Relatorio5.PNG?raw=true "Grafico 1">
</p> 


- SELECT cidade.nome AS nome_da_cidade, COUNT( * ) AS qtd_de_moradores FROM usuario INNER JOIN usuario_endereco AS ue ON (usuario.codigo = ue.codigo_usuario) INNER JOIN endereco ON (ue.codigo_endereco = endereco.codigo) INNER JOIN cidade ON (cidade.codigo = endereco.codigo_cidade) INNER JOIN bairro ON (bairro.codigo = endereco.codigo_bairro) GROUP BY nome_da_cidade; 
                              
* Quantidade de moradores por cidade;

 <p align="center">
 <img width="768" height="450"          src=https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/images/Grafico5.PNG?raw=true "Grafico 5">
</p> 

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
   
Teste do Backup:
- [Grupo01]: [Kaio Fabio, Renato Lopes]


![Arquivo Backup completo do banco de dados postgres](https://github.com/GrupoAndreBiancaMayke/trabalho_bd1/blob/master/arquivos/ContrateiServicos.backup)

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


