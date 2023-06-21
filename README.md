# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 20/06/2023
Empresa: CompanyX 
Responsável: Vinicios M. Rodrigues

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa CompanyX, realizado por Vinicios M. Rodrigues. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

Etapa 1: 
- Amazon EC2 (Elastic Compute Cloud)
- O Amazon EC2 é um serviço de computação em nuvem que permite criar e gerenciar instâncias de servidores virtuais na nuvem. Ele fornece uma infraestrutura escalável e flexível, permitindo que você dimensione a capacidade de computação de acordo com as necessidades do seu aplicativo.
Aqui estão algumas das principais vantagens do EC2:
1. Escalabilidade: O EC2 permite que você dimensione a capacidade de computação de forma flexível de acordo com as necessidades do seu aplicativo.
2. Elasticidade: Elasticidade: Além da escalabilidade horizontal (aumento do número de instâncias), o EC2 também oferece a elasticidade vertical. Isso significa que você pode ajustar as especificações das instâncias, como CPU, memória e capacidade de armazenamento, para atender às necessidades específicas do seu aplicativo.
3. Diversidade de instâncias: O EC2 oferece uma ampla variedade de tipos de instâncias com diferentes configurações de recursos. Isso permite que você escolha a instância mais adequada para o seu caso de uso, levando em consideração fatores como CPU, memória, armazenamento, capacidade de rede e necessidades de desempenho.
4. Flexibilidade de configuração: Com o EC2, você tem controle total sobre o ambiente de computação. Você pode escolher o sistema operacional, instalar bibliotecas e aplicativos personalizados, configurar redes e segurança, e ajustar as configurações de desempenho de acordo com suas necessidades específicas.
5. Integração com outros serviços da AWS: O EC2 se integra perfeitamente a outros serviços da AWS, como o Amazon S3, Amazon RDS, Amazon VPC e Amazon CloudWatch, entre outros.
6. Segurança: A AWS possui uma ampla gama de recursos de segurança para proteger suas instâncias EC2. Isso inclui firewalls, grupos de segurança, controle de acesso baseado em função (IAM), criptografia de dados em repouso e em trânsito, e monitoramento de segurança.
- Um exemplo de caso de uso do Amazon EC2 (Elastic Compute Cloud) é o seguinte:
Suponha que você esteja desenvolvendo um aplicativo web que precise lidar com tráfego variável ao longo do dia. Durante os horários de pico, você pode ter centenas ou até milhares de usuários acessando o aplicativo simultaneamente, exigindo uma capacidade de computação escalável para atender à demanda. No entanto, durante os períodos de baixo tráfego, você não precisa manter todos esses recursos computacionais ativos, pois seria um desperdício de recursos e custos desnecessários.

Nesse cenário, você pode usar o Amazon EC2 para dimensionar automaticamente a capacidade de computação de acordo com o tráfego do aplicativo. Você pode configurar um grupo de instâncias EC2 em um Auto Scaling Group (Grupo de Dimensionamento Automático), que monitora a demanda e adiciona ou remove instâncias conforme necessário.

Durante os horários de pico, o Auto Scaling Group aumenta o número de instâncias EC2 disponíveis para lidar com o aumento do tráfego. Por exemplo, se a demanda ultrapassar um determinado limite, o grupo pode adicionar automaticamente mais instâncias para lidar com a carga extra. À medida que a demanda diminui, o grupo pode reduzir o número de instâncias em funcionamento para economizar custos.

Ao utilizar o Amazon EC2, você pode aproveitar a escalabilidade sob demanda para garantir que seu aplicativo possa lidar com tráfego variável, garantindo uma boa experiência do usuário durante os períodos de pico e evitando custos excessivos durante os períodos de baixo tráfego. Além disso, você tem controle total sobre a configuração das instâncias EC2, permitindo personalizar o ambiente de computação de acordo com as necessidades específicas do seu aplicativo, como escolher o tipo de instância, o sistema operacional e as configurações de segurança.

