# 🐧 Estudos de Linux para Segurança

Anotações e conceitos essenciais de Linux para Segurança da Informação e Nuvem (AWS).

---

## 📖 Módulo: Introdução ao Sistema Operacional Linux

### 1. O que é um Sistema Operacional?
* **Definição:** É o software base que gerencia os recursos de hardware (CPU, memória, disco) e serve de plataforma para execução de programas e serviços.
* **Analogia:** Funciona como o maestro de uma orquestra: coordena os músicos (hardware) para que os instrumentos toquem em harmonia sem conflitos.

### 2. O que é o Linux?
* **Conceito:** Criado por Linus Torvalds em 1991, tecnicamente o Linux é o **kernel** (o coração) do sistema operacional. Ele é *open source* (código aberto).
* **Distribuições (Distros):** Conjunto do kernel Linux + utilitários e softwares.
  * **Ubuntu / Debian:** Uso geral e servidores web estáveis.
  * **Kali Linux:** Especializado em segurança ofensiva e testes de invasão (*pentest*).
  * **Amazon Linux:** Otimizado pela AWS para alta performance na nuvem.

### 3. Linux Desktop vs. Linux Server
* **Linux Desktop:** Focado em estações de trabalho e usuários finais, possui interface gráfica completa (GUI - janelas, ícones, mouse).
* **Linux Server:** Otimizado para servidores e nuvem, **opera sem interface gráfica (apenas CLI / terminal)**.
* **Vantagens do Server para Segurança e Nuvem:**
  * Menor consumo de hardware (mais leve e rápido).
  * Maior estabilidade e disponibilidade (*uptime*).
  * **Menor superfície de ataque:** sem componentes visuais ou serviços desnecessários abertos, reduzindo vulnerabilidades que invasores poderiam explorar.

---

## 📌 Comandos de Navegação e Sistema
- `pwd`: Exibe o diretório atual.
- `ls -la`: Lista todos os arquivos (incluindo ocultos) com detalhes de permissões e proprietários.
- `uname -a`: Mostra informações completas do kernel e sistema.

---

## 🔒 Gerenciamento de Permissões
No Linux, as permissões são divididas em **Usuário (u)**, **Grupo (g)** e **Outros (o)**:
- `r` (leitura = 4)
- `w` (escrita = 2)
- `x` (execução = 1)

### Exemplos práticos:
- `chmod 700 script.sh`: Permissão total apenas para o dono; ninguém mais acessa.
- `chmod 644 config.conf`: Leitura/escrita para o dono, apenas leitura para os demais.
- `chown usuario:grupo arquivo`: Altera o dono e o grupo do arquivo.

---

## 🔑 Acesso Remoto Seguro (SSH)
- `ssh usuario@ip_do_servidor`: Conecta remotamente via terminal seguro (porta padrão: 22).
