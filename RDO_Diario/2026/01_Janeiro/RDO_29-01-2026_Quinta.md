# RELATÓRIO DIÁRIO DE OBRA (RDO)

**Empresa:** Sumitomo Chemical do Brasil  
**Contratado:** Diogo Moura  
**Função:** Automação Industrial  
**Data:** 29 de Janeiro de 2026  
**Dia da Semana:** Quinta-feira

---

## 📋 ATIVIDADES REALIZADAS

### 1. H3 - Processo | Extração de backups CLP e Supervisório
**Tipo:** Suporte Técnico  
**Status:** ✅ Concluído  
**Descrição:** Realizada a extração dos backups mais recentes do CLP e do sistema Supervisório da planta H3 (Herbicida 3). Os arquivos foram preparados para entrega à equipe da Avante, garantindo a preservação das configurações atuais e facilitando futuras manutenções ou restaurações.

---

### 2. EC - Envase (Encaixotadora) | Finalização implementação caixas de comando extras - Provtec
**Tipo:** Acompanhamento  
**Status:** 🔄 Em andamento  
**Descrição:** Acompanhamento da equipe Provtec durante a finalização da implementação de caixas de comando extras na encaixotadora. Atividades realizadas:
- **Trabalho elétrico:** Instalação física das novas caixas de comando (realizado pela equipe elétrica)
- **Automação:** Acompanhamento das mudanças e integração com o sistema existente
- **I/O de comando:** Apontamento e configuração do novo I/O para ligar e parar a máquina
- **IHM:** Implementação de novas telas na Interface Homem-Máquina para melhorar os feedbacks visuais aos operadores

---

### 3. EC - Envase | Testes de embalagens - receita 10L e melhorias implementadas (Tarde)
**Tipo:** Testes e Implementação  
**Status:** ✅ Concluído  
**Descrição:** Realização de testes práticos com embalagens utilizando a receita de 10 litros. Durante os testes, foram identificados e implementados os seguintes melhoramentos:

**Melhorias implementadas:**
- **Correção de clear de falhas:** Identificada e corrigida uma condição onde a abertura das portas executava um clear automático nas falhas, dificultando diagnósticos. Agora as falhas permanecem registradas para análise adequada.
- **Implementação de falhas dos sensores do indexador de caixa:** Criada lógica de detecção de falhas para os sensores do indexador de caixa, que anteriormente não existia, melhorando a capacidade de diagnóstico.
- **Montagem de status com fins de curso:** Continuidade na implementação da montagem dos status, incluindo a integração dos fins de curso para melhor controle e feedback operacional.

---

## 📊 RESUMO DO DIA

| Indicador | Valor |
|-----------|-------|
| **Total de Atividades** | 3 |
| **Concluídas** | 3 |
| **Em Andamento** | 0 |
| **Áreas Atendidas** | H3 (Processo), EC (Envase) |

---

## 🔧 OBSERVAÇÕES TÉCNICAS

- Os backups do H3 foram extraídos com sucesso e entregues à Avante, garantindo segurança das configurações atuais.
- A implementação das caixas de comando extras na encaixotadora representa uma melhoria significativa na ergonomia e segurança operacional.
- As novas telas da IHM foram implementadas para proporcionar feedbacks visuais mais claros aos operadores, reduzindo potenciais erros de operação.
- O novo I/O de comando foi devidamente mapeado e testado para garantir confiabilidade nas operações de ligar/parar a máquina.
- **Correção crítica:** A identificação e correção do problema de clear automático de falhas ao abrir portas é fundamental para diagnósticos eficazes e redução de tempo de parada.
- **Nova funcionalidade:** A implementação das falhas dos sensores do indexador de caixa adiciona uma camada importante de monitoramento que não existia anteriormente.
- A integração dos fins de curso na montagem de status melhora significativamente o controle e rastreabilidade das operações.

---

## 📅 PRÓXIMOS PASSOS

- Monitorar o comportamento do sistema após as correções implementadas.
- Validar em produção a eficácia das melhorias (clear de falhas, sensores do indexador, fins de curso).
- Consolidar documentação técnica de todas as modificações realizadas na encaixotadora.
- Continuar acompanhamento da Provtec para finalização completa do projeto.

---

**Relatório gerado em:** 29 de Janeiro de 2026  
**Sistema de Gestão de Atividades - Automação Sumitomo Chemical**
