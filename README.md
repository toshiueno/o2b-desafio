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

Após a criação do ambiente um arquivo de texto com o nome "elb_url_app.txt" será criado na raiz do projeto e conterá a URL do load balancer para acesso ao nginx.

O script deverá:

1. Criar um grupo de segurança para acesso
2. Criar um Load Balancer
3. Criar um novo par de chaves para o EC2
4. Criar uma nova instância EC2 com Centos 7.
5. Criar um novo disco de 5GB
6. Formatar o disco em XFS e montar como "/fileshare"
7. Desabilitar o IPV6
8. Desabilitar o serviço de auditd
9. Instalar o nginx
10. Desabilitar o SELinux
11. Habilitar o repositório "elrepo"
12. Habilitar e instalar o "kernel-ml"








