# CONTEXTO DO SISTEMA

O projeto é o "FakeNet-NG", uma ferramenta de análise de rede dinâmica para software malicioso. Seu principal objetivo é interceptar o tráfego de rede do malware, impedindo que ele chegue à Internet.

O sistema funciona "desviando" o tráfego da pilha de rede local para seus próprios servidores falsos, chamados "Listeners". Isso permite que um analista observe o comportamento do malware.

Os componentes principais são:
- **Aplicação (Application):** O ponto de entrada que lê a configuração e inicia os serviços.
- **Diverter:** O componente que manipula a pilha de rede para interceptar e redirecionar o tráfego.
- **Listeners:** Servidores que simulam serviços reais (DNS, HTTP, etc.) para "enganar" o malware.
- **Proxy Listener:** Um listener especial que pode identificar e rotear tráfego para o listener correto.

# EXEMPLOS DE REQUISITOS (30%)

Abaixo estão alguns exemplos de requisitos funcionais do sistema:

---
## Requisito de Aplicação: Término Graceful com Control-C
Quando o usuário pressiona Control-C (sinal SIGINT), a Aplicação deve:
1. Desligar as instâncias dos Listeners.
2. Encerrar a filtragem e modificação de pacotes.
3. Reverter a configuração da rede local ao seu estado original.

---
## Requisito de Aplicação: Habilitação do Diverter
Deve existir uma configuração booleana (`DivertTraffic`) que controla se a Aplicação iniciará o Diverter. Se desabilitado, o FakeNet-NG não deve redirecionar nenhum tráfego, mas ainda deve iniciar os Listeners configurados.

---
## Requisito do Diverter: Captura de Pacotes (PCAP)
O Diverter deve respeitar a configuração booleana `DumpPackets`. Quando habilitada, ele deve escrever um arquivo .pcap contendo as formas inicial e final (se modificada) do tráfego.

---
## Requisito do Listener: Suporte ao "Taste"
Todos os Listeners devem implementar um callback `taste()` para permitir que o Proxy Listener identifique o Listener correto para encaminhar o tráfego, com base em uma amostra inicial dos dados.
---

# INSTRUÇÕES

Com base no Contexto e seguindo o formato e o nível de detalhe dos Exemplos acima, gere a lista completa dos demais requisitos funcionais para este sistema.