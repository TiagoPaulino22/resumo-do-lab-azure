# Resumos dos Laboratórios Azure
### Este repositório contém o resumo das lições aprendidas sobre Microsoft Azure durante o desenvolvimento dos labobarórios na DIO. 

## Sumário

[1. Resumo do laboratório 1: Localizando serviços por categoria](#1.-Resumo-do-laboratório-1:-Localizando-serviços-por-categoria) </br>
[2. Resumo do laboratório 2: Criando máquinas virtuais Azure](#2.-Resumo-do-laboratório-2:-Criando-máquinas-virtuais-Azure)  </br>
[3. Resumo do laboratório 3: Configurando uma instância de banco de dados Azure ](#3.-Resumo-do-laboratório-3:-Configurando-uma-instância-de-banco-de-dados-Azure-)</br>
[4. Resumo do laboratório 4: Construindo Arquiteturas no Azure](#4.-Resumo-do-laboratório-4:-Construindo-arquiteturas-no-Azure)</br>
[5. Resumo do laboratório 5: Consfigurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure](#5.-Resumo-do-laboratório-5:-Consfigurando-recursos-e-dimensionamentos-em-máquinas-virtuais-na-Azure )</br>


#### 1. Resumo do laboratório 1: Localizando serviços por categoria
Foi acessado o portal da Microsoft Azure. 
Em configurações do portal, pode ser trocado o idioma e a aparência do portal.  
Em todos os serviços, são mostrados os serviços por categoria, que inclui, entre outras: </br> 
-	IA + Machine Learning </br>
-	Bancos de dados </br>
-	Computação </br>
-	Contêiners </br>

Em todos os serviços/rede, pode ser acessado o **Bastions**, que é uma rede segura para fazer acesso às máquinas (Jump Server). </br>
Os serviços em versão prévia são aqueles que estão começando a ser disponibilizados e testados, eles não têm SLA(acordo de nível de serviço)

#### 2. Resumo do laboratório 2: Criando máquinas virtuais Azure 

Foi visto o tempo de inatividade para cada porcentagem no SLA (acordo de nível de serviço). Percebe-se que não há a possibilidade de 100% de disponibilidade do serviço. O cliente deve escolher o que melhor lhe atende. Ver figura abaixo:  </br> 

<img src = https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/SLA.PNG>

Para criar uma máquina virtual, é necessário ir em *Todos os serviços/computação/Infraestrutura como serviço/máquinas virtuais*. </br>
Ao criar uma máquina virtual, é necessário escolher a região, opções de disponibilidade, zona de disponibilidade, entre outras opções. 
A interface conta com informações e dicas nos itens para auxiliar o usuário. </br>
Foi mostrada a possibilidade de criar armazenamentos para redundância em local (LRS), em zonas (ZES), entre outros.  

#### 3. Resumo do laboratório 3: Configurando uma instância de banco de dados Azure 
**Tipos de serviços de nuvem Azure** </br>

<ins> Infraestrutura como serviço (IaaS)</ins> </br>
- Envolve servidores, máquinas virtuais, armazenamento e redes e segurança. 
- Você configura e gerencia o hardware para o seu aplicativo
- É o tipo de serviço que mais delega responsabilidade para o usuário

<ins>Plataforma como serviço (PaaS)</ins> </br>
- Engloba a infraestrutura como serviço mais ferramentas para: desenvolvedores, análises de negócios, gerenciamento de date base e sistemas operacionais
- Fornece um ambiente para a criação, teste e a implementação de aplicativos de softwares. 

<ins>Software como serviço (SaaS)</ins> </br>
- Engloba infraestrutura como serviço e plataforma como serviço </br>
- Os usuários se conectam e usam aplicativos com base em nuvem pela internet. </br>
- Usuários pagam pelo software que utilizam em um modelo de assinatura. </br>
- Os aplicativos são acessados pelo browser, como exemplos: </br>
  * Microsoft Office 365 </br>
  * E-mail </br>
  * Calendários  </br>

 <ins>Modelo de responsabilidade compartilhada</ins> </br>

 <img src = https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/mode_reponsabilidade.PNG>

**</ins>Laboratório 3</ins>** </br>

No laboratório 3, foram vistos alguns recursos que devem ser preenchidos para a criação de uma máquina virtual como a parte básica, discos, rede e monitoramento. 
Isso deixa evidente as características da infraestrutura como serviço, que delega grande parte da responsabilidade para o usuário. </br>

 <img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/maquina_virtual.PNG  >

Foi visto a criação de um banco de dados SQL. </br>
Para a sua criação é necessário ir em *Página incial/Bancos de dados SQL/Criar Banco de Dados SQL*. </br>
Para a criação de um banco de dados SQL é necessário criar um servidor e dizer qual vai ser o tipo de redundância de armazenamento do backup </br>

- Armazenamento de backup com redundância local
- Armazenamento de backup com redundância de zona 
- Armazenamento de backup com redundância geográfica



  


#### 4. Resumo do laboratório 4: Construindo arquiteturas no Azure

#### 5. Resumo do laboratório 5: Consfigurando recursos e dimensionamentos em máquinas virtuais na Azure 




