# RELATÓRIO DE IMPLEMENTAÇÃO DE MEDIDAS DE SEGURANÇA  :closed_lock_with_key: 🛡️

Data: 21/09/2023
Empresa: PharmaNova Labs
Responsável: Ana Clara R R M Becker

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa PharmaNova Labs, realizado por Ana Clara R R M Becker. O objetivo do projeto foi elencar 3 medidas de segurança em conjunto dos serviços da AWS, com a finalidade de realizar o aumento da segurança na empresa.



## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 medidas de segurança. A seguir, serão descritas as etapas da implementação:



#### Medida 1: 

<u>**Políticas de Controle de Acesso e IAM (Identity and Access Management)**</u>

- **Políticas de Controle de Acesso**: Definirão quais recursos da AWS os usuários e serviços têm permissão de acesso e quais ações podem ser feitas. Isso auxilia no controle de acesso de recursos, dando permissões para usuários ou serviços específicos. 

- Para facilitar, o IAM conta com a criação de usuários, grupos, políticas de acesso e roles.

  

- **Autenticação Multifatorial (MFA)**: Exige que os usuários autentiquem suas identidades por meio de uma autenticação de vários fatores, que adiciona uma camada adicional de segurança além de senhas e login (como exemplo, a solicitação de um código enviado por SMS ou e-mail cadastrados). Isso torna mais difícil os ataques às contas dos usuários.

- Os métodos MFA disponíveis são:

1. Chaves de segurança FIDO

   (disponibilizadas por terceirizadas)

2. Aplicações de autenticadores virtuais

   (Microsoft Authenticator, Google Authenticator, Symantec VIP, entre outros apps compatíveis com Android e iOS)

3. Tokens TOTP de hardware

   (tokens fornecidos pela Thales, fornecedor terceirizado)



- **Rotação de Credenciais**: Implemente a rotação regular de chaves de acesso e segredos, como senhas ou chaves de API, para reduzir o risco associado à exposição de credenciais.



#### Medida 2: 

<u>**Monitoramento e Registro de Atividades**</u>

- **Amazon CloudWatch**: Com ele podemos configurar alertas e monitorar o desempenho, a disponibilidade e a integridade dos recursos da AWS. Este serviço ajudará a identificar e responder a eventos de segurança em tempo real.
- **AWS CloudTrail**: Ao ativá-lo obteremos os registros de todas as ações realizadas nas contas da AWS. Ele fornecerá um registro detalhado de atividades que pode ser usado para auditoria de segurança e investigação de incidentes.
- **Amazon GuardDuty**: Utilizado para detectar ameaças de segurança automaticamente, como atividades suspeitas ou tentativas de invasão em diversas fontes de dados (Logs DNS, VPC, CloudTrail, S3, EBS, RDS). Ele utiliza Machine Learning para prever atividades inesperadas.



#### Medida 3: 

 <u>**AWS Key Management Service (KMS)**</u>

- **Gerenciamento de Chaves de Criptografia**: O AWS Key Management Service (KMS) é um serviço de controle de chaves utilizado para gerenciar e proteger as chaves de criptografia que protegerão os dados. O AWS KMS também é integrado ao AWS CloudTrail, que ajudará a verificação de quem usou quais chaves, em quais recursos e quando. 

- **Criptografia de Dados em Repouso**: A criptografia protegerá os dados em repouso em serviços como Amazon S3, Amazon RDS e Amazon EBS. Isso garantirá que, mesmo que os dispositivos de armazenamento sejam comprometidos, os dados permaneçam inacessíveis sem a chave de criptografia.
- **Criptografia de Dados em Trânsito**: Possibilidade de configurar a criptografia SSL/TLS para proteger os dados em trânsito entre os usuários e os serviços da AWS. Isso impedirá a interceptação de informações confidenciais durante a transferência.




## Conclusão
A implementação de ferramentas na empresa *PharmaNova Labs tem como esperado o fortalecimento da postura de segurança da empresa na AWS*, proporcionando uma defesa mais robusta contra ameaças cibernéticas e garantindo a proteção adequada dos recursos e dados críticos. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.



## Anexos

[https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html]

[https://aws.amazon.com/pt/iam/features/mfa/?audit=2019q1]

[https://aws.amazon.com/pt/cloudtrail/?nc2=type_a]

[https://aws.amazon.com/pt/guardduty/?nc2=type_a]

[https://aws.amazon.com/pt/cloudwatch/?nc2=type_a]

[https://aws.amazon.com/pt/kms/features/]

[Apresentação PPT](https://github.com/Ana-Becker/ImplantacaoSegurancaAWS/blob/main/ImplementacaoMedidasSeguranca.pdf)

Assinatura do Responsável pelo Projeto:

Ana Clara R R M Becker
