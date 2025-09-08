# Lição 4: Entenda os benefícios e as estratégias de migração para a nuvem da AWS

## Introdução

Vamos começar com a terceira declaração de tarefa para entender os benefícios e estratégias de migração para a AWS. Para esta declaração de tarefa, saiba como usar o AWS Cloud Adoption Framework e quais recursos podem ajudar a apoiar sua jornada de migração para a AWS.

## AWS Cloud Adoption Framework (CAF)

Em nossa última lição, sobre o AWS Well-Architected Framework, que é diferente do AWS Cloud Adoption Framework. O AWS CAF fornece uma abordagem abrangente para a nuvem e identifica capacidades organizacionais específicas para transformações bem-sucedidas na nuvem. Esses recursos oferecem orientações sobre práticas recomendadas e ajudam você a melhorar sua preparação para a nuvem. 

Essas capacidades são agrupadas em seis categorias:
- Negócios
- Pessoas
- Governança
- Plataforma
- Segurança
- Operações

Saiba como usar o AWS CAF para identificar e priorizar oportunidades de transformação, avaliar e aperfeiçoar sua preparação para a nuvem e desenvolver de modo iterativo seu roteiro de transformação.

### Benefícios do AWS CAF

Quais são os benefícios do uso dos serviços do AWS CAF? 

- **Reduzir o risco comercial** por meio do aumento da confiabilidade, do desempenho e da segurança
- **Aumentar sua eficiência operacional** reduzindo custos e aumentando a produtividade
- **Expandir** criando novos produtos e serviços para alcançar novos clientes ou novos mercados
- **Melhorar o desempenho** melhorando sua sustentabilidade e transparência

## Estratégias de Adoção da Nuvem

Quais são algumas estratégias de adoção da nuvem? Quando as organizações começarem a migrar para a AWS, elas poderão estar em diferentes estágios de adoção:

### Estágios de Adoção

1. **Fase de projeto**: quando você avalia se a migração para a AWS atenderia aos seus requisitos e necessidades específicos

2. **Estágio básico**: quando a migração para a AWS começa. Talvez você mova algumas aplicações de produção para a AWS ou implante um framework inicial na zona de pouso em um ambiente de não produção

3. **Estágio de migração**: quando você define funções para operações na nuvem, estabelece um Cloud Center of Excellence, também conhecido como CCOE, e se prepara para operações na nuvem de longo prazo, em vez de operações on-premises

4. **Estágio de reinvenção**: onde todos os novos projetos começam na AWS

Uma avaliação de ponto em que você e sua organização estão é concluída para entender qual o estágio de adoção você está antes do início da migração.

## Estratégias de Migração

Para o exame, saiba como identificar estratégias de migração adequadas, como replicação de banco de dados usando o AWS Database Migration Service ou o AWS Snowball. Falaremos sobre isso mais detalhadamente em uma lição posterior.

### As Sete Estratégias de Migração

Antes do exame, aprenda as sete estratégias de migração:

1. **Retirar**: para aplicações a serem desativadas ou retiradas

2. **Reter**: para aplicações que você quer manter no ambiente de origem ou aplicações que não estão prontas para migrar

3. **Redefinir hospedagem** (também conhecido como lift-and-shift): serve para migrar aplicações sem fazer nenhuma alteração na aplicação

4. **Realocar**: para um grande número de servidores que são compostos de uma ou mais aplicações

5. **Recomprar** (também conhecido como drop and shop): para aplicações com uma versão ou produto diferente e oferece mais valor do que a infraestrutura existente

6. **Redefinir a plataforma** (também conhecido como lift, tinker e shift e lift): para aplicações que precisam de algum nível de otimização para operar com eficiência ou aproveitar as vantagens dos recursos da AWS

7. **Refatorar ou refazer arquitetura**: para aplicações que você quer migrar para a AWS e aproveitar ao máximo os recursos nativos da nuvem para melhorar a agilidade, o desempenho e o dimensionamento

## Serviços e Recursos da AWS para Migração

Quais são alguns outros serviços e recursos da AWS disponíveis para apoiar sua jornada de migração para a nuvem?