Etapa 2: 
- Amazon S3 (Simple Storage Service)
- O Amazon S3 é um serviço de armazenamento de objetos altamente escalável e durável. Ele permite que você armazene e recupere quantidades maciças de dados de forma segura pela Internet. O Amazon S3 é frequentemente usado para armazenar e fazer backup de arquivos, hospedar sites estáticos, distribuir conteúdo e alimentar aplicativos com dados armazenados na nuvem. Ele fornece recursos avançados, como criptografia, controle de acesso granular e integração com outros serviços da AWS.
- Imagine que você esteja desenvolvendo um aplicativo ou site que precise armazenar e exibir uma grande quantidade de imagens e vídeos. Usar o Amazon S3 para esse caso de uso tem várias vantagens:
Escalabilidade: O Amazon S3 é altamente escalável e pode lidar com grandes volumes de dados. Você pode armazenar quantidades maciças de arquivos e ter a certeza de que eles estarão disponíveis para recuperação imediata, independentemente do tamanho do seu acervo.

1. Durabilidade e disponibilidade: O Amazon S3 é projetado para oferecer durabilidade e disponibilidade de dados. Ele armazena redundante e automaticamente suas informações em várias zonas de disponibilidade dentro de uma região da AWS. Isso garante que seus arquivos estejam protegidos contra falhas de hardware e sejam acessíveis a qualquer momento.

2. Acesso rápido e baixa latência: O Amazon S3 é otimizado para oferecer acesso rápido aos arquivos armazenados. Ele é integrado à rede de entrega de conteúdo (CDN) da Amazon, chamada Amazon CloudFront, que permite entregar seus arquivos aos usuários finais de forma rápida e eficiente, independentemente da localização geográfica deles. Isso ajuda a reduzir a latência e melhorar a experiência do usuário.

3. Gerenciamento e controle de acesso: O Amazon S3 oferece recursos de gerenciamento e controle de acesso granulares. Você pode definir políticas de acesso para controlar quem pode ler, gravar ou excluir os arquivos armazenados no S3. Isso garante que seus dados estejam protegidos e só sejam acessados por pessoas autorizadas.

4. Integração com outros serviços da AWS: O Amazon S3 se integra facilmente com outros serviços da AWS, permitindo criar fluxos de trabalho automatizados e aplicar lógica de negócios ao seu armazenamento de objetos. Por exemplo, você pode usar o Amazon Lambda para executar ações personalizadas em seus arquivos, como redimensionar imagens, extrair metadados ou acionar processos adicionais.

5. Opções de armazenamento e classes de armazenamento: O Amazon S3 oferece diferentes opções de armazenamento para atender a diferentes necessidades de desempenho e custo. Por exemplo, você pode usar a classe de armazenamento "Standard" para acesso imediato e frequente aos seus arquivos, ou escolher a classe "Glacier" para arquivamento de longo prazo a um custo mais baixo.

Em resumo, o Amazon S3 oferece durabilidade, disponibilidade, baixa latência e controle de acesso, tornando-o adequado para uma ampla gama de aplicativos, desde sites e aplicativos móveis até serviços de backup e armazenamento em nuvem.

Etapa 3: 
- AWS Lambda
- O AWS Lambda é um serviço de computação sem servidor que permite executar código sem precisar provisionar ou gerenciar servidores. Com o AWS Lambda, você pode criar funções que respondem a eventos, como acionadores de API, eventos de upload de arquivos no Amazon S3 ou atualizações de tabelas no Amazon DynamoDB. Quando um evento ocorre, o código da função é executado automaticamente, dimensionando dinamicamente a capacidade de acordo com a demanda. O AWS Lambda é altamente flexível e pode ser usado para criar uma variedade de aplicativos e recursos, desde pequenos scripts até aplicativos de grande escala e em tempo real.
- Um caso de uso comum para o AWS Lambda é o processamento de eventos e execução de código em resposta a ações específicas, proporcionando uma arquitetura serverless. Aqui está um exemplo de caso de uso para o AWS Lambda:

