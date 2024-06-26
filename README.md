# GOVERNANÇA NO AZURE
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Bongiorno14/Governa-a_Azure/blob/main/LICENSE) 

Neste projeto faço uma breve descriçao das 2 calculadoras para estimativas nos custos dos serviços da plataforma Azure.
Tive a oportunidade de fazer uma simulaçao, porem considerando valores arbitrários para cada estimativa.
Um ponto importante sobre estas estimativas é de que elas devem utilizadas como referências, sendo necessária de fato a colocaçao em funcionamento de todos os serviços para de fato sabermos o valor real.
Mas certamente esta referencia nos atenderá muito bem, caso queiramos decidir ou nao seguirmos com o projeto.

## OVERVIEW CALCULADORA TCO.

A calculadora TCO do Azure é uma ferramenta que permite às organizações estimar os custos totais de propriedade ao migrar cargas de trabalho para a plataforma Azure da Microsoft. Ela ajuda a avaliar os custos em várias dimensões, incluindo custos de infraestrutura, custos de operação, custos de licenciamento e outros fatores relevantes.

Pontos a serem considerados:
- Entrada de Dados: A calculadora requer várias informações para realizar uma estimativa precisa. Isso inclui o tipo de carga de trabalho que será migrada (por exemplo, máquinas virtuais, bancos de dados, aplicativos web), a quantidade de recursos computacionais, a frequência de uso, entre outros.
- Análise de Cenários: Com base nas informações fornecidas, a calculadora permite criar diferentes cenários para análise. Por exemplo, é possivel comparar os custos de executar uma carga de trabalho no Azure com os custos de manter essa carga de trabalho em infraestrutura local.
- Estimativa de Custos: A calculadora usa algoritmos e modelos para calcular os custos esperados ao longo do tempo. Isso inclui custos iniciais de migração, custos de hardware e software, custos de armazenamento, custos de rede, custos de backup e recuperação, entre outros.
- Relatórios e Análises: Após inserir os dados e selecionar os cenários desejados, a calculadora gera relatórios detalhados que mostram os custos projetados ao longo do tempo. Esses relatórios incluem gráficos e tabelas que facilitam a compreensão das principais métricas, como custo total, custo por unidade de recurso, assim por diante.
- Revisão e Ajustes: Com base nos resultados da análise, os usuários podem revisar os dados e fazer ajustes conforme necessário. Isso pode incluir a modificação das configurações da carga de trabalho, a seleção de opções de licenciamento mais adequadas, a otimização do uso de recursos, entre outros.

## OVERVIEW CALCULADORA DO AZURE.

A Calculadora de Preços do Azure é uma ferramenta online fornecida pela Microsoft para ajudar os clientes a estimarem os custos associados ao uso dos serviços de nuvem do Azure. 

Alguns pontos a serem considerados nesta calculadora:
- Seleção de Serviços: A calculadora permite que você escolha entre uma ampla variedade de serviços oferecidos pelo Azure. Isso inclui computação, armazenamento, banco de dados, rede , entre outros.
- Configuração dos Serviços: Após selecionar os serviços desejados, é possivel configurar detalhes específicos, como o tipo e tamanho das instâncias de máquinas virtuais, a quantidade de armazenamento necessário, a região geográfica onde os serviços serão implantados, a frequência de uso dos recursos, entre outros parâmetros.
- Estimativa de Custos: Com base nas informações fornecidas, a calculadora gera uma estimativa dos custos associados ao uso dos serviços selecionados. Isso inclui custos de uso por hora, custos mensais estimados e custos anuais projetados. A calculadora também considera descontos por reserva de recursos e opções de pagamento antecipado.
- Comparação de Preços: A calculadora permite comparar os preços entre diferentes tipos de instâncias, opções de armazenamento, níveis de serviço e modelos de pagamento. Isso ajuda na escolha da combinação mais econômica de serviços para suas necessidades específicas.
- Simulações e Cenários: Além de estimativas simples, a calculadora permite criar cenários complexos e simulações para entender melhor o impacto de diferentes configurações nos custos.
- Otimização de Custos: Com base nos resultados da estimativa, é possivel ajustar as configurações dos serviços para otimizar os custos. Isso pode incluir escolher instâncias de máquinas virtuais mais econômicas, utilizar opções de armazenamento mais eficientes, entre outras estratégias.

## FERRAMENTAS
Links para as Calculadoras.
- <https://azure.microsoft.com/pt-br/pricing/tco/calculator>
- <https://azure.microsoft.com/pt-br/pricing/calculator>
- AZURE

## APRENDIZADO

