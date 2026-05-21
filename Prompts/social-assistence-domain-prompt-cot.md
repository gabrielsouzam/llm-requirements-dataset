Aja como um Engenheiro de Requisitos Sênior experiente. Sua tarefa é analisar o contexto de um projeto de software e, a partir dos exemplos de requisitos fornecidos, gerar a especificação completa dos demais requisitos funcionais que faltam.

# CONTEXTO DO SISTEMA

O projeto é o "Abrace" (Casa da Caridade), uma plataforma web de assistência social e filantrópica. O objetivo é auxiliar a "Casa da Caridade de Quixadá" a superar a dificuldade de divulgação e a dependência de métodos informais (como "boca a boca" e registros em papel).

A plataforma visa registrar e evidenciar todo o trabalho social realizado, aumentando a credibilidade da instituição e centralizando a divulgação de ações e o recebimento de doações. O sistema servirá a diferentes perfis: Visitantes (público geral), Usuários (cadastrados para receber novidades) e Administradores (a equipe da Casa da Caridade).

# EXEMPLOS DE REQUISITOS (30%)

Abaixo estão alguns exemplos de requisitos funcionais do sistema, com suas descrições detalhadas conforme o padrão do projeto:

## RF001 - Visualizar Ações de Caridade
O sistema deve permitir que o visitante (público) visualize uma lista de todas as ações de caridade da casa. Cada ação na lista deve ser apresentada de forma clara, incluindo:
 Título da ação
 Descrição breve
 Data e hora (se aplicável)
 Local (se aplicável)
 Fotos ou vídeos (opcional)
O visitante deve poder clicar em uma ação para ver uma página com todos os detalhes.

## RF004 - Realizar Doação via Pix
O sistema deve exibir um link ou botão "Doar via Pix". Ao clicar, o visitante deve ser direcionado para uma página que exibe o QR Code do Pix da Casa da Caridade. O QR Code deve ser válido para permitir que o visitante use seu aplicativo de banco para realizar a doação.

## RF005 - Cadastrar Novas Ações de Caridade
O sistema deve prover um painel administrativo acessível apenas por login seguro. Neste painel, o administrador (Casa da Caridade) deve ter a opção de criar uma nova ação de caridade através de um formulário que solicita:
 Título da ação
 Descrição detalhada
 Data e hora
 Local
 Objetivo da ação
 Fotos ou vídeos (opcional)
O sistema deve validar as informações antes de salvar e exibir a nova ação no site.

## RF009 - Acompanhar Doações Recebidas
O sistema deve prover, no painel administrativo, uma funcionalidade para visualizar e gerenciar as doações recebidas. O painel deve exibir uma lista de doações contendo:
 Nome do doador
 Valor da doação
 Data da doação
 Forma de pagamento (Pix, etc.)
 Status da doação (pendente, confirmada, etc.)
O administrador deve poder editar o status e registrar informações adicionais da doação.

## RF015 - Cadastrar-se como Usuário
O sistema deve prover um formulário de cadastro solicitando nome completo, endereço de e-mail e senha. O sistema deve verificar se o e-mail já está cadastrado. Após o envio, o sistema deve enviar um e-mail de confirmação contendo um link para o usuário clicar e concluir o cadastro.

# INSTRUÇÕES

Para garantir uma análise completa e gerar os demais requisitos funcionais (RFs) com alta qualidade, siga esta cadeia de pensamento (Chain-of-Thought) passo a passo:

Passo 1: Análise dos Perfis de Usuário.
Primeiro, analise os perfis de usuário do sistema (Visitante, Usuário Cadastrado, Administrador). Descreva brevemente o objetivo principal de cada perfil e as interações que eles precisam realizar.

Passo 2: Análise de Lacunas (Gap Analysis).
Em seguida, compare os Exemplos (30%) com os objetivos dos perfis do Passo 1. Identifique e liste quais categorias de requisitos funcionais não estão cobertas pelos exemplos. (Ex: "Para o 'Visitante', faltam as funções de 'Pesquisa' e 'Filtro'". "Para o 'Administrador', falta o ciclo completo de 'Gestão de Ações' (Editar, Excluir) e 'Gestão de Usuários'". "Para o 'Usuário Cadastrado', falta o 'Login' e 'Alteração de Perfil'").

Passo 3: Geração Final dos Requisitos Funcionais.
Finalmente, com base nas lacunas detalhadas no Passo 2, formule e apresente a lista final dos Requisitos Funcionais faltantes. Certifique-se de que cada requisito siga exatamente o mesmo formato de numeração (RFXXX) e o nível de detalhe descritivo usado nos exemplos.

Apresente cada passo da sua análise (Passo 1, Passo 2) antes de exibir a lista final de requisitos (Passo 3).