Imagine que você esteja desenvolvendo um aplicativo web que permite que os usuários façam upload de imagens e, em seguida, aplique filtros às imagens antes de salvá-las. Você pode usar o AWS Lambda da seguinte maneira:

1. Upload de imagem: Quando um usuário faz o upload de uma imagem para o seu aplicativo, você pode usar o Amazon S3 para armazenar a imagem em um bucket. Em seguida, você pode configurar um gatilho no bucket do Amazon S3 para acionar um AWS Lambda sempre que uma nova imagem for adicionada.

2. Processamento assíncrono: O AWS Lambda permite que você escreva uma função que seja executada automaticamente sempre que o gatilho do Amazon S3 for acionado. Essa função pode ser escrita em várias linguagens de programação, como Python, Node.js, Java, entre outras. Dentro dessa função, você pode escrever o código necessário para processar a imagem e aplicar os filtros desejados.

3. Manipulação de imagens: Ao receber a notificação do evento de upload, a função do AWS Lambda é acionada e recebe a informação sobre a imagem. Você pode usar bibliotecas de processamento de imagens, como o Pillow em Python ou o Sharp em Node.js, para aplicar os filtros desejados à imagem. Por exemplo, você pode redimensionar a imagem, aplicar efeitos ou ajustar o contraste e a saturação.

4. Salvamento da imagem processada: Depois de aplicar os filtros à imagem, você pode salvar a imagem processada em outro bucket do Amazon S3 ou em algum outro serviço de armazenamento, como o Amazon DynamoDB ou o Amazon RDS, dependendo das necessidades do seu aplicativo.

O uso do AWS Lambda nesse caso de uso permite que você aproveite os benefícios da arquitetura serverless, onde não há necessidade de provisionar ou gerenciar servidores. O AWS Lambda cuida automaticamente da escala e da execução do código em resposta aos eventos, permitindo que você se concentre no desenvolvimento do aplicativo em si.

Essa é apenas uma das várias possibilidades de uso do AWS Lambda. Ele pode ser aplicado em diversos cenários, como processamento de eventos em tempo real, processamento de fila de mensagens, execução de tarefas agendadas, entre outros. Sua flexibilidade e escalabilidade o tornam uma escolha popular para criar aplicativos serverless na AWS.



## Conclusão
A implementação de ferramentas na empresa *CompanyX*, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

É importante ressaltar que a AWS oferece muitas outras ferramentas e serviços, como o Amazon RDS (serviço de banco de dados relacional), o Amazon DynamoDB (banco de dados NoSQL), o Amazon SQS (fila de mensagens) e o Amazon CloudFront (rede de entrega de conteúdo), entre outros.

## Anexos

- Vantagens da AWS: https://aws.amazon.com/pt/what-is-aws/#aws-benefits

- Estudos de caso da AWS: https://aws.amazon.com/pt/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.sortDate&customer-references-cards.sort-order=desc&awsf.language=language%23english&awsf.content-type=*all&awsf.customer-references-location=*all&awsf.customer-references-segment=*all&awsf.customer-references-industry=*all&awsf.customer-references-use-case=*all&awsf.customer-references-tech-category=*all&awsf.customer-references-product=*all

- Comparação de preços da AWS: https://aws.amazon.com/pt/pricing/?aws-products-pricing.sort-by=item.additionalFields.productNameLowercase&aws-products-pricing.sort-order=asc&awsf.Free%20Tier%20Type=*all&awsf.tech-category=*all

- Benefícios do Amazon EC2: https://aws.amazon.com/pt/ec2/benefits/

- Benefícios do Amazon S3: https://aws.amazon.com/pt/s3/features/

- Benefícios do AWS Lambda: https://aws.amazon.com/pt/lambda/features/

Assinatura do Responsável pelo Projeto: Vinicios M. Rodrigues

