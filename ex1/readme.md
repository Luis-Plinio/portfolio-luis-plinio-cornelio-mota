# Sistema de Auditoria de Vendas Semanais

Este projeto é uma ferramenta em Python desenvolvida para automatizar o processo de monitorização e validação de transações comerciais. O sistema foca-se na análise de médias de vendas, gestão de limites de risco e identificação de anomalias financeiras.

## 🚀 Funcionalidades

O script realiza as seguintes operações:
- **Cálculo de Média:** Processa três valores de venda e gera a média aritmética.
- **Validação de Legitimidade:** Interface interativa para confirmação manual de autenticidade das vendas.
- **Gestão de Limites:** Permite a reconfiguração dinâmica do limite de segurança caso uma irregularidade seja detectada.
- **Estado de Quarentena:** Sistema de alerta para médias que ultrapassam o teto de segurança em vendas não confirmadas.
- **Detecção de Anomalias (Revisão Manual):** Identifica automaticamente se alguma venda individual é desproporcional (5x superior à média), sinalizando a necessidade de auditoria humana.

## 🛠️ Como Funciona

1. **Entrada de Dados:** O utilizador insere os valores de três vendas semanais (`V1`, `V2`, `V3`).
2. **Processamento:** A função `analisar_vendas()` calcula a média e exibe-a no terminal.
3. **Verificação:** O auditor responde se a venda é legítima (`s/n`).
   - Se **'n'**: O sistema solicita um novo limite de segurança e verifica se deve entrar em **QUARENTENA**.
   - Se **'s'**: O sistema prossegue com a confirmação de sucesso.
4. **Análise de Risco:** O software verifica se existe algum valor atípico que exija uma **REVISÃO MANUAL**.
5. **Logs Técnicos:** No final, o sistema imprime o tipo de variável de cada dado processado para garantir a integridade do sistema.

## 📋 Pré-requisitos

* Python 3.x instalado.

## 🖥️ Exemplo de Uso

```text
Valor da venda 1: 1200
Valor da venda 2: 1500
Valor da venda 3: 8000
A média das vendas é: 3566.66
A venda é legitima? (s/n) s
MÉDIA DAS VENDAS NORMAL
REVISÃO MANUAL
