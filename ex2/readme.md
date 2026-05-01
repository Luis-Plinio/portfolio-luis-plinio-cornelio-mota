📝 Descrição do Projeto
Este projeto automatiza o protocolo de triagem hospitalar, coletando sinais vitais e dados do paciente para determinar a prioridade de atendimento. O algoritmo garante a integridade dos dados antes do processamento e utiliza uma lógica de decisão em cascata para classificar a gravidade de cada caso.

⚙️ Fluxo de Operação do Algoritmo
Entrada de Dados e Coleta de Sinais Vitais:
O sistema inicia solicitando quatro variáveis fundamentais: a descrição dos sintomas, a frequência cardíaca, a temperatura corporal e a idade do paciente.

Validação e Ciclo de Segurança:
Antes de avançar, o algoritmo realiza uma verificação de consistência. Se os dados estiverem incorretos ou incompletos, o sistema retorna à etapa inicial (loop), garantindo que apenas informações válidas sejam processadas.

Análise de Risco Crítico:
Com os dados validados, o sistema calcula o nível de risco. Caso o cálculo aponte um risco alto, o fluxo é encerrado imediatamente com a atribuição de Prioridade Vermelha, destinada a casos de emergência.

Avaliação de Sintomas Graves:
Se o risco inicial não for alto, o algoritmo verifica a presença de sintomas graves. Confirmada a gravidade, o paciente é classificado com Prioridade Laranja (muito urgente), finalizando o processo.

Classificação de Rotina (Amarelo e Verde):
Para os demais casos onde não há risco alto ou sintomas graves, o sistema diferencia a gravidade clínica entre as categorias Amarelo (urgente) ou Verde (pouco urgente), concluindo a triagem.
