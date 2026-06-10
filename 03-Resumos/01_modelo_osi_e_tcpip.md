# Resumo Teórico: Modelo OSI vs. TCP/IP

### 1. As 7 Camadas do Modelo OSI (De cima para baixo)
1. **Aplicação** - Interface com o usuário e programas (Ex: HTTP, DNS, FTP, SSH).
2. **Apresentação** - Criptografia, compressão e formatação dos dados (Ex: SSL, JPEG).
3. **Sessão** - Estabelece, gerencia e finaliza a comunicação entre as aplicações.
4. **Transporte** - Comunicação fim-a-fim, controle de fluxo e erro (Ex: TCP, UDP).
5. **Rede** - Endereçamento lógico (IP) e roteamento de pacotes (Ex: Roteadores).
6. **Enlace** - Endereçamento físico (MAC) e controle de acesso ao meio (Ex: Switches, Wi-Fi).
7. **Física** - Transmissão física de bits através de cabos ou ondas de rádio (Ex: Cabos UTP, Fibra).

### 2. O Modelo TCP/IP (Atualizado - 5 Camadas)
O modelo prático da Internet resume as camadas de software em apenas uma:
* **Aplicação** (Une as antigas camadas 5, 6 e 7 do OSI)
* **Transporte**
* **Rede** (Também chamada de Internet)
* **Enlace**
* **Física**

### 3. Encapsulamento de Dados (PDU)
Conforme os dados descem as camadas, eles ganham cabeçalhos específicos e mudam de nome:
* Camadas de Aplicação ➡️ **Dados**
* Camada de Transporte ➡️ **Segmento** (Adiciona portas de origem/destino)
* Camada de Rede ➡️ **Pacote** (Adiciona IPs de origem/destino)
* Camada de Enlace ➡️ **Quadro / Frame** (Adiciona MACs de origem/destino e o FCS no final)
* Camada Física ➡️ **Bits** (Sinais elétricos ou ópticos no cabo)
