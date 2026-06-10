# Guia de Segurança e ACLs CCNA

### 1. Configuração de Acesso Seguro (SSH)
* `ip domain-name empresa.com` - Define o nome de domínio obrigatório para o SSH.
* `crypto key generate rsa` - Gera as chaves de criptografia (escolha 1024 ou 2048 bits).
* `username admin secret senha123` - Cria um usuário local com senha criptografada.
* `line vty 0 4` - Entra nas linhas de acesso remoto.
* `transport input ssh` - Bloqueia o Telnet e permite apenas conexões via SSH.
* `login local` - Exige que o dispositivo use o usuário criado localmente para dar acesso.

### 2. ACLs Standard (Numéricas: 1 a 99)
* `access-list 10 permit 192.168.1.0 0.0.0.255` - Permite toda a rede 192.168.1.0 com máscara curinga.
* `access-list 10 deny any` - Bloqueia qualquer outro tráfego restante.
* `interface g0/0` - Entra na interface onde a regra será aplicada.
* `ip access-group 10 in` - Aplica a ACL 10 na entrada (in) da interface.

### 3. ACLs Extended (Numéricas: 100 a 199)
* `access-list 100 permit tcp 192.168.1.0 0.0.0.255 any eq 80` - Permite que a rede acesse qualquer servidor na web (porta HTTP 80).
* `access-list 100 deny ip any any` - Bloqueia qualquer outro tráfego de rede.
* `interface g0/1` - Entra na interface de saída.
* `ip access-group 100 out` - Aplica a ACL 100 na saída (out) da interface.

### 4. Diagnóstico de Segurança
* `show access-lists` - Mostra todas as ACLs configuradas e quantas vezes as regras foram acionadas (matches).
* `show ip interface g0/0` - Mostra, entre outras coisas, se há alguma ACL aplicada nesta interface.
* `show ssh` - Exibe o status e as conexões SSH ativas no momento no dispositivo.
