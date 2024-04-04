# CRIANDO GRUPO DE RECURSOS NO AZURE
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Bongiorno14/Criando_RecourseGroup_Azure/blob/main/LICENSE) 

# OVERVIEW

Antes de mergulhar nos detalhes técnicos, é essencial entender o papel crucial que os Resource Groups desempenham na estrutura do Azure. Um Resource Group é um contêiner lógico que agrupa recursos relacionados para facilitar o gerenciamento, implantação e monitoramento dentro de um ambiente de nuvem. Ao organizar recursos em Resource Groups,tem se alguns beneficios, tais como:

- Organização Lógica: Agrupamento de recursos por projeto, equipe ou função para uma melhor organização e navegação.
- Gerenciamento Simplificado: Realizaçao de operações em lote, como implantação, atualização e exclusão, em todos os recursos de um grupo de uma vez.
- Governança e Segurança: Aplicação de políticas e permissões específicas a um Resource Group para garantir conformidade e segurança.

A lista certamente é maior que esta, porém atentei para estes 3 tópicos.

# DETALHAMENTO DA CRIAÇAO E CONFIGURAÇÃO

## Introdução ao Azure Resource Group
O que é um Resource Group?
- Benefícios e finalidade do Resource Group no Azure.
- Passos para Criar um Resource Group

## Criando um Resource Group via Portal do Azure.
Utilizando a CLI do Azure para criar um Resource Group.
- Exemplos de templates ARM para automação de criação de Resource Groups.
- Configurações Avançadas e Nuances

## Gerenciamento de permissões e acessos no Resource Group.
Tags e marcações para organização e gerenciamento eficiente.
- Definição de políticas de governança para o Resource Group.
- Recursos Agregados na Criação do Resource Group

## Implementação de Virtual Networks (VNets) dentro do Resource Group.
Criação de Máquinas Virtuais (VMs) e Armazenamento associado.
- Uso de Grupos de Segurança de Rede (NSGs) para controle de tráfego.
- Ferramentas e Referências Úteis

# UPDATE NO APRENDIZADO  DE CRIAÇAO DE MÁQUINAS VIRTUAIS.

Após o parofundamento do aprendizado, seguem um update no conteudo de criação de máquinas virtuais, com o detalhamento de algumas configurações importantes.
## Definiçao
Máquinas virtuais (VMs) são ambientes de computação virtual que funcionam como se fossem computadores físicos completos, incluindo hardware e software. No entanto, em vez de dependerem de hardware físico, as VMs são criadas em software e podem ser executadas em um único servidor físico ou em uma infraestrutura em nuvem, no caso de estudo o Azure.
As VMs são criadas usando um software chamado hipervisor, que permite a criação e execução de múltiplas máquinas virtuais em um único servidor físico. Cada VM tem seu próprio sistema operacional, aplicativos e recursos dedicados, mas compartilha os recursos físicos do servidor subjacente de forma virtualizada.

## Tamanho e Configuração:
- Escolha do tipo de VM: Determina a capacidade de processamento, memória e armazenamento da máquina virtual, com opções como geral, otimizada para computação, memória otimizada, etc.
- Tamanho da VM: Define a quantidade de vCPUs, RAM e armazenamento disponíveis para a máquina virtual, com opções que variam de pequenas a grandes instâncias.

## Modelos de Trabalho:
- VMs dedicadas a funções específicas: São configurações pré-definidas otimizadas para cargas de trabalho específicas, como desenvolvimento, produção, teste, entre outras.
- VMs otimizadas para diferentes cargas de trabalho: Podem ser configuradas para processamento em lote, análise de dados, aplicações web, etc.

## Escalabilidade e Condições:
- Escalabilidade automática: Permite que a quantidade de recursos (como vCPUs e RAM) seja ajustada automaticamente com base em métricas predefinidas, como utilização da CPU.
- Condições de escalabilidade: Define critérios para escalar verticalmente (aumentando os recursos da VM) ou horizontalmente (adicionando mais instâncias da VM).

## Regras para Portas de Entrada:
- Firewall e regras de rede: Permite configurar regras de firewall para controlar o tráfego de entrada e definir quais portas e protocolos são permitidos ou bloqueados.

