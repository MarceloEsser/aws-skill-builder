# Lição 2: Entender o modelo de responsabilidade compartilhada

## Introdução

Vamos começar com a primeira declaração de tarefa do Domínio 2, que é entender o modelo de responsabilidade compartilhada da AWS.

No Domínio 1, discutimos a AWS como computação em nuvem e também apresentamos a infraestrutura global da AWS. Nesta lição, daremos um passo adiante e discutiremos o Modelo de responsabilidade compartilhada da AWS.

## O que é o Modelo de Responsabilidade Compartilhada da AWS?

O Modelo de responsabilidade compartilhada da AWS é como a AWS fornece clareza sobre quais áreas de segurança dos sistemas pertencem à AWS e quais pertencem ao cliente.

A AWS fornece o Modelo de responsabilidade compartilhada para que você tenha clareza sobre:

- Quais elementos da infraestrutura a AWS gerencia
- Quais elementos os clientes são responsáveis pelo gerenciamento

### Conceito Fundamental

Em um nível muito alto:

- **AWS é responsável pela segurança DA nuvem**
- **Você é responsável pela segurança NA nuvem**

## Estrutura da Infraestrutura AWS

Se você observar o diagrama com a infraestrutura global da AWS na parte inferior, também verá diferentes níveis de serviço na parte superior dessa infraestrutura global.

### Níveis da Infraestrutura

**Infraestrutura Global:**

- Regiões
- Zonas de Disponibilidade  
- Locais de borda em todo o mundo

A AWS gerencia tudo isso: o hardware, a segurança e muito mais para a infraestrutura global. Vocês, como clientes da AWS, não têm controle sobre nada disso e não precisam se preocupar com essa infraestrutura.

**Níveis de Serviço:**

- Computação
- Armazenamento
- Redes
- Bancos de dados

A AWS é novamente responsável por gerenciá-los e pela segurança desses serviços e sistemas.

**Software de Gerenciamento:**

Existe outro nível que a AWS gerencia: o software que auxilia qualquer um dos níveis de serviço abaixo dele.

## Exemplo Prático: Amazon EC2

Por exemplo, se você optar por provisionar uma instância do Amazon EC2 no nível de computação da AWS:

### Responsabilidades da AWS

- Gerenciará a Região e a Zona de Disponibilidade em que sua instância do Amazon EC2 será executada
- Cuida do provisionamento e da segurança da computação, das redes e do armazenamento necessários para essa instância
- Cuida do software da instância, como a interface do usuário ou o hipervisor

### Responsabilidades do Cliente

Agora é aqui que entra a sua responsabilidade. Você é responsável pelo **sistema operacional e superior**:

- Criptografia de dados do lado do cliente
- Integridade
- Autenticação
- Criptografia do lado do servidor
- Proteção do tráfego de rede
- Criptografar seus dados
- Usar certificados SSL
- Sistema operacional
- Configurações de rede e firewall
- Aplicação
- Gerenciamento de identidade e acesso
- Dados de seus clientes e proteção deles
- Backups desses dados

## Responsabilidades por Tipo de Serviço

Ser um Cloud Practitioner significa que você deve estar apto a determinar quando é necessário proteger recursos na AWS e o quanto precisa se envolver na segurança, o que pode variar de um serviço para outro.

### Exemplo de Análise

**Pergunta:** Quem é responsável por proteger os data centers que hospedam serviços da AWS?

**Resposta:** A AWS e não o cliente.

Esse é o nível de esforço que você precisa estar apto a fazer com relação ao Modelo de responsabilidade compartilhada da AWS.

## Variação de Responsabilidades por Serviço

Você também deve conseguir descrever como a responsabilidade de um cliente muda dependendo do serviço que ele está usando.

### Exemplo Comparativo: Banco de Dados MySQL

#### Cenário 1: Amazon RDS

- Pergunta: Você é responsável por aplicar patches no mecanismo de banco de dados em uma instância de banco de dados Amazon RDS?
- Resposta: **Não, a AWS é responsável por esses patches de segurança**

#### Cenário 2: Amazon EC2

- Pergunta: E se você tiver o mesmo banco de dados em execução em uma instância do Amazon EC2? Quem seria responsável pela aplicação de patches?
- Resposta: **Você, o cliente, é responsável pela aplicação de patches no Amazon EC2**

### Conceito-Chave: Serviços Gerenciados vs Não Gerenciados

As tarefas pelas quais você é responsável com relação à segurança dependem de um serviço da AWS ser ou não **gerenciado**.

**Serviços Gerenciados (ex: Amazon RDS):**

- Você precisa realizar **menos tarefas** de segurança e gerenciamento em geral

**Serviços Não Gerenciados (ex: Amazon EC2):**

- Você tem **mais controle** sobre o serviço
- Você é **mais responsável** pela execução de tarefas de segurança e gerenciamento

## Lição Principal

> **O nível de responsabilidade que o cliente assume depende do serviço usado.**

## Preparação para o Exame

Para o exame, é importante saber pelo que o cliente é responsável em comparação com a AWS para serviços como:

- Amazon RDS
- Amazon EC2
- Amazon DynamoDB
- AWS Lambda

---

Vamos começar com a segunda declaração de tarefa e falar sobre segurança, governança e conformidade da nuvem.