# kali-linux-bruteforce-lab
1. Introdução

Objetivo:

O objetivo deste trabalho foi realizar testes de segurança em um ambiente controlado utilizando Kali Linux como máquina atacante e Metasploitable 2 como máquina vulnerável, simulando um cenário real de testes de penetração.

2. Ambiente do Laboratório

Exemplo:

Máquina	Sistema	IP
Kali Linux	Atacante	192.168.56.4
Metasploitable 2	Alvo	192.168.56.3

Rede utilizada:

Host-only Adapter

3. Reconhecimento

Ferramenta utilizada:

nmap -sV 192.168.56.3

Resultados principais:

Porta	Serviço
21	FTP
22	SSH
23	Telnet
80	HTTP
139	SMB
445	SMB
3306	MySQL

4. Ataques Realizados
Brute Force FTP

Ferramenta:

medusa

Resultado:

User: msfadmin
Password: msfadmin
Password Spraying SMB

Ataque testando a mesma senha contra múltiplos usuários.

Resultado:

ACCOUNT FOUND
Acesso Telnet

Login bem sucedido com:

msfadmin / msfadmin
Exploração Web

Aplicação vulnerável:

DVWA

Tipo de ataque:

SQL Injection

Payload utilizado:

1' OR '1'='1

Resultado: acesso aos dados da base.

5. Conclusão
   
Os testes demonstraram diversas vulnerabilidades no sistema Metasploitable 2, incluindo credenciais fracas, serviços expostos e aplicações web vulneráveis. Essas falhas poderiam permitir acesso não autorizado e comprometimento total do sistema em um ambiente real.
