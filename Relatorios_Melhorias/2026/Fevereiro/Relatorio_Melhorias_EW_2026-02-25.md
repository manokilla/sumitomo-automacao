# Relatório de Melhorias Implementadas – Planta EW

**Autor:** Diogo Moura
**Data:** 25 de Fevereiro de 2026

## 1. Objetivo

Este documento apresenta um resumo das melhorias implementadas na planta EW, conforme solicitação de Gfter (Manufatura). As ações foram executadas com foco em otimizar a operação dos equipamentos, aumentar o controle do operador sobre os processos e reforçar a segurança operacional.

## 2. Melhorias Implementadas

### 2.1 Otimização do Controle de Processo – Reator 3098

Foram implementadas duas melhorias no controle do Reator 3098 para otimizar os processos de reciclo e transferência, eliminando a necessidade de intervenção manual do operador e garantindo a conformidade com os parâmetros de processo.

**Resultado**

| Aspecto | Antes | Depois |
|---|---|---|
| **Controle de Reciclo** | Operador precisava ajustar manualmente a velocidade da bomba de 22 RPM para 150 RPM. | Um pulso automático ajusta a velocidade para 150 RPM, mantendo a flexibilidade de controle do setpoint. |
| **Controle de Transferência** | Velocidade da bomba podia ser alterada manualmente. | Velocidade da bomba é fixada em 22 RPM, sem possibilidade de alteração, garantindo a segurança do processo. |
| **Status** | | ✅ Implementado |

### 2.2 Intertravamento de Segurança – Válvulas de Nitrogênio

**Problema Identificado**

Ocorreu um incidente de transbordo em um dos reatores da área EW quando a válvula de admissão de nitrogênio foi acionada enquanto a válvula de fundo do reator estava aberta. A pressurização do tanque aberto resultou na projeção de produto para fora do reator.

**Solução Implementada**

Foi implementado um intertravamento de segurança nos reatores **R8000, R8001, R8002 e R8003**. A nova lógica impede a abertura da válvula de admissão de nitrogênio caso a válvula de fundo do respectivo reator esteja aberta. Essa medida de segurança crítica previne a pressurização indevida de um reator aberto, eliminando o risco de transbordamento.

**Evidências**

| Imagem | Descrição |
|---|---|
| ![Interlock Ativo](assets_EW/IMG_4687.jpeg) | Tela do supervisório mostrando o intertravamento: quando a válvula de fundo (verde) está aberta, a válvula de nitrogênio da linha amarela (AV00184) fica bloqueada com a mensagem "Interlock: Valv. Fundo Aberta". |
| ![Situação Normal](assets_EW/IMG_4686.jpeg) | Situação normal de operação: válvula de fundo fechada (cinza), permitindo que a válvula de nitrogênio da linha amarela (AV00184) possa ser aberta sem intertravamento. |

| Item | Descrição |
|---|---|
| **Equipamentos** | Reatores R8000, R8001, R8002, R8003 |
| **Ação** | Implementação de intertravamento entre válvula de fundo e válvula de nitrogênio. |
| **Status** | ✅ Implementado |

## 3. Conclusão

As melhorias implementadas na planta EW focaram em **aumentar a eficiência operacional e a segurança dos processos**. A otimização do controle do Reator 3098 reduz a carga de trabalho do operador e minimiza a possibilidade de erro humano, enquanto o novo intertravamento nos reatores da série 8000 mitiga um risco de segurança crítico identificado. Todas as ações foram executadas e validadas conforme solicitado.
