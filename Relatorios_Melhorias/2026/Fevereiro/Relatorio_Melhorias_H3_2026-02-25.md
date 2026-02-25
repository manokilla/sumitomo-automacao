# Relatório de Melhorias Implementadas – Planta H3

**Autor:** Diogo Moura
**Data:** 25 de Fevereiro de 2026

## 1. Objetivo

Este documento apresenta um resumo da melhoria implementada na planta de Herbicidas 3 (H3), conforme solicitação de Natália (Manufatura). A ação foi executada com foco em aumentar a segurança operacional dos equipamentos através da implementação de um novo sistema de proteção para 27 motores da área.

## 2. Melhoria Implementada

### 2.1 Implementação de 27 Intertravamentos de Corrente

**Problema Identificado**

A necessidade de um sistema de proteção mais robusto para os motores da planta H3, especificamente para detectar condições de operação anormais que não eram cobertas pelos intertravamentos existentes. A operação com baixa corrente, por exemplo, pode indicar um problema mecânico ou de processo (ex: bomba operando a seco) que necessita de uma parada segura do equipamento.

**Solução Implementada**

Foi realizado o levantamento e a implementação de uma nova lógica de proteção para **27 motores** (bombas de transferência e agitadores). Para centralizar e padronizar a lógica, foi desenvolvida uma instrução **Add-On (AOI)** customizada, `BreakOpr_Motor_v2`. Esta AOI monitora continuamente o status e a corrente do motor, gerando um alarme e incrementando um contador de eventos sempre que uma condição de falha (baseada em setpoint de corrente e tempo) é detectada.

O bit de alarme gerado pela AOI foi integrado à estrutura de interlocks do motor, garantindo a parada segura do equipamento e fornecendo uma mensagem clara ao operador sobre a causa da falha. As lógicas foram implementadas e testadas, porém se encontram **bloqueadas**, aguardando a definição dos parâmetros finais (valor de corrente e tempo) e a autorização formal para liberação da melhoria.

**Evidências**

| Imagem | Descrição |
|---|---|
| ![Estrutura de Interlocks](assets_2026-02-25/IMG_4683.jpeg) | Lógica de controle do agitador, mostrando a integração do alarme de subcorrente (`AlmLatched`) na cadeia de intertravamento. |
| ![Add-On BreakOpr_Motor_v2](assets_2026-02-25/IMG_4682.jpeg) | Detalhe da Add-On `BreakOpr_Motor_v2` aplicada a dois motores, exibindo os parâmetros de status, corrente e contagem de falhas. |
| ![Mensagem de Alarme](assets_2026-02-25/IMG_4680.jpeg) | Configuração da mensagem de alarme "Subcorrente Motor" que é exibida ao operador no sistema supervisório. |

| Item | Descrição |
|---|---|
| **Equipamentos** | 27 motores (bombas de transferência e agitadores) |
| **Ação** | Implementação de intertravamento de subcorrente via AOI customizada. |
| **Status** | ⏳ Em Avaliação (Aguardando parametrização e liberação) |

## 3. Conclusão

A implementação do novo sistema de proteção por subcorrente representa um avanço significativo na segurança operacional da planta H3. A solução padronizada via AOI facilita a manutenção e a replicação para outros equipamentos no futuro. A melhoria está pronta para ser ativada assim que os parâmetros operacionais forem definidos e a liberação formal for concedida.
