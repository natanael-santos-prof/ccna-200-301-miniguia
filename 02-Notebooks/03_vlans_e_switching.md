# Guia de Switching e VLANs CCNA

### 1. Configuração de VLANs
* `vlan 10` - Cria a VLAN ID 10 no switch.
* `name Vendas` - Dá um nome identificador para a VLAN 10.

### 2. Associação de Portas (Acesso e Trunk)
* `interface f0/1` - Entra na configuração da porta FastEthernet 0/1.
* `switchport mode access` - Define a porta no modo de acesso (para conectar PCs).
* `switchport access vlan 10` - Coloca essa porta permanentemente dentro da VLAN 10.
* `interface f0/24` - Entra na configuração da porta de uplink.
* `switchport mode trunk` - Configura a porta como Tronco (para passar todas as VLANs para outro Switch ou Roteador).

### 3. Segurança de Porta (Port Security)
* `switchport port-security` - Ativa a segurança na interface de acesso.
* `switchport port-security maximum 1` - Permite apenas 1 dispositivo (MAC) conectado nesta porta.
* `switchport port-security mac-address sticky` - Memoriza automaticamente o endereço MAC do primeiro PC que plugar.
* `switchport port-security violation shutdown` - Desativa e bloqueia a porta automaticamente se um MAC desconhecido tentar se conectar.

### 4. Diagnóstico de Switching
* `show vlan brief` - Mostra todas as VLANs criadas e em quais portas elas estão associadas.
* `show interfaces trunk` - Exibe quais portas estão operando em modo Trunk.
* `show port-security interface f0/1` - Mostra os detalhes de segurança e violações da porta f0/1.
* `show mac address-table` - Mostra a tabela de endereços MAC que o switch aprendeu.
