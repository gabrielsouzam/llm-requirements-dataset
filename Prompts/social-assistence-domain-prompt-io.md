# CONTEXTO DO SISTEMA

O projeto é o "Abrace" (Casa da Caridade), uma plataforma web de assistência social e filantrópica. O objetivo é auxiliar a "Casa da Caridade de Quixadá" a superar a dificuldade de divulgação  e a dependência de métodos informais (como "boca a boca" e registros em papel).

A plataforma visa registrar e evidenciar todo o trabalho social realizado, aumentando a credibilidade da instituição  e centralizando a divulgação de ações e o recebimento de doações. O sistema servirá a diferentes perfis: Visitantes (público geral), Usuários (cadastrados para receber novidades) e Administradores (a equipe da Casa da Caridade).

# EXEMPLOS DE REQUISITOS (30%)

Abaixo estão alguns exemplos de requisitos funcionais e não-funcionais do sistema, com suas descrições detalhadas conforme o padrão do projeto:

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
O sistema deve prover um painel administrativo acessível apenas por login seguro. Neste painel, o administrador (Casa da Caridade) deve ter a opção de criar uma nova ação de caridade  através de um formulário que solicita:
 Título da ação 
 Descrição detalhada 
 Data e hora 
 Local 
 Objetivo da ação 
 Fotos ou vídeos (opcional) 
O sistema deve validar as informações  antes de salvar e exibir a nova ação no site

## RF009 - Acompanhar Doações Recebidas
O sistema deve prover, no painel administrativo, uma funcionalidade para visualizar e gerenciar as doações recebidas 332. O painel deve exibir uma lista de doações  contendo:
 Nome do doador 
 Valor da doação 
 Data da doação 
 Forma de pagamento (Pix, etc.) 
 Status da doação (pendente, confirmada, etc.) 
O administrador deve poder editar o status e registrar informações adicionais da doação.

## RF015 - Cadastrar-se como Usuário
O sistema deve prover um formulário de cadastro  solicitando nome completo, endereço de e-mail e senha. O sistema deve verificar se o e-mail já está cadastrado. Após o envio, o sistema deve enviar um e-mail de confirmação contendo um link para o usuário clicar e concluir o cadastro.

## RNF02 - Segurança de Doações
O sistema deve garantir que a aba de doações, especialmente o QR Code e as informações do Pix, não possa ser alterada ou ser vítima de fraude ou adulteração de informações por terceiros.

# INSTRUÇÕES

Com base no Contexto do sistema e nos requisitos fornecidos, gere os demais requisitos faltantes do sistema.