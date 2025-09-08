# Definir os Benefícios da Nuvem AWS

Vamos começar com a declaração da primeira tarefa que é **definir os benefícios da nuvem AWS**.

Para essa declaração de tarefa, você deve conhecer o valor da AWS. Mas antes de você entender o valor da AWS, deve saber o que é a AWS.

## O que é a AWS?

Bem, a AWS diz que a **Amazon Web Services (AWS)** é a mais abrangente e amplamente adotada nuvem do mundo, oferecendo mais de 200 serviços completos diretamente de data centers em todo o mundo.

Milhões de clientes, inclusive startups em rápido crescimento, grandes empresas e importantes órgãos governamentais, estão usando a AWS para:
- Reduzir custos
- Elevar a agilidade
- Inovar mais rapidamente

Então, a AWS nos fornece uma maneira de aprimorar nossa infraestrutura enquanto nos tornamos mais ágeis e também diminuímos nossos custos.

## O que é Computação em Nuvem?

Mas você também precisa entender o que é a computação em nuvem. Se você perguntar por aí ou pesquisar no Google o que é computação em nuvem, encontrará várias respostas diferentes.

Porém, computação em nuvem significa basicamente que você precisa cumprir determinados critérios. Vamos detalha-lá e examinar rapidamente os **cinco critérios**.

### 1. Autoatendimento sob Demanda

O primeiro critério que precisamos atender para a AWS ser considerada computação em nuvem é que a AWS tem a oferecer um **autoatendimento sob demanda** que é a capacidade de provisionar recursos ou capacidades de computação como:
- Servidores
- Banco de dados
- Redes
- Armazenamento
- E mais

Sob demanda quando esse serviço é necessário. Além disso, a computação em nuvem precisa ser capaz de provisionar nossos recursos sem qualquer intervenção ou interação humana para fazê-la um autoatendimento sob demanda.

A AWS nos permite fazer isso do console, a linha de comando, e também usando as interfaces de programação de aplicação (APIs). Não precisamos solicitar nem pedir a ninguém. Com as permissões certas, você pode entrar e começar a criar.

### 2. Acesso Amplo à Rede

O segundo critério é que a computação em nuvem precisa ter conexão com uma rede para acessar e provisão recursos necessários.

A AWS nos dá a capacidade de criar usando:
- Console de Gerenciamento da AWS
- Linha de comando
- HTTP
- HTTPS
- VPN
- SSH
- E mais

### 3. Agrupamento de Recursos

O terceiro critério é que a computação em nuvem precisa de **agrupamento de recursos**. Bem, o que é agrupamento de recursos?

A AWS fornece recursos em pool para atender a vários clientes diferentes da AWS. A AWS tem milhares de servidores, banco de dados e mais que podemos provisionar sob demanda e criar em nosso próprio ambiente. E esses recursos em pool estão disponíveis para mim, para você e para outros também.

Mas outra parte desse terceiro critério que temos que atender é **não saber a localização exata** desses recursos em pool. Por exemplo, ao ativar uma instância do Amazon Elastic Compute, Amazon EC2, instância você pode selecionar a Região AWS. Porém, a AWS pode escolher qualquer data center nessa Região AWS. No entanto, você pode escolher a Zona de Disponibilidade se quiser.

Vamos falar mais sobre Regiões e Zonas de Disponibilidade em alguns minutos.

#### Economias de Escala

A AWS adquire vários recursos para seus clientes da AWS. Portanto, estamos falando de milhares para garantir que estejam utilizando economias de dimensionamento. Você vai saber mais sobre economias de dimensionamento na otimização de custos.

Por enquanto, as economias de dimensionamento permitem que a AWS, com maior dimensionamento de recursos, ofereça economias em escala aos seus clientes, o que significa que a AWS pode repassar as economias aos seus clientes, ao mesmo tempo que fornece aos clientes os recursos necessários para dimensionar e crescer.

### 4. Elasticidade

Isso nos leva ao nosso quarto critério que a computação em nuvem precisa, que é a **elasticidade**, da qual falaremos ao longo deste curso.

Mas a elasticidade é a capacidade de dimensionar com a demanda. Conforme sua demanda aumenta, você pode aumentar verticalmente os recursos da AWS; e, quando essa demanda diminuir, você pode redimensionar seus recursos.

### 5. Serviço Medido

E o quinto e último critério que a AWS deve atender para ser considerada computação em nuvem é que o uso de recursos nas contas da AWS pode ser **monitorado e cobrado**.

Portanto, com a AWS, não estamos mais pré-provisionando, alocando armazenamento, servidores, computação e assim por diante. Você não tem mais que estimar suas demandas, porque com a AWS não estamos apenas usando serviços que tem o uso monitorado e, em seguida, são cobrados, mas também dimensionamos esses recursos para atender à sua demanda, em vez de super ou subprovisioná-los.

