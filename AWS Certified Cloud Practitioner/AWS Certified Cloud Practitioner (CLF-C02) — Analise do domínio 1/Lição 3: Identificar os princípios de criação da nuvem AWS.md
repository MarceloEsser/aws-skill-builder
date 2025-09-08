# Lição 3: Identificar os princípios de criação da nuvem AWS

## Introdução

Vamos começar com a segunda declaração de tarefa, identificar os princípios de criação da AWS. Um foco principal para esta declaração de tarefa é o AWS Well-Architected Framework. Para este exame, tenha uma compreensão de como usar o AWS Well-Architected Framework para projetar e criar ambientes resilientes, altamente disponíveis e otimizados para custos.

## O que é o AWS Well-Architected Framework?

O AWS Well-Architected Framework contém princípios, práticas recomendadas e estratégias fundamentais para arquitetar sistemas na nuvem. Ele ajuda você a projetar, criar e operar sistemas confiáveis, seguros, eficientes e econômicos que aumentarão sua probabilidade de sucesso.

O AWS Well-Architected Framework é baseado em seis pilares:
- Excelência operacional
- Segurança
- Confiabilidade
- Eficiência de desempenho
- Otimização de custos
- Sustentabilidade

### Princípios Gerais de Criação

O Well-Architected Framework também identifica um conjunto de princípios gerais de criação para facilitar projetos de boa qualidade na nuvem que são os seguintes:

- Parar de adivinhar sua capacidade
- Usar o auto scaling para garantir que seu fornecimento atenda à sua demanda
- Testar sistemas em escala de produção
- Automatizar sua arquitetura e isso torna a experimentação mais fácil
- Permitir mudanças evolutivas e usar dados para fazer as mudanças necessárias
- Melhorar durante os dias de jogo e executar testes para ver seus sistemas em nível de produção

### Ferramenta AWS Well-Architected

Você pode estar se perguntando, "Julie, por que isso é importante? Por que estamos discutindo a computação em nuvem e o Well-Architected Framework?" O motivo é que isso dá a você uma base sólida para compreender a AWS, e isso será benéfico para você dedicar algum tempo para aprender e entender esses conceitos fundamentais durante o exame.

A AWS também fornece uma ferramenta AWS Well-Architected com as práticas recomendadas para nos ajudar. Essa ferramenta analisa suas cargas de trabalho e as compara às práticas recomendadas mais recentes da AWS para projeto arquitetônico. E essas práticas recomendadas para projeto arquitetônico vêm diretamente do AWS Well-Architected Framework. Vou adicionar um link para o AWS Well-Architected Framework e também um link para a ferramenta, caso você queira se aprofundar.

## Os Seis Pilares do AWS Well-Architected Framework

### 1. Excelência Operacional

O primeiro pilar é Excelência operacional, que é a habilidade de dar suporte ao desenvolvimento e executar cargas de trabalho de modo eficiente, obter informações sobre as operações e melhorar continuamente os processos e procedimentos de suporte para proporcionar valor comercial.

**Há cinco princípios de criação para a excelência operacional:**
- Executar operações como código
- Fazer alterações frequentes, pequenas e reversíveis
- Refinar procedimentos operacionais com frequência
- Prever falhas
- Aprender com todas as falhas operacionais

### 2. Segurança

O pilar Segurança envolve a habilidade de proteger dados, sistemas e ativos para aproveitar as tecnologias de nuvem para melhorar sua segurança.

**Há sete princípios de criação para a segurança na nuvem:**
- Implementar uma base de identidade sólida
- Manter a rastreabilidade
- Aplicar segurança em todas as camadas
- Automatizar as práticas recomendadas de segurança
- Proteger os dados em trânsito e em repouso
- Manter as pessoas afastadas dos dados
- Preparar-se para eventos de segurança

### 3. Confiabilidade

O pilar Confiabilidade engloba a capacidade de uma carga de trabalho de executar a função pretendida corretamente e de forma consistente quando é esperado. Isso inclui a capacidade de operar e testar a carga de trabalho por meio de seu ciclo de vida total.

**Há cinco princípios de criação para a confiabilidade na nuvem:**
- Recuperar-se automaticamente de falhas
- Testar procedimentos de recuperação
- Dimensionar horizontalmente para aumentar a disponibilidade agregada da carga de trabalho
- Parar de adivinhar a capacidade
- Gerenciar mudanças na automação

### 4. Eficiência de Desempenho

O pilar Eficiência de desempenho inclui a capacidade de usar recursos computacionais com eficiência para atender aos requisitos do sistema e manter essa eficiência à medida que a demanda muda e as tecnologias evoluem.

**Há cinco princípios de criação para a eficiência de desempenho na nuvem:**
- Democratizar tecnologias avançadas
- Tornar-se global em minutos
- Usar arquiteturas serverless
- Experimentar com mais frequência
- Considerar a facilidade mecânica

### 5. Otimização de Custos

O pilar Otimização de custos inclui a capacidade de executar sistemas para entregar valor comercial com o menor preço. E abordaremos o pilar Otimização de custos em Domínio 4: Cobrança, preços e suporte.

### 6. Sustentabilidade

E o sexto pilar é a Sustentabilidade. Este pilar concentra-se nos impactos ambientais, especialmente no consumo e na eficiência de energia, porque são alavancas importantes para que os arquitetos informem a ação direta para reduzir o uso de recursos.

**Há seis princípios de criação para a sustentabilidade na nuvem:**
- Entender seu impacto
- Estabelecer metas de sustentabilidade
- Maximizar a utilização
- Prever e adotar ofertas de hardware e software novas e mais eficientes
- Usar serviços gerenciados
- Reduzir o impacto de distribuição de suas cargas de trabalho na nuvem

## Importância para o Exame

E garantir que você entenda as práticas recomendadas de todos os pilares também. O AWS Well-Architected Framework é muito importante no mundo real, para este exame e para a certificação AWS Certified Solutions Architect Associate.

Você provavelmente verá perguntas neste exame de certificação indagando quais princípios de design para requisitos ou casos de uso específicos você escolheria ao projetar sistemas ou soluções na AWS.

Portanto, reserve algum tempo para ler e criar soluções. Saiba como criar designs à prova de falhas, desacoplar seus componentes que reforçam o princípio de criação de arquitetura orientada a serviços, implementar elasticidade usando auto scaling, segurança e paralelização que são necessários para criar aplicações altamente dimensionáveis na AWS.

### Definição de Paralelização

Quero definir rapidamente a paralelização, porque acho que já defini os outros. O pensamento paralelo é semelhante ao desacoplamento, mas é como dividir um trabalho da forma mais simples e, então, distribuir essa carga para vários componentes para lidar com a demanda. E um exemplo seria dividir grandes conjuntos de dados em partes menores que podem ser processadas ao mesmo tempo e fornecer tempos de processamento mais rápidos.

## Conclusão

E voltando à nossa primeira lição, uma vantagem da AWS é conseguir se concentrar em serviços e designs, não em servidores e hardware, bem como na rápida implementação e lançamento desses recursos também.

Vamos começar com a terceira declaração de tarefa para entender os benefícios e estratégias de migração para a AWS.
