# resumo-do-lab-Azure
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab Dio.


*As a service:* Modelo de negocio que ao invés de adquirir um produto, contratamos um serviço do que será cobrado de acordo com a utilização.
Exemplo:
- Produto - Máquina de lavar
- As a service - Lavanderia

*On-premise:* Ambiente no local privado

*Nuvem:* Acessar contéudos através da internet em maquinas não estão localmente. (ambiente cloud)

*Hybrid Model:* Possui produtos on-premisse, porém em momentos especificos se faz necessário as a service, modelo de negocios sazional.

*Infra as a Service (Iaas):* Alugar infraestrutura de outra empresa para consumir recursos.

*Plataforms:* Empresas com infraestrutura completa que vendem ambinetes para outras empresas.
Exemplo:
- AWS
- Azure
- Oracle
- GCP (google)a

*Regions e Zones*:
- Regions: Lugres diferentes do mundo que possui maquinas para serem alugadas (SA-EAST1: SÃO PAULO,BRASIL)
Areas diferentes dentro de uma região (SA-EAST1a)

*Computação em Nuvem:* É o fornecimento de serviços de computação pela internet, habilitando inovações mais rápidas, recusos flexíveis e economias de escala.

*Nuvem privada:* On Premisse - Capex (adquire e é responsavél por todo o hardware)
- As organizações criam um ambiente em nuvem em seu datacenter.
- As organizações são responsáveis por oprerar os serviços que fornecem.
- Não fornece acesso aos usuários fora da organizações (apenas com VPN)

*Nuvem pública:* Opex (modelo fatura mensal)
- Pertencente a serviços de nuvem ou provedor de hosting.
- Fornece recursos e serviços a várias ortganizações e usuários.
- Acessada via conexão de rede segura (geralmente pela Internet)

*Nuvem Híbrida:* Combina nuvens públicas e privadas para permitir que os aplicativos sejam executados.

*CAPEX x OPEX:*

- Depesas de capital (CAPEX)
O gasto inicial em Infra física
As despesas do CAPEX tem um valor que reduz c/ tempo (depreciação)

- Depesas operacionais (OPEX)
Gastar com produtos e serviços conforme necessário, pagamento conforme o uso.
Cobrado imediatamente

*Benefícios da Nuvem:*
- Alta disponibilidade: manter o serviço sempre disponivel
- Escalabilidade: Capacidade de elevar o total
- Elasticidade: Compartamento que oscila (períodos sazionais)
- Confiabilidade: Permite medir cada byte trafegado
- Gerenciabilidade: Contro abrangente
- Governança: Cria normas
- Segurança: Microsoft Defender Cloud
- Previsibildade: Custo mensal de utilização

#Tipos de serviços de nuvem#

*Iaas (infra as a service):* Crie uma infraestrutura de TI de pagamento conforme o uso alugando servidores, máquinas virtuais, armazenamento, redes e sistemas operacionais de um provedor de nuvem.
I- Armazenamento
II- Redes virtuais
III- Máquinas virtuais

*Paas (Plataform as a Service):* Fornece um ambinete para a criação, o teste e a implantação de aplicativos de software, sem forcar no gerenciamento da infraestrutura subjacente.
Garente o funcionamento, desenvolvedor se concentra a escrever o código, sistema operacional utilizado e frameworks com mais performance, o resto está sob a gestão do Paas (plataforma)

*Saas (software as a service):* Os usuários se concetam e usam aplicativos com base em nuvem pela internet: por exemplo Canva, Trello, Office 365, e-mail e calendarios.

#Modelos de responsabilidade compartilhada#

- Saas: Vai de Uber
- Paas: Alugue um carro na locadora
- Iaas: Alugue um carro e pague os custos (aluguel por dia)
- On premisse: Tenha um carro e pague 
IPVA
Manutenção
Estacionamento
Multa

#Componentes de arquitetura do Azure#

*Regiões:* Local que tem uma ou mais datacenters. Ponto geogratico que possui 3 zonas de disponibilidade.

