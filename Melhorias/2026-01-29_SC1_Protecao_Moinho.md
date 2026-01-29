# Melhoria Proposta: SC1 - Proteção do Moinho contra Acionamentos Excessivos

**Data de Identificação:** 29 de Janeiro de 2026  
**Área/Planta:** SC1  
**Equipamento:** Moinho  
**Identificado por:** Diogo Moura  
**Prioridade:** 🟡 Média (Manutenção Preventiva)

---

## 📋 Descrição da Necessidade

O moinho do SC1 necessita de uma **lógica de proteção** (zelo) para evitar acionamentos excessivos em curto período de tempo, que podem causar desgaste prematuro e falhas no equipamento.

---

## ⚠️ Problema Identificado

Atualmente, o moinho pode ser acionado repetidamente sem restrições de tempo, o que pode resultar em:

- **Desgaste mecânico acelerado:** Partidas frequentes aumentam o estresse nos componentes
- **Sobrecarga térmica:** Acionamentos sucessivos podem causar aquecimento excessivo do motor
- **Redução da vida útil:** Ciclos de liga/desliga frequentes reduzem a durabilidade do equipamento
- **Risco de falha prematura:** Maior probabilidade de quebras e paradas não programadas

---

## 🔧 Melhoria Proposta

Implementar uma **lógica de proteção inteligente** no CLP para controlar os acionamentos do moinho:

### 1. **Contador de Acionamentos**
- Monitorar o número de partidas em uma janela de tempo definida
- Exemplo: máximo de 3 acionamentos em 10 minutos

### 2. **Temporizador de Intervalo Mínimo**
- Definir tempo mínimo entre acionamentos consecutivos
- Exemplo: mínimo de 2 minutos entre uma parada e uma nova partida

### 3. **Bloqueio Temporário**
- Se o limite de acionamentos for atingido, bloquear novas partidas por um período
- Exemplo: após 5 partidas em 15 minutos, bloquear por 30 minutos

### 4. **Alarmes e Indicações**
- Alarme quando o limite de acionamentos estiver próximo
- Indicação no supervisório do tempo restante para próximo acionamento permitido
- Contador visual de acionamentos realizados

### 5. **Parâmetros Configuráveis**
- Permitir ajuste dos limites via supervisório ou IHM
- Histórico de acionamentos para análise

---

## 📊 Benefícios Esperados

- ✅ Aumento da vida útil do moinho
- ✅ Redução de manutenções corretivas
- ✅ Menor desgaste dos componentes mecânicos
- ✅ Proteção contra uso inadequado do equipamento
- ✅ Redução de custos de manutenção
- ✅ Maior disponibilidade do equipamento

---

## 🛠️ Implementação Técnica

### Recursos Necessários:
- Programação no CLP (lógica de temporização e contagem)
- Atualização de telas no supervisório/IHM
- Testes em ambiente controlado
- Treinamento dos operadores

### Etapas:
1. Definir parâmetros ideais (consultar fabricante/manutenção)
2. Desenvolver lógica no CLP
3. Criar telas de configuração e monitoramento
4. Testar em modo simulação
5. Implementar em produção
6. Monitorar e ajustar conforme necessário

---

## 📅 Status

**Status Atual:** 🟡 Proposto - Aguardando Aprovação  
**Complexidade:** Média  
**Tempo Estimado:** 3-4 dias (desenvolvimento + testes + validação)

---

## 📝 Observações

Esta melhoria é uma **ação preventiva** que pode evitar custos significativos de manutenção e paradas não programadas no futuro. Recomenda-se implementação em janela de manutenção programada.

---

**Documentado por:** Diogo Moura  
**Sistema de Gestão de Atividades - Automação Sumitomo Chemical**
