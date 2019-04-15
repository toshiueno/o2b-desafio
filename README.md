# Desafio O2B
Essa receita ansible foi desenvolvida em resposta ao desafio O2B e tem como objetivo criar um ambiente novo na AWS.

# Ambiente Utilizado

O ambiente descrito abaixo foi o utilizado no desafio e serve como parâmetro/ponto de partida para execução do playbook.

## Pré Requisitos do client

### Sistema Operacional
Linux Mint 19.1

### Ansible
Ansible 2.5.1

### Boto
boto3 (1.9.130)

## Cloud

### Amazon AWS

Os seguintes componentes foram utilizados/criados

EC2  
ELB  
Security Group  
KeyPair  
Volumes  

# Execução

Após a instalação dos pré-requisitos como o ansible e boto3, copiar a credential aws que foi enviada por email para o home do usuário que irá executar o playbook.

O diretório ficará com a seguinte estrutura:

~/.aws/config  
~/.aws/credentials  

Efetuar o clone deste repositório git e executar o comando a partir da raiz deste diretório:

$ ansible-playbook -i inventory o2b.yml

A execução desta receita criará os seguintes itens:




