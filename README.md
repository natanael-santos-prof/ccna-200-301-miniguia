# 🎓 Projeto Final: Aprendizado Acelerado com NotebookLM aplicado ao CCNA

Este repositório é o projeto de conclusão do desafio proposto pelo programa **Bootcamp & Bradesco**. O objetivo principal é demonstrar como utilizar o **NotebookLM** de forma estratégica para acelerar o aprendizado técnico de infraestrutura de redes (Cisco CCNA 200-301) de maneira altamente eficaz.

## 📝 Resumo da Metodologia Utilizada no Bootcamp

O foco do projeto foi transformar materiais brutos e extensos de redes em uma base de conhecimento interativa e personalizada dentro do NotebookLM, aplicando múltiplos métodos de estudo ativo:

### 🧠 Métodos de Otimização de Estudo com o NotebookLM:
1. **Resumos Inteligentes:** Geração de resumos teóricos focados apenas nos pontos mais cobrados na prova (Modelos OSI, TCP/IP e Serviços de Rede).
2. **Guias de Áudio (Podcasts Acadêmicos):** Utilização da IA do NotebookLM para transformar apostilas densas em conversas de áudio dinâmicas em formato de podcast, facilitando a fixação do conteúdo no dia a dia.
3. **Mapas Mentais e Estruturação:** Organização visual de tópicos complexos, interligando conceitos de Roteamento, Switching e Automação em Python.
4. **Flashcards para Memorização Ativa:** Criação de cartões de pergunta e resposta rápidos para decorar timers de protocolos (OSPF), portas de serviços (DHCP/DNS) e Distâncias Administrativas.
5. **Estudo Multimodal (Vídeos, Imagens e Infográficos):** Integração de referências visuais e topologias de rede para facilitar a compreensão dos comandos práticos do Cisco IOS.

---

## 📁 Estrutura do Repositório (Organização do Estudo)

Para refletir essa metodologia de estudo com IA, o projeto foi estruturado nas seguintes pastas:
* **01-Fontes:** PDFs originais de estudo, apostilas e links que alimentaram a fonte do NotebookLM.
* **02-cadernos:** Guias práticos com scripts de comandos Cisco extraídos e organizados através da IA.
* **03-Resumos:** Fichamentos teóricos gerados e revisados a partir das interações com o NotebookLM.
* **04-prompts:** Engenharia de prompts detalhada com os comandos exatos usados para fazer a IA gerar os materiais certos.
* **05-extras:** Glossário inglês/português de termos técnicos e materiais complementares recomendados.

---

## 🛠️ Scripts Práticos de Automação Desenvolvidos

Além da metodologia de estudo, este repositório também guarda a aplicação prática do aprendizado de Python para redes:

### 📌 1. Consulta Automática de Interfaces (`consulta_roteador.py`)
Utiliza a biblioteca Netmiko para fazer um "raio-X" automático das portas de um roteador via SSH em menos de 2 segundos, eliminando o processo manual de troubleshooting.

### 📌 2. Varredor de Portas (`port_scanner.py`)
Script focado em segurança de infraestrutura para testar e identificar portas lógicas abertas ou vulneráveis na rede.

