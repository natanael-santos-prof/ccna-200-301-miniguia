# Resumo Teórico: Serviços de Rede (DHCP, DNS e NAT)

### 1. DHCP (Dynamic Host Configuration Protocol) - UDP 67/68
O DHCP automatiza a distribuição de endereços IP, máscaras, gateways e servidores DNS para os dispositivos da rede. Ele funciona através do processo de 4 etapas conhecido como **DORA**:
1. **D**iscover (Descoberta): O cliente envia uma mensagem em broadcast procurando um servidor DHCP.
2. **O**ffer (Oferta): O servidor responde oferecendo um endereço IP disponível.
3. **R**equest (Requisição): O cliente aceita a oferta e pede o IP formalmente.
4. **A**cknowledge (Confirmação): O servidor confirma o aluguel do IP para o cliente.

### 2. DNS (Domain Name System) - UDP/TCP 53
O DNS funciona como a "lista telefônica" da Internet, traduzindo nomes de domínios amigáveis (como `://cisco.com`) em endereços IP que os computadores entendem. Os principais tipos de registros DNS cobrados no CCNA são:
* **Registro A:** Mapeia um nome de host para um endereço IPv4.
* **Registro AAAA:** Mapeia um nome de host para um endereço IPv6.
* **Registro CNAME:** Cria um apelido (alias) para um nome já existente.
* **Registro MX:** Aponta para os servidores de e-mail do domínio.

### 3. NAT (Network Address Translation)
O NAT traduz endereços IP privados (RFC 1918) em endereços IP públicos roteáveis para permitir o acesso à Internet, economizando IPs públicos globais. Ele se divide em três tipos:
* **NAT Estático:** Mapeamento fixo de 1 para 1 (um IP privado específico para um IP público específico). Muito usado em servidores internos.
* **NAT Dinâmico:** Mapeamento de vários para vários usando um grupo (pool) de IPs públicos disponíveis por ordem de chegada.
* **PAT (Port Address Translation / NAT Overload):** Mapeia milhares de IPs privados para um **único** IP público, diferenciando as conexões pelos números das portas TCP/UDP de origem. É o modelo usado nas residências e empresas.

### 4. Terminologia do NAT na Cisco
* **Inside Local:** O endereço IP real configurado na máquina dentro da rede local (Privado).
* **Inside Global:** O endereço IP público atribuído pelo provedor que representa a máquina na Internet.
* **Outside Local:** O endereço IP do destino visto a partir da rede interna.
* **Outside Global:** O endereço IP real configurado no dispositivo de destino na Internet.