E o maior benefício de otimização de custos é que **pagamos apenas pelo que usamos** com a AWS.

---

## Infraestrutura Global da AWS

Como a AWS fornece tal computação em nuvem incrível? Bem, a AWS oferece uma **infraestrutura global** que é uma coleção de agrupamentos menores de infraestruturas que é conectada por uma rede global de alta velocidade.

E essa infraestrutura global permite que você crie sistemas que são resilientes e altamente disponíveis. E nos aprofundaremos na infraestrutura global da AWS posteriormente no curso no Domínio 3.

Mas por hora, entenda:
- Regiões AWS
- Zonas de Disponibilidade
- Locais de borda

---

## Vantagens da Nuvem AWS

Vamos concluir esta lição e abordar as vantagens da alta disponibilidade, da elasticidade e da agilidade.

### Alta Disponibilidade vs Tolerância a Falhas

Alta disponibilidade e tolerância a falhas costumam ser confundidas. Vamos nos aprofundar um pouco mais em ambas, e também na recuperação de desastres.

#### Alta Disponibilidade

A **alta disponibilidade** é um modo de projetar sistemas para que eles continuem em execução e prestando serviço o máximo de tempo possível. É feita de modo que, se ocorrer falha de um componente do sistema, ele será substituído ou corrigido assim que possível. Isso maximiza o tempo do sistema on-line.

Mas a alta disponibilidade não significa que ela impeça as falhas. E alta disponibilidade também não significa que não haverá tempo de inatividade nem interrupções. A alta disponibilidade responde quando há uma falha a ser corrigida assim que possível, para possibilitar o retorno do sistema ao serviço.

**Exemplo de Alta Disponibilidade:**
Digamos que temos uma aplicação em execução em um único servidor dentro da AWS. E este servidor é usado pelos funcionários para trabalhar. Se o servidor cair, os funcionários não poderão trabalhar porque ele está inativo e passando por uma interrupção.

Se você projetar essa arquitetura para ser altamente disponível, poderá criar rapidamente um novo servidor para fazer failover ou executar dois servidores para essa aplicação. Um em modo ativo e outro em modo de espera. Assim, se um servidor ficar inativo, será possível fazer failover para o segundo para atender os funcionários.

Mas, nessa situação, os funcionários precisam iniciar a sessão outra vez, então pode haver um pouco de tempo de inatividade, o que não é um problema. Não é o que você deseja, mas, com alta disponibilidade, algum tempo de inatividade é esperado, dependendo do design.

O objetivo da alta disponibilidade é reduzir interrupções e permanecer operacional para ser rápido, com recuperação automática é melhor. Mas geralmente há um tempo de inatividade, mesmo que seja muito breve.

#### Tolerância a Falhas

Agora, vamos analisar a **tolerância a falhas**. Ela é semelhante à alta disponibilidade, mas tolerância a falhas é a capacidade de um sistema de continuar funcionando em caso de falha.

Por exemplo, vamos dizer que ocorre falha em um ou mais dos componentes do sistema, mas ele continua funcionando mesmo assim. Portanto, um design tolerante a falhas deve continuar em operação.

**Exemplo de Tolerância a Falhas:**
Vamos voltar ao cenário anterior. Neste caso, estamos projetando para tolerância a falhas. Então teríamos dois servidores ativos atendendo a uma aplicação. Se um servidor ficar inativo, o segundo já estará ativo e vai continuar atendendo aos funcionários. Então não há tempo de inatividade nessa situação.

Os designs tolerantes a falhas operam para minimizar as falhas, mas também para continuar a operar durante elas. E esses designs de sistema costumam ser mais caros do que os de alta disponibilidade.

#### Recuperação de Desastres

A **recuperação de desastres** é um pouco diferente da tolerância a falhas e da alta disponibilidade, porque a tolerância a falhas e da alta disponibilidade tratam de projetar sistemas para operar durante um desastre.

A recuperação de desastres envolve o que precisamos planejar e também o que precisamos fazer no caso de um desastre. E ter um plano de recuperação de desastres é crucial porque o pior momento para se recuperar de um desastre é no meio dele.

Essa recuperação de desastres precisa de planejamento prévio e também de etapas para concluir o processo de recuperação de desastres. Portanto, quando o desastre ocorrer, você já terá um plano para recuperar seus sistemas o mais rápido possível.

Ao longo deste curso, continuaremos a discutir alta disponibilidade, tolerância a falhas e recuperação de desastres e como diferentes serviços da AWS são ótimas opções para um, ambos ou todos.