- Tive a oportunidade de explorar a utilização desta ferramentas, fazer uma simulaçao e obter as estimativas, bem como os beneficios da utilizaçao das mesmas.
- Um ponto importante é a facilidade da obtenção das informações das estimativas, e o site é muito intuitivo, direto, e se caso tens alguma duvida, todo campo tem o ícone de informaçao adicional.

# UPDATE I - PORTAL DE CONFIANÇA DO SERVIÇO E MICROSOFT PURVIEW

Neste update fiz um pequeno resumo em conisderaçao ao site do Portal de Confiança do serviço, bem como algumas caracteristicas do Microsoft Purview.

## PORTAL DE CONFIANÇA
O Portal de Confiança do Serviço da Microsoft é uma plataforma que oferece transparência e informações detalhadas sobre as práticas de segurança, privacidade e conformidade da empresa. Vamos explorar seus principais aspectos:
- Certificações: O portal destaca as certificações obtidas pela Microsoft em relação a padrões de segurança e privacidade, como ISO 27001, SOC 1 e 2, HIPAA, GDPR e muitas outras. Essas certificações demonstram o compromisso da empresa em adotar práticas de segurança robustas.
- Regulamentos e Padrões: Além das certificações, o portal aborda os regulamentos e padrões de conformidade aos quais a Microsoft se compromete, como o GDPR na União Europeia, a Lei de Privacidade do Consumidor da Califórnia (CCPA) nos EUA e outros requisitos locais e globais.
- Relatórios de Conformidade: O portal disponibiliza relatórios detalhados sobre a conformidade dos serviços da Microsoft com os padrões e regulamentos mencionados. Isso inclui informações sobre controles de segurança implementados, auditorias realizadas e outras métricas relevantes.
- Recursos Regionais: Há também informações específicas sobre conformidade e segurança relacionadas a diferentes regiões do mundo. Isso inclui detalhes sobre como os dados são armazenados e processados em conformidade com as leis locais de proteção de dados.
- Recursos dos Setores: O portal oferece recursos direcionados a setores específicos, como saúde, educação, governo e outros. Esses recursos abordam requisitos e melhores práticas de segurança e privacidade relevantes para cada setor.

## MICROSOFT PURVIEW

O Microsoft Purview é uma plataforma de governança de dados desenvolvida pela Microsoft para ajudar as organizações a gerenciar e proteger seus dados de forma eficiente. Algumas funcionalidades:
- Descoberta de Dados: O Purview permite que as organizações descubram e identifiquem seus dados em diferentes fontes, incluindo nuvem, local e híbrida. Ele usa conectores pré-construídos para se integrar a uma variedade de sistemas de armazenamento de dados, como Azure Data Lake Storage, SQL Server, AWS S3, Oracle, entre outros.
- Classificação e Catalogação: Após a descoberta, o Purview ajuda a classificar e catalogar os dados com metadados detalhados, incluindo tags, tipos de dados, proprietários, políticas de uso, entre outros. Isso permite uma organização mais eficiente e uma compreensão clara do que cada conjunto de dados contém e como ele deve ser tratado.
- Governança de Dados: A plataforma oferece recursos robustos de governança de dados, permitindo que as organizações estabeleçam políticas de acesso, privacidade e conformidade para seus dados. Isso inclui o monitoramento de atividades de acesso aos dados, auditoria e a capacidade de impor políticas automatizadas para garantir o cumprimento das regulamentações.
- Colaboração e Insights: O Purview promove a colaboração entre equipes, permitindo que diferentes partes interessadas acessem e compartilhem informações sobre os dados de forma segura e controlada. Ele também fornece insights e análises sobre a qualidade dos dados, padrões de uso e tendências, ajudando as organizações a tomar decisões informadas sobre seus dados.
- Integração com Ecossistema Microsoft: Como parte do ecossistema Microsoft, o Purview se integra perfeitamente a outras soluções, como Azure Synapse Analytics, Power BI e Azure Data Factory, oferecendo uma abordagem completa para gerenciamento e análise de dados.

## FERRAMENTAS
- <https://servicetrust.microsoft.com/>
- <https://www.microsoft.com/pt-br/security/business/microsoft-purview>
- AZURE

## APRENDIZADO

- O entendimento acerca do Portal de confiança é de que necessitamos ter o correto entendimento das politicas e normas vigente para cada pais, para estarmos cobertos quanto aos polices necessários, procedimentos e regras de negócio.
- O Microsoft Purview vonsolida e gere todos os polices cada para regra de negócio.

# UPDATE II - CLOUD SHELL, POWER SHELL, AZURE ARC E MODELOS ARM. 

## Azure Cloud Shell:

