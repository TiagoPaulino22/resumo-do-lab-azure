# 📖 Resumos dos Laboratórios Azure
### Este repositório contém o resumo das lições aprendidas sobre Microsoft Azure durante o desenvolvimento dos labobarórios na DIO. 

## Sumário

[1. Resumo do laboratório 1: Localizando serviços por categoria](#1.-Resumo-do-laboratório-1:-Localizando-serviços-por-categoria) </br>
[2. Resumo do laboratório 2: Criando máquinas virtuais Azure](#2.-Resumo-do-laboratório-2:-Criando-máquinas-virtuais-Azure)  </br>
[3. Resumo do laboratório 3: Configurando uma instância de banco de dados Azure ](#3.-Resumo-do-laboratório-3:-Configurando-uma-instância-de-banco-de-dados-Azure-)</br>
[4. Resumo do laboratório 4: Construindo Arquiteturas no Azure](#4.-Resumo-do-laboratório-4:-Construindo-arquiteturas-no-Azure)</br>
[5. Resumo do laboratório 5: Consfigurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure](#5.-Resumo-do-laboratório-5:-Consfigurando-recursos-e-dimensionamentos-em-máquinas-virtuais-na-Azure )</br>


### 1. Resumo do laboratório 1: Localizando serviços por categoria
Foi acessado o portal da Microsoft Azure. 
Em configurações do portal, pode ser trocado o idioma e a aparência do portal.  
Em todos os serviços, são mostrados os serviços por categoria, que inclui, entre outras: </br> 
-	IA + Machine Learning </br>
-	Bancos de dados </br>
-	Computação </br>
-	Contêiners </br>

Em todos os serviços/rede, pode ser acessado o **Bastions**, que é uma rede segura para fazer acesso às máquinas (Jump Server). </br>
Os serviços em versão prévia são aqueles que estão começando a ser disponibilizados e testados, eles não têm SLA(acordo de nível de serviço)

### 2. Resumo do laboratório 2: Criando máquinas virtuais Azure 

Foi visto o tempo de inatividade para cada porcentagem no SLA (acordo de nível de serviço). Percebe-se que não há a possibilidade de 100% de disponibilidade do serviço. O cliente deve escolher o que melhor lhe atende. Ver figura abaixo:  </br> 

<img src = https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/SLA.PNG>

Para criar uma máquina virtual, é necessário ir em *Todos os serviços/computação/Infraestrutura como serviço/máquinas virtuais*. </br>
Ao criar uma máquina virtual, é necessário escolher a região, opções de disponibilidade, zona de disponibilidade, entre outras opções. 
A interface conta com informações e dicas nos itens para auxiliar o usuário. </br>
Foi mostrada a possibilidade de criar armazenamentos para redundância em local (LRS), em zonas (ZES), entre outros.  

### 3. Resumo do laboratório 3: Configurando uma instância de banco de dados Azure 
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

### 4. Resumo do laboratório 4: Construindo arquiteturas no Azure

No laboratório foi mostrado sobre a replicação em regiões que são oferecidas pelo Azure. Exemplos: </br>

- Brazil South: Data replication to the US
- Brasil Southeast: Data replication to the Brazil South

Foi explorado o site da Microsoft para visualizar as regiões e datacenters </br>
Link para visualizar os datacenters da Microsoft: 
- 🔎 [Microsoft Datacenters](https://datacenters.microsoft.com/globe/explore/)

Foi criado o grupo de recursos em *Todos os serviços/grupo de recursos*. A região escolhida foi **(US) East Us**. 
As **Marcações** servem para identificar o grupo de recursos. </br>
Foi explicado sobre IAM (controle de acesso) e eventos. </br>
Foi criada uma rede virtual na região **South America (Brasil South)**, que foi incluída no grupo de recursos criado. 


### 5. Resumo do laboratório 5: Consfigurando recursos e dimensionamentos em máquinas virtuais na Azure 

<ins>**Criação de máquina virtual**</ins>  </br>

<ins>Configuração básica</ins>  </br>
Em *Assinatura/Grupo de recursos* foi utilizado o grupo de recursos criado no lab.4. </br>
A região utilizada foi a **(US) East US 2**. </br>
Em *Opções de disponibilidade*, entramos na configuração *Criar um conjunto de dimensionamentos de máquinas virtuais* e vimos algumas configurações de escala em *Adicionar uma condição de escala*, opção *Dimensionamento automático*. </br>
Esse recurso permiti dimensionar a escalabilidade horizontal da nossa máquina virtual, configurando um número mínimo e máximo de instâncias e qual a porcentagem de uso da CPU para haver aumento e diminuição das instâncias.  </br>
**Importante:** O valor padrão de duração da consulta é 10 min.  </br> 

A opção de disponibilidade escolhida foi a *Nenhuma redundância infraestrutura necessária*. Assim, a primeira configuração ficou como mostrado abaixo. 

<img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/vm1.PNG >

*Desconto Spot do Azure* permite que os recursos da Azure sejam usados com um preço muito mais em conta, contudo, caso alguém queira usar esses recursos pagando o preço normal, os serviços são desabilitados e passados para a outra pessoa. </br>
Foram mostrados alguns tamanhos de VM. O tamanho escolhido foi o **Standart_DS1_v2 – 2 vcpu, 3.1GiB**. </br>
Foi configurado um usuário e senha.  </br>

Em regras de portas de entrada foi selecionado *Permitir portas secionadas* e a porta de entrada selecionada foi a **RDP(3389)**. </br>
O intuito da escolha da porta era pegar alertas, pois ela deixa a máquina virtual exposta para a internet.  Essa parte da configuração ficou mostrado abaixo:

<img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/vm2.PNG >

<ins>Configuração de disco</ins> </br>
A parte de configuração de disco ficou como é mostrado na figura seguinte. </br>
Deve-se ter cuidado e deixar a opção **Excluir com VM** selecionado. Assim, quando a vm for excluída, o disco também será, evitando custos adicionais. 

<img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/vm3.PNG >

<ins>Configuração de rede</ins> </br>
A configuração de rede ficou como mostrado nas imagens seguintes. </br>

<img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/vm4.PNG >
<img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/vm5.PNG >

<ins>Configuração de gerenciamento</ins> </br>
Foi configurado o horário de desligamento automático e um e-mail de notificação.  </br>
Não foi configurada a opção de backup para fins didáticos. Mas é importante de lembrar de habilitá-lo sempre. 

<ins>Configuração de monitoramento</ins> </br>
Os alertas não foram configurados. Mas é possível configurar regras de alertas baseados em diversas métricas, como porcentagem de CPU, memória disponível, entro outros. </br>
A parte de monitoramento ficou como mostrado abaixo.

<img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/vm6.PNG >

<ins>Revisar + criar</ins> </br>
Nessa opção é dada uma estimativa de custo de uso da máquina virtual por hora. </br>

</br>

<ins>**Criação de área de trabalho virtual** </ins>  </br>
A criação da área de trabalho virtual é realizada em *Todos os serviços/Área de Trabalho Virtual Azure*. </br>

<ins>Noções básicas</ins>  </br>
A primeira etapa da configuração ficou como mostrado nas imagens abaixo. 
O tipo de pool de hosts **Pessoal** é indicado para uma pessoa que mexa com um software específico. Caso contrário é indicado a opção **Em pool** (grupo).  

<img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/atv1.PNG >
<img src =  https://github.com/TiagoPaulino22/resumo-do-lab-azure/blob/main/imagens/atv2.PNG > 

</br>

### 🔎 Links úteis
- [Link para laboratórios no site da Microsoft](https://learn.microsoft.com/pt-br/training/)




















