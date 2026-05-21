Aja como um Engenheiro de Requisitos Sênior experiente. Sua tarefa é analisar o contexto detalhado de um projeto de software e, a partir dos exemplos de requisitos fornecidos, gerar a especificação completa dos demais requisitos funcionais que faltam.

# CONTEXTO DO SISTEMA

O sistema é uma ferramenta de gestão para nutricionistas que centraliza todo o acompanhamento do paciente. O fluxo começa com a anamnese, onde são coletados dados sobre a rotina, trabalho, família e saúde (medicamentos e alergias). Em seguida, o sistema registra informações físicas (peso, altura, medidas e dobras cutâneas) para calcular gastos calóricos. Com esses dados, o profissional realiza a construção da dieta, definindo horários, locais de alimentação e o equilíbrio de macro e micronutrientes. Por fim, o software gerencia o retorno, permitindo que o nutricionista analise novos exames, colete feedbacks sobre as refeições e ajuste o plano alimentar conforme a evolução do paciente. 

# EXEMPLOS DE REQUISITOS

Abaixo estão alguns exemplos de requisitos funcionais do sistema, derivados das especificações originais:

RF001 - Registrar Anamnese e Perfil do Paciente

O sistema deve permitir o cadastro detalhado do perfil do paciente, incluindo: dados socioeconômicos (renda e trabalho), rotina diária (atividades físicas, horários de alimentação, tempo livre e presença de filhos), histórico de saúde (medicações em uso, exames laboratoriais prévios, intolerâncias e alergias) e hábitos alimentares atuais.


RF002 - Planejamento de Dieta Estruturada

O sistema deve permitir a construção de dietas personalizadas, permitindo a definição da quantidade de refeições, horários, local de consumo e a adequação precisa de proteínas, carboidratos, lipídios, além de macro e micronutrientes.


RF003 - Gestão de Ajustes e Manutenção

O sistema deve permitir que o nutricionista realize ajustes na dieta vigente com base no retorno do paciente, considerando os resultados de novos exames apresentados, a evolução das medidas físicas e o feedback subjetivo do usuário.

RF004 - Registro de Avaliação Antropométrica e Bioenergética

O sistema deve permitir o registro de medidas físicas, incluindo estatura, peso, circunferências (fita métrica) e dobras cutâneas (adipômetro), realizando automaticamente o cálculo do gasto calórico basal e o gasto calórico total baseado no nível de atividade física.


RF005 - Monitoramento de Evolução e Retorno

O sistema deve possibilitar o registro de consultas de acompanhamento para que sejam realizadas novas medições e a comparação com os exames laboratoriais atualizados trazidos pelo paciente, visando gerar um histórico de progresso.


RF006 - Gestão de Variabilidade Dietética e Feedback

O sistema deve permitir a inclusão de múltiplas opções de alimentos para cada refeição prescrita e oferecer um canal para que o paciente registre feedbacks específicos sobre a aceitabilidade e preferência de cada opção durante o retorno.

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