## Sistemas Operacionais e Gerenciamento de Chaves:
- Seleção de sistemas operacionais: Permite escolher entre Windows Server, várias distribuições Linux, etc.
- Gerenciamento de chaves: Configura chaves SSH para acesso seguro a VMs Linux e chaves RDP para VMs Windows, garantindo a segurança dos acessos.

## Interfaces de Rede e Balanceamento de Carga:
- Interfaces de rede: Define as configurações de rede, como IP, sub-rede, gateway, etc., para comunicação interna e externa da VM.
- Balanceamento de carga: Distribui o tráfego entre várias instâncias de VMs para otimizar o desempenho e garantir alta disponibilidade.

## Gerenciamento de Identidades:
- Integração com Azure Active Directory: Permite gerenciar identidades de usuários e aplicar políticas de acesso baseadas em funções.
- Políticas de acesso: Define permissões e restrições de acesso com base em papéis e responsabilidades dos usuários.

## Monitoramento:
- Azure Monitor: Oferece ferramentas para monitorar o desempenho das VMs, coletando métricas como CPU, memória, disco, etc., e gerando alertas em caso de problemas.

## Adicionar Extensões:
- Extensões: São módulos que adicionam funcionalidades extras às VMs, como monitoramento de agentes, ferramentas de segurança, etc.

## Tags e Categorização:
- Tags: Permitem categorizar e organizar as VMs em grupos lógicos, facilitando a gestão, identificação e rastreamento das instâncias dentro do ambiente Azure.

# UPDATE II - ARMAZENAMENTO NO AZURE

Primeiro ponto importante, a escolha da redundância.
PS: Durante o processo de criaçao, o nome deste é como um CPF, único e intransferível.

## LRS (Locally Redundant Storage):
- O LRS replica seus dados dentro de uma região do Azure para proteção contra falhas de hardware ou interrupções de serviço localizadas. Por exemplo, se você armazenar dados em um contêiner de blobs com redundância LRS em uma região específica, o Azure replicará esses dados três vezes dentro dessa região.
- Exemplo de utilização: Armazenamento de backups de máquinas virtuais para recuperação de desastres dentro da mesma região.

## ZRS (Zone Redundant Storage):
- O ZRS replica seus dados em zonas de disponibilidade diferentes dentro de uma região do Azure, oferecendo proteção adicional contra falhas de zona devido a desastres naturais ou interrupções em uma zona específica. Por exemplo, ao usar ZRS para armazenar dados, o Azure replica esses dados em três zonas de disponibilidade diferentes dentro da mesma região.
- Exemplo de utilização: Armazenamento de dados críticos para aplicativos de alta disponibilidade que exigem resiliência em várias zonas de disponibilidade.

## GRS (Geo-Redundant Storage):
- O GRS replica seus dados de forma síncrona em uma região primária e de forma assíncrona em uma região secundária distante para proteção contra desastres regionais. Por exemplo, se você usar GRS para armazenamento, o Azure replicará seus dados em LRS na região primária e em outra região geograficamente distante para failover em caso de desastres.
- Exemplo de utilização: Armazenamento de dados críticos que exigem recuperação rápida em uma região secundária em caso de falha na região primária.

## GZRS (Geo-Zone Redundant Storage):
- O GZRS é uma combinação do ZRS e GRS, oferecendo redundância em zonas de disponibilidade e também em regiões geograficamente distantes. Ele replica seus dados de forma síncrona em zonas de disponibilidade dentro da região e de forma assíncrona em uma região secundária distante.
- Exemplo de utilização: Armazenamento de dados críticos para aplicativos altamente resilientes que exigem redundância em várias zonas de disponibilidade e em regiões diferentes para proteção contra desastres regionais.

## TIPOS DE ARMAZENAMENTO
### Azure Blob Storage
- O Azure Blob Storage é um serviço de armazenamento de objetos escalável e durável, projetado para armazenar grandes quantidades de dados não estruturados, como imagens, vídeos, arquivos de backup e logs. Ele oferece redundância para alta disponibilidade dos dados, incluindo:
- Redundância localmente redundante (LRS): Os dados são replicados dentro de uma região do Azure, garantindo alta disponibilidade dentro dessa região.
- Redundância georreplicada (GRS): Além da replicação dentro da região, os dados também são replicados de forma síncrona para uma região secundária distante para proteção contra desastres naturais ou falhas em larga escala.

