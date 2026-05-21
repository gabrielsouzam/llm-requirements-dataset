Aja como um Engenheiro de Requisitos Sênior experiente. Sua tarefa é analisar o contexto de um projeto de software e, a partir dos exemplos de requisitos fornecidos, gerar a especificação completa dos demais requisitos funcionais que faltam.

# CONTEXTO DO SISTEMA

O projeto é o "FakeNet-NG", uma ferramenta de análise de rede dinâmica para software malicioso. Seu principal objetivo é interceptar o tráfego de rede do malware, impedindo que ele chegue à Internet.

O sistema funciona "desviando" o tráfego da pilha de rede local para seus próprios servidores falsos, chamados "Listeners". Isso permite que um analista observe o comportamento do malware.

Os componentes principais são:
- Aplicação (Application): O ponto de entrada que lê a configuração e inicia os serviços.
- Diverter: O componente que manipula a pilha de rede para interceptar e redirecionar o tráfego.
- Listeners: Servidores que simulam serviços reais (DNS, HTTP, etc.) para "enganar" o malware.
- Proxy Listener: Um listener especial que pode identificar e rotear tráfego para o listener correto.

# EXEMPLOS DE REQUISITOS (30%)

Abaixo estão alguns exemplos de requisitos funcionais do sistema:

---
## Requisito de Aplicação: Término Graceful com Control-C
Quando o usuário pressiona Control-C (sinal SIGINT), a Aplicação deve:
1. Desligar as instalações dos Listeners.
2. Encerrar a filtragem e modificação de pacotes.
3. Reverter a configuração da rede local ao seu estado original.

---
## Requisito de Aplicação: Habilitação do Diverter
Deve existir uma configuração booleana (DivertTraffic) que controla se a Aplicação iniciará o Diverter. Se desabilitado, o FakeNet-NG não deve redirecionar nenhum tráfego, mas ainda deve iniciar os Listeners configurados.

---
## Requisito do Diverter: Captura de Pacotes (PCAP)
O Diverter deve respeitar a configuração booleana DumpPackets. Quando habilitada, ele deve escrever um arquivo .pcap contendo as formas inicial e final (se modificada) do tráfego.

---
## Requisito do Listener: Suporte ao "Taste"
Todos os Listeners devem implementar um callback taste() para permitir que o Proxy Listener identifique o Listener correto para encaminhar o tráfego, com base em uma amostra inicial dos dados.
---

# INSTRUÇÕES

Siga os seguintes passos (Árvore de Pensamentos - ToT) para derivar os requisitos funcionais faltantes:

Passo 1: Geração de Múltiplos Pensamentos (Exploração de Lacunas)
Analise o Contexto (Funções Principais) e os Exemplos fornecidos. Gere 3 "linhas de pensamento" (propostas) distintas que explorem as categorias de requisitos que ainda não foram cobertas pelos exemplos.

Proposta 1 (Agente Focado em Roteamento e Modos): Gere os cenários faltantes relacionados a como o tráfego é interceptado e em que escopo. Considere os diferentes NetworkMode (SingleHost vs. MultiHost), a modificação de DNS local (ModifyLocalDNS) e a regra principal de desvio (RedirectAllTraffic).

Proposta 2 (Agente Focado em Filtragem e Exceções): Gere os cenários faltantes relacionados ao controle do que é interceptado. Explore exaustivamente as funcionalidades de "Blacklist" e "Whitelist" (ex: BlackListPortsTCP, HostBlackList, ProcessBlackList).

Proposta 3 (Agente Focado em Simulação de Resposta): Gere os cenários faltantes relacionados a como os Listeners devem responder ao malware. Explore as capacidades de "Resposta Customizada" (Custom Response) para os listeners HTTP, TCP e UDP (ex: retornar um arquivo, uma string estática ou delegar a um script Python).

Passo 2: Autoavaliação dos Pensamentos (Avaliação e Refinamento)
Aja como um "Arquiteto Chefe" e avalie criticamente as 3 propostas. Analise quais propostas cobrem as funcionalidades mais críticas para um analista de malware. Determine se as propostas, em conjunto, cobrem todas as funcionalidades-chave restantes inferidas do contexto (como controle de automação e regras de filtragem).

Passo 3: Síntese e Resposta Final (Geração Consolidada)
Com base na sua autoavaliação, combine os melhores e mais relevantes elementos de todas as propostas. Produza a lista final e consolidada dos requisitos funcionais faltantes. A resposta final deve seguir exatamente o mesmo formato ("## Título do Requisito" e descrição em prosa ou tópicos) usado nos exemplos.

Apresente sua resposta de forma claramente separada por cada passo: Proposta 1, Proposta 2, Proposta 3, Avaliação e, por fim, a Versão Final Consolidada.