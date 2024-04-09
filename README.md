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