### Azure Disk Storage
- O Azure Disk Storage fornece discos persistentes que podem ser anexados a máquinas virtuais (VMs) no Azure. Ele oferece três tipos de discos:
- Discos gerenciados padrão: São discos HDD (Hard Disk Drive) tradicionais para cargas de trabalho com baixo custo e baixo desempenho.
- Discos gerenciados Premium SSD: Oferecem alto desempenho e baixa latência, ideais para aplicativos que exigem I/O intensivo.
- Discos gerenciados Ultra Disk: São discos de armazenamento de alto desempenho e baixa latência, otimizados para cargas de trabalho de missão crítica.

### Azure Queue Storage
- O Azure Queue Storage é um serviço de fila de mensagens que permite a comunicação assíncrona entre componentes de aplicativos distribuídos. Ele oferece:
- Filas padrão: Garante a entrega de mensagens pelo menos uma vez e suporta um modelo de entrega de mensagens FIFO (First-In-First-Out).
- Filas de mensagens prioritárias: Oferece suporte a priorização de mensagens para aplicativos que exigem entrega rápida de mensagens críticas.

### Azure File Storage
- O Azure File Storage é um serviço de armazenamento de arquivos totalmente gerenciado, que permite compartilhar arquivos entre várias instâncias de VMs e sistemas operacionais. Ele oferece:
- Camada Hot: Ideal para arquivos frequentemente acessados e que exigem baixa latência.
- Camada Cool: Mais econômica, adequada para arquivos de backup e arquivamento que não são acessados com frequência.

### Azure Table Storage
- O Azure Table Storage é um serviço de armazenamento NoSQL altamente escalável, adequado para armazenar dados estruturados e semi-estruturados, como dados de aplicativos da Web e IoT. Ele oferece:
- Particionamento e dimensionamento automático: Permite escalonamento horizontal dos dados para lidar com cargas de trabalho em constante crescimento.
- Suporte a grandes volumes de dados: Capaz de armazenar petabytes de dados de maneira eficiente e econômica.

## Camadas de Acesso
O Azure oferece camadas de acesso para otimizar o desempenho e reduzir custos:
- Camada de acesso quente (Hot access tier): Ideal para dados frequentemente acessados, com custo mais alto de armazenamento, mas menor custo de acesso.
- Camada de acesso frio (Cool access tier): Mais econômica para dados raramente acessados, com custo mais baixo de armazenamento, mas custo mais alto de acesso.
- Camada de arquivo de arquivo (Archive access tier): Destinada a dados de arquivo inativos, com custo de armazenamento extremamente baixo, mas custo alto de acesso e recuperação.

# UPDATE III - SEGURANÇA E IDENTIDADE NO AZURE

Um pequeno overview de alguns serviços referentes a questoes de segurança, abordando também alguns detalhes do Microsoft Entra Conect e Microsoft Defender for Cloud.

## Recursos de Segurança e Identidade no Azure:

### Azure Active Directory (Azure AD):
- Centraliza o gerenciamento de identidades e acesso para usuários, grupos e aplicativos.
- Oferece autenticação multifatorial (MFA) para camadas adicionais de segurança.
- Integra-se com serviços do Azure e aplicativos de terceiros.

### Azure Security Center:
- Fornece visibilidade e controle sobre o ambiente de nuvem, identificando ameaças potenciais.
- Oferece recomendações de segurança baseadas em práticas recomendadas.
- Permite a configuração de políticas de segurança e detecção de anomalias.

### Azure Sentinel:
- Plataforma de gerenciamento de informações e eventos de segurança (SIEM).
- Oferece detecção avançada de ameaças e análise de segurança.
- Integra dados de vários serviços e fontes para correlacionar informações e identificar padrões suspeitos.

### Azure Firewall:
- Fornece uma camada adicional de segurança para proteger redes virtuais no Azure.
- Controla o tráfego de entrada e saída com base em regras de segurança.
- Suporta integração com serviços de segurança de terceiros.

