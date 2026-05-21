Aja como um Engenheiro de Requisitos Sênior experiente. Sua tarefa é analisar o contexto detalhado de um projeto de software e, a partir dos exemplos de requisitos fornecidos, gerar a especificação completa dos demais requisitos funcionais que faltam.

# CONTEXTO DO SISTEMA

O sistema em questão é é uma plataforma voltada para o credenciamento e gestão de eventos municipais focados em agricultores. O objetivo central é permitir o controle preciso do fluxo de participantes e a coleta de dados obrigatórios de interesse municipal. O software deve substituir processos manuais de assinatura por um fluxo digital que abrange desde a divulgação e pré-credenciamento até o registro no local do evento. Além disso, o sistema deve ser capaz de gerar relatórios estratégicos sobre o impacto econômico e social das capacitações e vendas realizadas durante os eventos

# EXEMPLOS DE REQUISITOS

Abaixo estão alguns exemplos de requisitos funcionais do sistema, derivados das especificações originais:

RF001 - Gestão de Eventos

O sistema deve permitir o cadastro completo de eventos, exigindo informações como nome, local, data, público-alvo, tipo de evento e se a entrada é aberta ao público geral.

RF002 - Cadastro de Espectadores e Produtores

O sistema deve permitir o registro de participantes (Pessoa Física ou Jurídica), coletando obrigatoriamente nome, telefone, CPF/CNPJ ou CAF/CICAB, e-mail e local de origem. Para garantir a conformidade legal, o sistema deve impedir o cadastro de menores de 18 anos.

RF003 - Fluxo de Credenciamento e Identificação

O sistema deve gerenciar a chegada do participante no local do evento, permitindo a busca por cadastros prévios ou novos registros; caso o usuário seja identificado como produtor rural, o sistema deve emitir um crachá de acesso específico.

RF004 - Relatórios de Impacto e Mobilização

O sistema deve processar os dados coletados para gerar relatórios detalhados sobre a quantidade de participantes, o volume financeiro mobilizado, o número de comerciantes ativos e o total de pessoas que participaram de capacitações.

RF005 - Formulários Adaptativos por Volume

Para otimizar o tempo de espera em eventos de grande escala, o sistema deve oferecer uma funcionalidade para adaptar e reduzir os campos do formulário, solicitando apenas os dados estritamente necessários para evitar a desistência do participante.

RF006 - Divulgação e Pré-Credenciamento Online

O sistema deve fornecer um módulo de divulgação antecipada que permita aos interessados realizarem o credenciamento prévio via internet, reduzindo as filas e o uso de assinaturas manuais no dia do evento

# INSTRUÇÕES

Para garantir uma análise completa e gerar os requisitos faltantes com alta qualidade, siga esta cadeia de pensamento (Chain-of-Thought) passo a passo:

Passo 1: Análise da Jornada do Usuário.
Primeiro, visualize a jornada completa do aluno no restaurante. Além de reservar e comer (já cobertos nos exemplos), o que mais ele precisa saber antes de comer (nutrição, fila)? O que ele faz durante ou após a refeição (check-in, feedback)?

Passo 2: Análise de Lacunas (Gap Analysis).
Em seguida, compare os Exemplos (30%) com a jornada mapeada no Passo 1. Identifique as categorias de funcionalidades que estão faltando:
 Informação Nutricional e Transparência: Faltam os requisitos sobre visualização de ingredientes, calorias, fornecedores e equipe.
 Operação e Fluxo: Faltam os requisitos de controle de fila, registro de presença (check-in) e histórico de consumo.
 Comunicação e Social: Faltam os requisitos de notificações (alertas de cardápio/reserva), feedback sobre a refeição, compartilhamento social e ranking de pratos.
 Manutenção: Falta a atualização de dados cadastrais.

Passo 3: Geração Final dos Requisitos Funcionais.
Finalmente, com base nas lacunas detalhadas no Passo 2, formule e apresente a lista final dos Requisitos Funcionais faltantes. Certifique-se de que cada requisito siga exatamente o mesmo formato de numeração (RFXXX) e o nível de detalhe descritivo usado nos exemplos.

Apresente cada passo da sua análise (Passo 1, Passo 2) antes de exibir a lista final de requisitos (Passo 3).