# NEXON-TESTE

Projeto de validação da infraestrutura Nexon Labs na Hostinger VPS.

## Objetivo

Validar o fluxo:

GitHub → Hostinger Docker Manager → Docker → Traefik → HTTPS → subdomínio

## Endereço planejado

https://teste.nexonlabs.com.br

## Implantação

No Hostinger Docker Manager, use **Compose from URL** e informe:

https://raw.githubusercontent.com/juniorsousa-oss/NEXON-TESTE/main/docker-compose.yml

Nome do projeto:

nexon-teste

## DNS

Crie um registro A:

- Nome: teste
- Valor: 179.236.238.126

O projeto usa a rede externa `traefik-proxy` do Traefik da Hostinger e solicita SSL via Let's Encrypt.
