# 🐧 Estudos de Linux para Segurança

Anotações e comandos essenciais para administração e segurança em ambientes Linux.

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