### Exemplo Prático: Aplicação Financeira

Digamos que você esteja migrando sua aplicação que armazena informações financeiras na AWS. Sua aplicação requer acesso de baixa latência e os dados estão em constante mudança. Quais serviços da AWS você poderia usar para essa migração de aplicação? Amazon Elastic File System, AWS Snowball Edge, Amazon Simple Storage Service ou Amazon Relational Database Service?

Bem, o Amazon S3 é sempre uma boa escolha, mas, para o requisito de baixa latência, o Amazon S3 não é a melhor alternativa, pois fica na zona pública, está fora da Amazon VPC e poderia ter mais latência. O AWS Snowball Edge é usado para migração quando você precisa mover grandes quantidades de dados para dentro ou para fora da AWS.

**Minhas escolhas seriam Amazon EFS e Amazon RDS:**
- O **Amazon RDS** é um serviço de banco de dados gerenciado que fornece um banco de dados relacional dimensionável com desempenho rápido, alta disponibilidade e segurança
- O **Amazon EFS** fornece armazenamento de arquivos dimensionável com instâncias do Amazon EC2 e a capacidade de armazenamento também é elástica

### Exemplo: Banco de Dados NoSQL

E se você estiver migrando um banco de dados NoSQL e precisar garantir que o banco de dados seja dimensionável, rápido e confiável? Qual serviço de banco de dados da AWS você recomendaria? Amazon S3, Amazon RDS, Amazon Redshift ou Amazon DynamoDB?

O **Amazon DynamoDB** é um serviço de banco de dados NoSQL totalmente gerenciado que fornece desempenho rápido e previsível com dimensionamento. NoSQL e não relacional são palavras-chave para o DynamoDB, assim como relacional é uma palavra-chave para o Amazon RDS. O Amazon DynamoDB é um banco de dados de documentos e chave-valor e armazena documentos do tipo JSON. O AWS tem outro serviço de banco de dados totalmente gerenciado, o Amazon Aurora.

### Exemplo: Microsoft SQL Server

E se você precisar iniciar um banco de dados de servidor Microsoft SQL na AWS, mas precisar garantir que o banco de dados tenha custos otimizados e apenas uma licença-padrão para servidor SQL seja necessária?

**Opções disponíveis:**
- Você inicia um banco de dados Amazon Aurora que executa o SQL Server e compra uma licença-padrão de servidor do Microsoft SQL do serviço AWS License Manager?
- Ou você usa uma instância do RDS que executa o SQL Server com uma licença SQL-padrão?
- Ou executa uma instância do Amazon EC2, instala o SQL Server e adquire uma licença SQL-padrão da Microsoft?
- Ou você usa um Windows Server com AMI do SQL Server Standard para não precisar comprar ou gerenciar sua própria licença?

**Resposta:** A AWS oferece várias imagens de máquina da Amazon (AMIs) para instâncias do Amazon EC2. Se você iniciar uma instância do Amazon EC2 usando uma AMI do Windows, poderá escolher uma que vem com o SQL Server Standard e não precisará adquirir sua própria licença da Microsoft. 

Você poderia escolher a instância de banco de dados do Amazon RDS que executa o SQL Server Standard e comprar a licença, mas a questão era a otimização de custos e o Amazon RDS custa mais do que o Amazon EC2, já que o Amazon RDS é um serviço gerenciado. E o Amazon Aurora oferece suporte apenas para o MySQL e o PostgreSQL, não para o SQL Server.

## Backup de Dados e Armazenamento

Outra área de foco para esta declaração de tarefa são os backups de dados, porque você precisa de um plano para armazenar seus dados depois de migrados. Entenda as opções de armazenamento de custos para os serviços de armazenamento da AWS.

Por exemplo, as storage classes do Amazon S3 Glacier são projetadas para serem as de menor custo do Amazon S3, permitindo o arquivamento de grandes quantidades de dados a um custo muito baixo. Mas é necessário considerar as taxas e os tempos de recuperação.

---

Vamos começar com a quarta declaração de tarefa e falar sobre os aspectos econômicos da nuvem.