*Zonas de disponibilidade:* 3 data centers dentro de cada região

*Pares de regiões:* replicação automatica de uma região para outra com no minimo 300 milhas de distancia (como se fosse um bkp)

*Regiões soberanas do Azyre (Serviço governamentais do EUA):* Atende as necessidade de segurança e conformidade das agências federais, governos estaduas e locais dos EUA e seus provedores de soluções.

*Azure governamental:* Instância separada do Azure. Fisicamente isolda de implatanões que não sejam do governo dos EUA. Acessivel somente por pessoas verificadas e autorizadas.

*Recusros do Azure:* Os recursos da Azure são componentes como armazenamento, máquinas virtuais e redes que estão disponíveis para criar soluções de nuvem.
Um grupo de recursos pe um conteiner que você usa para gerencias e agregar recursos em uma única unidade.
- Os recursos podem existir em apenas um grupo de recursos.
- Os recursos podem existir em diferentes regiões.
- Os recursos podem-ser movidos para diferentes grupos de recursos.
- Os aplicativos podem utilizar vários grupos de recursos.

*Assinaturas do Azure e grupos de gerencimanento:* Vem antes do grupo de recurso e fornece acesso autentico e autorizado as contas do Azure

#Computação e rede#

*Serviços de computação do Azure:* A computação do Azure é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memórias, rede e sistemas operacionais.
- Virtual machine
- Aplicativos/Serviços
- Contêiners/Instâncias
- Servicos de Kubenets di Azure (AKS)
- Area de trabalho virtual (vm)

- As máquinas virtuais do Azure (Vms) são emulações de software de computadores físicos
Inclui processador virtual, memória, armazenamento e rede

- Oferta de Iaas que ogerece personalização e controle total

*Serviços de contêiners do Azure:* Os conteiners do Azure fornecem um ambinete leve e virtualizado que não exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda.

- Instâncias de contêiners do Azure: uma oferta de Paas que executa um contêiner ou pod de contêiners no Azure
- Aplicativos de contêiners do Azure: uma oferta de Paas, como instâncias de contêineers que pode balancear a carga e escalar.
- Serviços de Kubernets do Azure: um serviço de orquestração para contêiners com arquiteturas distribuidas e grandes volumes de contêiners.

*Azure functions:* Uma oferta de Paas que da suportes a operações de computação sem servidor. O código baseado em eventos é executada quando chamado, sem exigir uma infra de servidor durante períodos inativos.

*Serviços de aplicativos do Azure:* Os serviços de aplicativos do Azure consistem em uma plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos Web e APIs rapidamente.
- Trabalha com .NET, .NETCORE, NODE.JS, Java, Python ou PhP
- Oferta de Paas com requisitos de nível coorporativo de desempenho, segurança e conformidade.

*Serviço de rede do Azure:* A rede virtual do Azure (Vnet) permite que os recursos do Azure se comuniquem uns com os outros, com o Internet e com as redes locais.
- Pontas de extremidade públicos, acessíveis de qualquer lugar na internet.
- Pontas de extremidade privadas, acessíveis somente de dentro da sua rede.
- As sub-redes virtuais sementam sua rede para atender as suas necessidades.
- O emparelhamento de rede conecta suas redes privadas diretamente

*DNS do Azure - Domain Server name*
- Confiabilidade e desempenho aprovetando uma rede global de servidores de nome DNS usando a rede Anyscat
- A segurança do DNS do Azure baseia-se no gererenciador de recurso do Azure, habilitando o controle de acesso baseado em função e o monitoramento e o registro em log.
- Facilidade de uso para gerenciar seus recursos externos e da Azure com um único serviço, DNS.
- As redes vituais personalizáveis permitem que você use nomes de dominio privados e totalmente perfonalizados em suas redes virtuais privadas.
- Os registrosd de alias dão suporte a conjunto de registros de alias para apontar diretamente par aum recurso do Azure.
