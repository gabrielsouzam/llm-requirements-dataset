Aja como um Engenheiro de Requisitos Sênior experiente. Sua tarefa é analisar o contexto detalhado de um projeto de software e, a partir dos exemplos de requisitos fornecidos, gerar a especificação completa dos demais requisitos funcionais que faltam.

# CONTEXTO DO SISTEMA

O projeto é um Sistema de Gerenciamento para Restaurante Universitário. O objetivo é modernizar e otimizar a experiência alimentar dos alunos, permitindo o controle de demanda, redução de desperdício e maior eficiência no atendimento.

O sistema atende principalmente aos Alunos, que precisam planejar suas refeições (almoço/jantar), informar restrições alimentares e acompanhar o cardápio, e à Administração, que precisa gerenciar a demanda diária e os relatórios. O sistema visa substituir controles manuais por uma gestão digital de reservas, filas e feedback.

# EXEMPLOS DE REQUISITOS (30%)

Abaixo estão alguns exemplos de requisitos funcionais do sistema, derivados das especificações originais:

## RF001 - Registrar Alunos
O sistema deve permitir o cadastro de alunos, coletando informações pessoais obrigatórias como nome completo, número de matrícula e curso, além de credenciais de acesso.

## RF002 - Efetuar Login
O sistema deve permitir que os alunos realizem autenticação segura utilizando suas credenciais (nome de usuário e senha) para acessar funcionalidades personalizadas.

## RF003 - Indicar Refeição
O sistema deve permitir que os alunos indiquem se farão uma refeição (almoço ou jantar) em uma data específica, auxiliando na previsão de demanda diária.

## RF005 - Indicar Restrições Alimentares
O sistema deve permitir que os alunos registrem em seu perfil quaisquer restrições alimentares, como alergias, intolerâncias ou preferências dietéticas especiais.

## RF006 - Reservar Antecipadamente
O sistema deve permitir que os alunos realizem reservas de refeições para datas futuras específicas, garantindo a disponibilidade e agilizando o atendimento.

## RF007 - Acessar Cardápio
O sistema deve disponibilizar a visualização completa do cardápio para cada horário de refeição, detalhando as opções disponíveis.

## RF009 - Cancelar Reserva
O sistema deve permitir que os alunos cancelem suas reservas previamente realizadas, liberando a vaga e auxiliando na redução de desperdício.

## RF011 - Gerar Relatórios de Demanda
O sistema deve gerar relatórios administrativos (diários, semanais e mensais) detalhando a quantidade de refeições solicitadas.

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