---

## Elasticidade e Scaling

Vamos prosseguir e falar sobre **elasticidade**.

Mencionamos scaling antes nessa lição. **Scaling** é a capacidade de um sistema de dimensionar. Portanto, aumentando ou diminuindo a carga colocada sobre esse sistema. E os sistemas são dimensionados quando precisam ser aumentados ou diminuídos, dependendo da carga.

Portanto, quando um sistema dimensiona, estamos adicionando ou removendo recursos em e de um sistema.

Existem duas formas de dimensionamento: **vertical** e **horizontal**.

### Scaling Vertical

Um exemplo de **scaling vertical** é se você tiver um tamanho específico de uma instância do Amazon EC2 e esse tamanho da instância não conseguir acompanhar o aumento da demanda, a instância poderá começar a ficar muito lenta ou, na pior das hipóteses, travar o sistema.

O scaling vertical está redimensionando sua instância do Amazon EC2 para um tamanho maior. Se você estivesse usando uma T2.micro, poderia ser necessário redimensioná-la para uma T2.medium ou maior.

E ao redimensionar sua instância, você está adicionando mais CPUs e memória ao seu sistema para lidar com o aumento na demanda.

#### Problemas do Scaling Vertical:
- Em geral, há uma pequena interrupção, porque a instância, quando redimensionada, precisa ser reinicializada
- Ao combinar com a otimização de custos, ao dimensionar verticalmente para um tamanho de instância maior ou muito maior, você também verá um aumento no seu custo

E essa é uma área na qual você pode se aprofundar no pilar Otimização de custos do AWS Well-Architected Framework, que abordaremos na próxima lição, para garantir que estamos dimensionando certo suas instâncias no início.

#### Benefícios do Scaling Vertical:
- Normalmente, não são necessárias modificações na aplicação
- Ele funciona para todas as aplicações

### Scaling Horizontal

Agora vamos falar sobre **scaling horizontal**, porque ele foi projetado para corrigir alguns dos problemas que temos com o scaling vertical.

Com o scaling horizontal, ao invés de aumentar o tamanho da instância, você adiciona mais instâncias do mesmo tamanho para lidar com a carga. E em vez de ter uma cópia em execução da aplicação, agora você tem uma cópia para cada instância dimensionada e pode usar um balanceador de carga para ajudar a distribuir a carga entre todas as instâncias.

#### Considerações do Scaling Horizontal:

**Sessões:**
Mas também temos que considerar certas coisas com o scaling horizontal. Uma consideração é a sessão. Com sua aplicação, não é recomendado interromper as sessões do cliente.

Quando você tem uma só aplicação em execução em um único servidor, todas as sessões são armazenadas nesse servidor. Mas o que você acha que acontece com suas sessões quando dimensionamos para vários servidores com cópias da sua aplicação?

Às vezes, você troca de instâncias, porque o scaling horizontal é feito para equilibrar a carga. Portanto, o balanceador de carga envia solicitações para diferentes servidores que têm uma cópia da aplicação.

Use o recurso **sticky sessions** para não perder suas sessões ao trocar de servidores. Isso funciona tanto com redução quanto com aumento da quantidade.

**Otimização de Custos:**
Além disso, no que diz respeito à otimização de custos, o scaling horizontal é normalmente mais barato, porque você usa tamanhos de instâncias menores e mais baratos.

### O que é Elasticidade?

Vamos abordar **elasticidade**. O que é? É um tópico importante de se conhecer e entender para o exame.

**Elasticidade** é o uso da automação com scaling horizontal para combinar a capacidade e o fornecimento com a demanda.

Você notará que a demanda raramente é linear. Geralmente está aumentando e diminuindo. Usar a elasticidade permite que sua capacidade aumente e diminua e atenda a essa demanda em constante mudança.

A AWS fornece configurações de inicialização e auto scaling para aumentar a quantidade de seus sistemas para combinar essa capacidade com essa demanda, o que permite que seu ambiente seja expandido, adicionando recursos à medida que a demanda aumenta.

E então, quando essa demanda diminuir, poderemos reduzir a escala para um número menor de servidores ou até mesmo nenhum servidor, o que otimiza:
- A eficiência do desempenho
- A excelência operacional
- A otimização de custos

Que são pilares do AWS Well-Architected Framework.

---

## Dicas para o Exame

Aqui estão algumas **dicas para o exame**:

- **Scaling vertical** = um tamanho maior
- **Scaling horizontal** = adicionar instâncias do mesmo tamanho
- **Elasticidade** = usar a automação com o scaling horizontal para adequar nossa capacidade à nossa demanda

---

Vamos começar com a segunda declaração de tarefa e falar sobre os princípios de criação da AWS.