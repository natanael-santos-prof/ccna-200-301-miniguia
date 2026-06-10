# Guia de Roteamento CCNA

### 1. Roteamento Estático e Padrão
* `ip route 0.0.0.0 0.0.0.0 192.168.1.254` - Configura uma rota padrão (Gateway).
* `ip route 10.0.0.0 255.0.0.0 192.168.1.2` - Configura uma rota estática para a rede 10.0.0.0.

### 2. Protocolo OSPF (Roteamento Dinâmico)
* `router ospf 10` - Ativa o processo OSPF com ID 10.
* `router-id 1.1.1.1` - Define manualmente a identidade do roteador no OSPF.
* `network 192.168.1.0 0.0.0.255 area 0` - Ativa o OSPF na rede usando máscara curinga (wildcard) na Área 0.
* `passive-interface g0/0` - Impede o envio de atualizações de rotas para redes com computadores.

### 3. Comandos de Diagnóstico de Rotas
* `show ip route` - Exibe a tabela completa de rotas do roteador.
* `show ip ospf neighbor` - Mostra todos os roteadores vizinhos conectados via OSPF.
* `show ip ospf interface` - Mostra detalhes técnicos do OSPF nas interfaces.
* `ping 192.168.1.1` - Testa a conectividade direta com outro IP.
* `traceroute 8.8.8.8` - Mostra todo o caminho e saltos até o destino.