- Azure Cloud Shell é uma interface de linha de comando baseada na nuvem que permite aos usuários acessar um ambiente de shell diretamente no navegador.
- O mesmo oferece suporte aos shells Bash e PowerShell.
- Vem pré-configurado com várias ferramentas e SDKs, como Azure CLI, Azure PowerShell, Terraform, etc.
- Permite o acesso a arquivos de armazenamento na nuvem para persistência de dados.
- Acessível de qualquer lugar com conexão à Internet.
- Não requer instalação local de ferramentas ou SDKs.
- Facilita a automação e a execução de tarefas administrativas no Azure.

## Azure PowerShell:

- Azure PowerShell é uma extensão do PowerShell que permite aos usuários gerenciar recursos do Azure usando scripts e cmdlets específicos do Azure.
- Fornece cmdlets para interagir com serviços, como criação, modificação e exclusão de recursos.
- Permite automação de tarefas complexas e repetitivas.
- Integrado com a autenticação do Azure para acesso seguro aos recursos.
- Integração nativa com outros serviços e ferramentas do Azure.
- Suporte para automação avançada e gerenciamento de infraestrutura como código.

## Azure Arc:

- Azure Arc é uma solução que estende os serviços de gerenciamento do Azure para ambientes externos, como data centers locais, infraestrutura multicloud e bordas de rede.
- Permite registrar e gerenciar recursos externos no Azure, como máquinas virtuais, Kubernetes e bancos de dados.
- Oferece recursos de governança, conformidade e segurança centralizados.
- Habilita a implantação de políticas e configurações consistentes em ambientes heterogêneos.
- Gerenciamento unificado de recursos em vários ambientes.
- Implementação de práticas de governança e segurança em ambientes distribuídos.
- Integração com ferramentas de automação e orquestração do Azure.

## Modelos ARM (Azure Resource Manager):

- Modelos ARM são arquivos JSON que definem a infraestrutura e a configuração de recursos no Azure de forma declarativa.
- Descreve recursos, dependências, propriedades e configurações em um formato legível por máquina.
- Permite a implantação consistente e repetível de recursos do Azure.
- Suporta a organização modular de recursos e a parametrização de configurações.
- Automação de implantação e gerenciamento de recursos.
- Documentação clara da infraestrutura como código.
- Validação prévia de configurações e dependências antes da implantação.

### Aspectos adicionais quanto aos modelos ARM

- Sintaxe Declarativa: Os modelos ARM usam uma sintaxe declarativa baseada em JSON (JavaScript Object Notation). Isso significa que você descreve o estado desejado da infraestrutura em vez de especificar uma série de etapas para alcançar esse estado.
- Resultados Repetíveis: Implementando o mesmo modelo várias vezes, o estado resultante da infraestrutura será sempre o mesmo, o que promove consistência e confiabilidade.
- Orquestração: É possivel definir dependências entre recursos, garantindo que sejam implantados na ordem correta.
- Arquivos Modulares:Pode-se dividir o modelo em partes menores e reutilizáveis. Isso facilita a manutenção, a colaboração em equipe e a organização lógica do código.

# UPDATE III - SERVIÇOS DE MONITORAMENTO

Uma abordagem dos 3 principaos serviços de monitoramento do Azure:

## Azure Advisor:

- O Azure Advisor é um serviço de otimização que fornece recomendações personalizadas para ajudar a melhorar a segurança, confiabilidade, desempenho e eficiência dos recursos implantados no Azure.
- Ele analisa as configurações e o uso dos recursos para identificar oportunidades de economia de custos, otimização de desempenho e aprimoramento da segurança.
- As recomendações do Azure Advisor abrangem áreas como configurações de segurança, disponibilidade de VMs, dimensionamento de recursos, otimização de custos e atualizações de serviço.

## Azure Monitor:

- O Azure Monitor é uma plataforma de monitoramento abrangente que coleta e analisa dados de vários recursos do Azure, como VMs, aplicativos Web, bancos de dados e muito mais.
- Ele fornece insights em tempo real sobre o desempenho e a integridade dos recursos, permitindo a detecção precoce de problemas e a resolução proativa de incidentes.
- O Azure Monitor oferece recursos como monitoramento de métricas, logs, alertas, dashboards personalizados e integração com ferramentas de terceiros.

## Azure Resource Health:

- O Azure Resource Health é um serviço que fornece informações sobre a integridade e a disponibilidade dos recursos implantados no Azure.
- Ele ajuda a monitorar o status operacional dos recursos e a identificar se há problemas afetando sua disponibilidade.
- O Azure Resource Health oferece insights sobre a causa raiz de problemas, informações de status em tempo real e recomendações para resolver problemas de integridade.
