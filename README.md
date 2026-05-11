# Gerenciamento de Instâncias EC2 na AWS

## Descrição

Este repositório foi desenvolvido como parte do desafio prático da DIO com foco no gerenciamento de instâncias EC2 na AWS.

O objetivo deste laboratório foi aplicar conceitos de computação em nuvem na prática, além de documentar todo o processo utilizando o GitHub como ferramenta de compartilhamento técnico.

---

# Objetivos do Laboratório

- Aprender a criar e configurar instâncias EC2
- Entender o funcionamento do Amazon EC2
- Configurar grupos de segurança (Security Groups)
- Realizar acesso remoto via SSH
- Gerenciar inicialização e encerramento de instâncias
- Desenvolver documentação técnica utilizando Markdown

---

# O que é Amazon EC2?

O Amazon EC2 (Elastic Compute Cloud) é um serviço da AWS que permite criar servidores virtuais na nuvem.

Com ele, é possível hospedar aplicações, APIs, bancos de dados e diversos outros serviços de forma escalável e segura.

---

# Etapas Realizadas

## 1. Criação da Instância EC2

Durante esta etapa foram realizadas as seguintes configurações:

- Acesso ao painel da AWS
- Seleção do serviço EC2
- Escolha da imagem Amazon Linux
- Escolha do tipo de instância `t2.micro`
- Configuração de chave SSH
- Criação da instância

---

## 2. Configuração do Security Group

Foram liberadas as seguintes portas:

| Porta | Protocolo | Finalidade |
|------|------|------|
| 22 | SSH | Acesso remoto |
| 80 | HTTP | Acesso web |

---

## 3. Inicialização da Instância

Após a configuração da instância:

- A máquina virtual foi iniciada
- O status da instância foi verificado
- O IP público foi utilizado para conexão remota

---

## 4. Conexão via SSH

Comando utilizado para acesso remoto:

```bash
ssh -i chave.pem ec2-user@IP-DA-INSTANCIA

## Aprendizados

Durante o desenvolvimento deste laboratório, foi possível aprender:

Como criar servidores virtuais na AWS
Funcionamento básico do Amazon EC2
Diferença entre IP público e privado
Importância dos grupos de segurança
Configuração de acesso SSH
Organização de documentação técnica no GitHub
Dificuldades Encontradas

## Algumas dificuldades encontradas durante o laboratório:

Configuração correta do Security Group
Entendimento das permissões da chave .pem
Conexão SSH inicial com a instância

Esses desafios ajudaram no aprendizado prático da plataforma AWS.
