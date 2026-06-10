# Resumo Teórico: Endereçamento IP e Sub-redes (Subnetting)

### 1. Estrutura do Endereço IPv4
Um endereço IPv4 possui 32 bits, divididos em 4 octetos (valores de 0 a 255). Ele é composto por duas partes:
* **Porção de Rede:** Identifica a qual rede o dispositivo pertence.
* **Porção de Host:** Identifica o dispositivo específico dentro daquela rede.
* **Máscara de Rede:** Define onde termina a rede e onde começam os hosts (Ex: `255.255.255.0` ou `/24`).

### 2. Classes de IP Padrão (Classful)
* **Classe A:** `1.0.0.0` a `127.255.255.255` (Máscara padrão: `/8`) -> Redes gigantescas.
* **Classe B:** `128.0.0.0` a `191.255.255.255` (Máscara padrão: `/16`) -> Redes médias.
* **Classe C:** `192.0.0.0` a `223.255.255.255` (Máscara padrão: `/24`) -> Redes pequenas.

### 3. IPs Privados vs. Públicos (RFC 1918)
Os IPs privados não são roteáveis na Internet e servem para economizar endereços nas redes locais:
* **Classe A Privado:** `10.0.0.0` a `10.255.255.255`
* **Classe B Privado:** `172.16.0.0` a `172.31.255.255`
* **Classe C Privado:** `192.168.0.0` a `192.168.255.255`

### 4. Endereços Especiais em uma Sub-rede
Toda sub-rede possui dois endereços que **nunca** podem ser atribuídos a computadores ou roteadores:
1. **Endereço de Rede:** O primeiro IP da sub-rede (identifica a rede).
2. **Endereço de Broadcast:** O último IP da sub-rede (usado para enviar pacotes para todos os hosts daquela rede ao mesmo tempo).

### 5. Fundamentos de IPv6
O IPv6 veio para substituir o IPv4. Ele possui 128 bits escritos em formato hexadecimal (8 grupos de 4 dígitos):
* **Exemplo:** `2001:0db8:85a3:0000:0000:8a2e:0370:7334`
* **Regra de Compressão:** É permitido omitir zeros à esquerda e substituir grupos consecutivos de zeros por dois-pontos duplos `::` (apenas uma vez por endereço). O exemplo acima reduz para: `2001:db8:85a3::8a2e:370:7334`.
