# Prompts para Treinamento de Sub-redes e VLSM

Estes comandos servem para fazer a IA gerar desafios matemáticos de cálculo de IP para você treinar a velocidade de resposta para a prova do CCNA.

### 1. Prompt para Simular Desafios de VLSM (Cenário Real)
> **Comando:** "Gere um desafio prático de VLSM (Variable Length Subnet Mask). Forneça uma rede principal (ex: 192.168.10.0/24) e peça para eu dividi-la atendendo a 3 departamentos com necessidades diferentes de hosts (ex: Vendas com 50 hosts, TI com 20 hosts e Diretoria com 5 hosts). Não dê a resposta, apenas o enunciado. Avalie meus cálculos quando eu responder."

### 2. Prompt para Treinar Velocidade de Cálculo de Bloco
> **Comando:** "Quero treinar minha velocidade para a prova do CCNA. Mande apenas um endereço IP com uma máscara em formato CIDR (ex: 172.16.45.122/22). Eu vou calcular e te mandar: a) O endereço de rede desse bloco, b) O primeiro IP válido, c) O último IP válido, d) O endereço de broadcast. Quando eu responder, corrija meu raciocínio."

### 3. Prompt para Identificar Erros de Endereçamento IP
> **Comando:** "Crie um cenário de configuração onde um administrador de redes tentou colocar um endereço IP em uma interface de roteador Cisco, mas o sistema retornou um erro de 'IP inválido' ou 'máscara sobreposta'. Me dê os comandos que o administrador digitou para que eu analise e descubra qual foi o erro de cálculo de sub-rede que ele cometeu."
