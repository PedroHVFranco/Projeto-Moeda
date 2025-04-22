# Projeto Moeda

Historias de Usuario

1.1 Aluno
HU01 - Resgatar Vantagem

Descrição:
Como Aluno, quero resgatar uma vantagem usando minhas moedas acumuladas, para obter benefícios de empresas parceiras.

Fluxo Principal:

O Aluno acessa o sistema e realiza o login.

O sistema exibe a lista de vantagens disponíveis (com descrição, custo em moedas e foto).

O Aluno seleciona uma vantagem e confirma o resgate.

O sistema desconta o valor em moedas do saldo do aluno, gera um código de cupom único e envia notificações por e-mail (ao aluno e à empresa parceira).

Fluxo Alternativo:

Se o saldo do Aluno for insuficiente, o sistema exibe uma mensagem de erro e bloqueia o resgate.

1.2 Professor
HU02 - Transferir Moedas

Descrição:
Como Professor, quero transferir moedas para alunos com justificativa, para reconhecer seu mérito acadêmico.

Fluxo Principal:

O Professor acessa o sistema e realiza o login.

O sistema exibe o saldo atual do professor e uma lista de alunos vinculados à sua instituição.

O Professor seleciona um aluno, insere a quantidade de moedas e uma mensagem de motivo.

O sistema valida o saldo do professor, atualiza os saldos (professor e aluno) e registra a transação com data/hora.

Fluxo Alternativo:

Se o saldo do Professor for insuficiente, o sistema cancela a operação e exibe um alerta.

1.3 Empresa Parceira
HU03 - Cadastrar Vantagem

Descrição:
Como Empresa Parceira, quero cadastrar novas vantagens no sistema, para atrair alunos a resgatarem meus benefícios.

Fluxo Principal:

A Empresa Parceira acessa o sistema e realiza o login.

O sistema exibe a interface de cadastro de vantagens.

A Empresa Parceira preenche nome, descrição, custo em moedas e URL da foto da vantagem.

O sistema valida os dados e adiciona a vantagem à lista disponível para resgate.

Fluxo Alternativo:

Se campos obrigatórios estiverem em branco, o sistema destaca os erros e solicita correção.

1.4 Secretaria
HU04 - Gerenciar Instituições

Descrição:
Como Funcionário da Secretaria, quero cadastrar ou atualizar instituições de ensino, para garantir que alunos e professores sejam vinculados corretamente.

Fluxo Principal:

O Funcionário da Secretaria acessa o sistema e realiza o login.

O sistema exibe a lista de instituições cadastradas.

O Funcionário da Secretaria adiciona uma nova instituição (nome, endereço) ou edita uma existente.

O sistema salva as alterações e atualiza a lista de instituições disponíveis para seleção.

Fluxo Alternativo:

Se o ID da instituição já existir, o sistema bloqueia o cadastro e solicita revisão.

1.5 Sistema
HU05 - Recarga Semestral Automática

Descrição:
Como Sistema, quero adicionar 1.000 moedas ao saldo de todos os professores no início do semestre, para garantir que eles possam distribuir reconhecimentos.

Fluxo Principal:

No primeiro dia do semestre, o sistema identifica todos os professores cadastrados.

O sistema adiciona 1.000 moedas ao saldo atual de cada professor (acumulando com saldos não usados).

O sistema registra a transação como "Recarga Semestral" no histórico de cada professor.

Fluxo Alternativo:

Se não houver professores cadastrados, o sistema ignora a operação.

