Aqui está uma proposta de README.md unificando os dois sistemas sob o tema de Gestão e Segurança em Microclimas Urbanos (UNICID).

🏢 Monitoramento e Segurança Urbana: UNICID
Este repositório contém dois sistemas desenvolvidos em Python voltados para a análise ambiental e segurança predial no campus da UNICID (Zona Leste, SP). O projeto une métricas de qualidade do ar e conforto térmico com algoritmos de tomada de decisão para evacuação de emergência.

📊 Parte 1: Análise de Microclima Urbano
Este módulo processa dados ambientais coletados manualmente em pontos estratégicos para calcular o índice de bem-estar da população flutuante.

Funcionalidades
Classificação IQA (Índice de Qualidade do Ar): Baseado nos parâmetros da CETESB, classifica o ar em faixas de Boa a Péssima.

Cálculo de Nota de Conforto (0 a 10): Uma fórmula ponderada que avalia:

Temperatura: Desvios em relação à temperatura ideal de 22°C.

Umidade: Faixa ideal entre 50% e 70%.

IQA: Penalização proporcional à poluição.

Análise Comparativa: Avalia os microclimas do Canteiro Arborizado, Terminal de Ônibus e dependências da Faculdade em horários distintos (Manhã e Tarde).

🏃 Parte 2: Simulador de Evacuação Espacial
Um algoritmo de simulação que modela a trajetória de um agente em uma situação de emergência, partindo do primeiro andar da instituição até as saídas de segurança.

Funcionalidades
Mapeamento de Nós: O trajeto é dividido em pontos reais (Sala de Aula, Corredor, Escadas e Térreo).

Gestão de Recursos e Energia: O agente possui uma barra de energia (100) e um inventário. Obstáculos como "fumaça" exigem o uso de itens (ex: garrafa de água) e consomem mais energia.

Lógica de Tomada de Decisão:

Ao chegar no térreo, o sistema avalia três saídas possíveis.

Um cálculo de Score de Segurança é realizado em tempo real para escolher a rota mais eficiente (Avenida Principal, Rua Lateral ou Lanchonete).

Diferentes resultados possíveis: Evacuação bem-sucedida ou falha por exaustão.

🛠️ Tecnologias Utilizadas
Linguagem: Python 3.10+

Recursos Lógicos:

match/case para classificação de faixas.

while e if aninhados para lógica de navegação.

random e time para simulação de eventos e dinamismo.

📂 Como Executar
Certifique-se de ter o Python instalado.

Clone o repositório ou copie os códigos.

Execute o script da Parte 1 para ver as estatísticas ambientais:

Bash
python analise_clima.py
Execute o script da Parte 2 para iniciar a simulação de emergência:

Bash
python simulador_evacuacao.py
📝 Referências
IQA: Faixas de referência fornecidas pela CETESB (Companhia Ambiental do Estado de São Paulo).

Localização: Mapeamento físico baseado no 1º andar do campus UNICID.

Nota: Este projeto possui fins educacionais e de simulação lógica de sistemas.
