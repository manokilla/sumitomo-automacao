# Relatório Diário de Ocorrências (RDO)

**Data:** 05 de fevereiro de 2026 (Quinta-feira)  
**Responsável:** Diogo Moura  
**Empresa:** Sumitomo Chemical  
**Período:** Integral


---

## Atividades Realizadas

### 1. SC2/EW | Mapeamento de messages para comunicação entre CLPs

**Área:** SC2 / EW - Comunicação entre plantas  
**Planta/Equipamento:** Sistema de Boiler - Válvulas e bombas  
**Tipo de Atividade:** Desenvolvimento / Integração  

**Descrição:** Iniciado mapeamento de messages (blocos lógicos Rockwell) para permitir comunicação entre CLP do EW e CLP do SC2, especificamente para controle de válvulas e bombas do sistema de Boiler.

**Atividades desenvolvidas:**
- Mapeamento de válvulas do sistema Boiler no SC2
- Mapeamento de bombas do sistema Boiler no SC2
- Configuração de blocos lógicos messages (Rockwell)
- Estruturação de comunicação EW → SC2

**Status:** 🔄 Em andamento

**Período:** Manhã e tarde

**Observações:**
- Trabalho necessário para permitir leitura e escrita no SC2 através do EW
- Mapeamento parcial concluído, continuidade necessária

---

### 2. Infraestrutura | Configuração plataforma Invenze

**Área:** Infraestrutura  
**Equipamento:** Invenze (plataforma de gerenciamento Control ID)  
**Tipo de Atividade:** Configuração / Integração  

**Descrição:** Configuração da plataforma Invenze para gerenciamento dos leitores faciais Control ID e controle de catracas do campus Sumitomo.

**Atividades desenvolvidas:**
- Configuração inicial da plataforma Invenze
- Integração com sistema Control ID
- Ajustes de parâmetros de comunicação
- Tentativa de estabelecimento de comunicação

**Status:** 🔄 Em andamento

**Período:** Manhã (~10h)

**Observações:**
- Comunicação ainda não estabelecida completamente
- E-mail enviado ao suporte do software
- Aguardando resposta técnica

---

### 3. Boiler | Continuação do mapeamento do sistema

**Área:** Boiler - Multi-plantas  
**Planta/Equipamento:** Sistema de Boiler  
**Tipo de Atividade:** Análise / Mapeamento  

**Descrição:** Continuidade do trabalho de mapeamento e levantamento da lógica do sistema de boiler iniciado no dia anterior.

**Atividades desenvolvidas:**
- Continuação do levantamento de lógica
- Mapeamento de componentes
- Análise de integração multi-plantas

**Status:** 🔄 Em andamento

**Período:** Tarde

**Observações:**
- Trabalho em andamento para conclusão do mapeamento completo

---

### 4. EW - Emulsão | Ajuste de pressão bomba tanque de gel

**Área:** EW - Emulsão Óleo em Água  
**Planta/Equipamento:** Bomba de envio tanque de gel (Mixer 60132)  
**Tipo de Atividade:** Ajuste / Parametrização  

**Descrição:** Ajuste do setpoint de pressão da bomba de envio do tanque de gel.

**Atividades desenvolvidas:**
- Alteração de setpoint de pressão: 3 bar → 4 bar
- Validação operacional
- Acompanhamento de funcionamento

**Status:** ✅ Concluído

**Período:** Tarde

**Observações:**
- Ajuste realizado com sucesso
- Sistema operando conforme novo parâmetro

---

### 5. EW - Emulsão | Desenvolvimento de lógica de controle de agitadores

**Área:** EW - Emulsão Óleo em Água  
**Planta/Equipamento:** Agitadores 3098 e 200342  
**Tipo de Atividade:** Desenvolvimento / Automação  

**Descrição:** Desenvolvimento de lógica de controle para permitir desligamento manual dos agitadores quando atendem condição de nível.

**Problema identificado:**
- Agitadores permanecem em modo automático mesmo quando operador coloca em manual
- Impossibilidade de desligar agitadores quando necessário

**Solução desenvolvida:**
- Lógica que permite desligamento manual quando condição de nível é atendida
- Controle de modo automático/manual aprimorado
- Segurança operacional mantida

**Atividades desenvolvidas:**
- Desenvolvimento da lógica de controle
- Programação no CLP
- Testes de validação

**Status:** ✅ Concluído

**Período:** Tarde

**Observações:**
- Lógica desenvolvida e pronta para uso
- Aguardando liberação para ativação em campo
- Sistema testado e validado

---

### 6. EW - Emulsão | Análise de alteração de RPM de agitador

**Área:** EW - Emulsão Óleo em Água  
**Planta/Equipamento:** Sistema de agitação  
**Tipo de Atividade:** Análise / Planejamento  

**Descrição:** Análise técnica em conjunto com equipe KMCC sobre possibilidade de alteração de RPM de agitador.

**Atividades desenvolvidas:**
- Análise técnica de viabilidade
- Discussão com equipe KMCC
- Avaliação de impactos operacionais

**Status:** 🔄 Em andamento

**Período:** Tarde

**Observações:**
- Aguardando decisão técnica da KMCC sobre viabilidade
- Análise em conjunto para garantir segurança operacional

---

## Resumo do Dia

**Total de atividades:** 6  
**Atividades concluídas:** 2  
**Atividades em andamento:** 4  

**Áreas atendidas:**
- SC2/EW - Comunicação (1 atividade)
- Infraestrutura (1 atividade)
- Boiler - Multi-plantas (1 atividade)
- EW - Emulsão (3 atividades)

**Destaques:**
- Mapeamento de comunicação entre plantas (SC2/EW)
- Desenvolvimento de lógica de controle de agitadores
- Ajuste operacional de pressão

---

## Observações Gerais

- Dia focado em desenvolvimento de integrações e automações
- Múltiplas frentes de trabalho em andamento
- Ajustes operacionais concluídos com sucesso na planta EW
- Aguardando retornos técnicos externos (Invenze, KMCC)

---

## Próximos Passos

- Concluir mapeamento de messages SC2/EW
- Aguardar resposta do suporte Invenze para resolução de comunicação
- Finalizar mapeamento do sistema Boiler
- Liberar lógica de controle de agitadores para operação
- Aguardar decisão KMCC sobre alteração de RPM

---

**Relatório gerado em:** 05/02/2026  
**Assinatura Digital:** Diogo Moura