### Azure Information Protection:
- Ajuda a proteger dados confidenciais aplicando políticas de classificação e rotulagem.
- Oferece criptografia e controle de acesso com base nas políticas definidas.

### Azure Key Vault:
- Gerencia e protege chaves de criptografia, segredos e certificados.
- Oferece controle de acesso granular e auditoria para chaves e segredos.

## Microsoft Defender for Cloud:

### Proteção de Workloads:
- Monitora e protege máquinas virtuais, contêineres e serviços como Azure Kubernetes Service (AKS) contra ameaças.
- Oferece detecção de ameaças em tempo real e respostas automatizadas.

### Proteção de Aplicativos:
- Analisa o código e o comportamento das aplicações em busca de vulnerabilidades e ameaças.
- Integra-se ao pipeline de desenvolvimento para segurança contínua.

### Proteção de Identidades:
- Detecta e responde a atividades suspeitas relacionadas a identidades de usuário.
- Oferece insights para fortalecer a postura de segurança das identidades.

### Proteção de Dados:
- Monitora e protege dados confidenciais em ambientes Azure e híbridos.
- Aplica políticas de prevenção contra perda de dados (DLP) e criptografia.

## Microsoft Entra Connect

### Gerenciamento de Identidade:
- Centraliza o gerenciamento de identidades e acesso para usuários, grupos e aplicativos em um diretório baseado na nuvem.
- Permite a criação, edição e exclusão de contas de usuário, além de definir políticas de senha e autenticação.

### Autenticação e Autorização:
- Oferece autenticação multifatorial (MFA) para uma camada adicional de segurança.
- Suporta diferentes métodos de autenticação, como senha, autenticação baseada em certificados, autenticação biométrica e muito mais.
- Permite o gerenciamento de permissões e acesso com base em funções (RBAC) para recursos e aplicativos.

### Sincronização de Diretórios:
- Oferece opções de sincronização entre o Azure AD e diretórios locais, como Active Directory local, para manter consistência nas identidades e políticas.
- Suporta o Azure AD Connect para integração e sincronização de identidades entre ambientes locais e na nuvem.

### Gerenciamento de Aplicativos:
- Facilita o acesso seguro a aplicativos em nuvem e locais usando o Azure AD como provedor de identidade.
- Oferece integração com milhares de aplicativos SaaS (Software as a Service) por meio da Galeria de Aplicativos do Azure AD.
- Permite o gerenciamento de acesso condicional com base em políticas de segurança.

### Proteção de Identidade:
- Detecta e responde a atividades suspeitas e ameaças de segurança relacionadas a identidades de usuário.
- Fornece insights sobre a postura de segurança das identidades e recomendações para melhorias.

### Integração com Outros Serviços Microsoft:
- Integra-se nativamente com outros serviços Microsoft, como Microsoft 365, Azure Information Protection, Microsoft Defender for Identity, entre outros, para oferecer uma segurança abrangente.

### Relatórios e Auditoria:
- Oferece relatórios e análises detalhadas sobre atividades de usuários, autenticações, aplicativos acessados e muito mais para fins de auditoria e conformidade.
- Suporta integração com ferramentas de gerenciamento de segurança e SIEM (Security Information and Event Management).

### Segurança Avançada:
- Oferece recursos avançados de segurança, como detecção de ameaças avançadas, prevenção contra perda de dados (DLP) e proteção contra acessos não autorizados.

# Aprendizado

- Tive a oportunidade de explorar a criaçao destas ferramentas, e um ponto importante.. A atençao aos detalhes é primordial para a escolha das opçoes em cada ferramenta.
- Tambem quero ressaltar a facilidade da criaçao, e a didática que o Azure te conduz em cada processo.

## Update

- Com o aprofundamento do aprendizado nas VMs, pude verificar a quantidade de personalizaçao que existe apenas neste serviço.
- AS configuraçoes atendem a necessidades muito especificas conforme cada projeto.

## Update II

- Muitos detalhes podem ser configurados e ajustados conforme a necessiade durante todo o processo de criaçao e gerenciamento dos armazenamento
- Potencial para explorar ferramentas de migraçao de Dados.

## Update III
- Questoes de segunraça tem um abordagem muito crítica, tendo inumero serviços para cada situaçao específica.
  
