Projeto: Manipulação de Emojis, Matrizes Musicais e Playlist de Imagens

Feito na raça por um estudante de CC pouco antes da aula — e surpreendentemente funcionando.

🧠 Visão Geral

Este projeto demonstra, de forma prática, o uso combinado de listas, tuplas e dicionários em Python para resolver três problemas diferentes:

🎨 Manipulação de pixels (emoji como imagem)
🎵 Transformação de matrizes (música)
🎬 Integração de estruturas (animação/playlist)

O foco está em:

Estruturas de dados aninhadas
Iterações com múltiplos níveis (for)
Manipulação respeitando a imutabilidade das tuplas
Uso de métodos importantes (.append(), .items(), .update(), .insert(), .pop(), .keys())
🚀 Como executar
Certifique-se de ter o Python 3 instalado
Salve o código em um arquivo .py
Execute no terminal:
python nome_do_arquivo.py
🧩 Desafio 1 — Filtro de Sombra em Emoji
📌 Objetivo

Aplicar um filtro de sombra em um emoji representado como uma grade 5x5 de pixels RGB.

🧱 Estrutura usada
dict → contém nome e grade
list → linhas da imagem
tuple → pixels (R, G, B)
⚙️ Lógica
Percorre:
dicionário → linhas → pixels (3 níveis de for)
Identifica pixels amarelos (255,255,0)
Cria nova tupla com valores reduzidos pela metade
Mantém os pixels pretos intactos
🎯 Conceitos-chave
Imutabilidade de tuplas
Criação de nova estrutura ao invés de alterar a original
🎵 Desafio 2 — Transposição de Matrizes Musicais
📌 Objetivo

Transpor matrizes 2x2 representando frequências musicais.

🧱 Estrutura usada
dict → biblioteca musical
list → coleção de músicas
tuple → matriz original
⚙️ Lógica
Para cada música:
Lê matriz original

Gera matriz transposta:

[[a, b],
 [c, d]]
  ↓
[[a, c],
 [b, d]]
Armazena resultado em nova estrutura
🎯 Conceitos-chave
Acesso a dados com .items()
Atualização com .update()
Manipulação de índices (linha/coluna)
🎬 Desafio 3 — Playlist de Imagens (Integrador)
📌 Objetivo

Criar uma estrutura que simula uma animação com frames de emoji.

🧱 Estrutura usada
dict → playlist principal
list → frames
tuple → duração e pixels
⚙️ Operações realizadas
➕ Inserção
.insert(0, frame_intro)
Adiciona frame de introdução no início
➖ Remoção
.pop()
Remove último frame
🔁 Iteração
.keys() para acessar o dicionário principal
3 níveis de for:
playlist → frames → pixels
⏱️ Cálculo
Soma da duração total da animação
🎯 Conceitos-chave
Estruturas aninhadas complexas
Manipulação dinâmica de listas
Desempacotamento de tuplas
📊 Saídas do Programa

O programa exibe:

Comparação entre emoji original e com sombra
Visualização com emojis (🟡 ⬛ 🟤)
Matrizes musicais originais e transpostas
Estrutura final da biblioteca
Frames da animação com duração
Tempo total da animação
🧪 Conceitos Praticados
✅ Listas (list)
✅ Tuplas (tuple)
✅ Dicionários (dict)
✅ Loops aninhados (3 níveis)
✅ Métodos:
.append()
.items()
.update()
.insert()
.pop()
.keys()
✅ Imutabilidade
✅ Criação de novas estruturas
✅ Organização de dados complexos
💡 Possíveis melhorias
Transformar em funções reutilizáveis
Adicionar interface gráfica simples
Permitir entrada dinâmica de dados
Exportar resultados (imagem ou JSON)
Suporte a matrizes maiores (não só 2x2)
🏁 Conclusão

Este projeto é um ótimo exercício para entender como estruturas básicas do Python podem ser combinadas para resolver problemas mais interessantes — indo de pixels a música e até simulações de animação.

E o mais importante: tudo isso usando só lógica, loops e estruturas fundamentais.
