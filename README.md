Curso Fundamentos de Observabilidade no nextwave(LuisDEV)

### Introdução
 - A medida que a transformação digital cresce exponecialmente, práticas eficazes de monitoramento e observabilidade se tornam cruciais para garantir a estabilidade e o desempenho dos sistemas.

### O que é DevOps ?
 - DevOps é uma metodologia que integra desenvolvedores de software e a area de IT operations (ops) para construir softwares melhores e de maneira mais rápida
 - Desenvolvimento: Deploys frequentes, novas funcionalidades, inovação
 - Operações: Garantir estabilidade orientado ao serviço racionalização

 ### O que é SRE ?
  - Site Reliability Engieering (SRE) é uma metodologia que incorpora um conjunto de princípios e práticas para garantir uma alta confiabilidade a sistemas

### Monitoramento vs Observabilidade
 - Monitoramento é uma ferramenta ou solução técnica que permite as equipes observar e entender o estado de seus sistemas, baseada na coleta de métricas ou logs pre-definidos
 - Observabilidade é uma ferramenta ou solução técnica que permite as equipes depurar ativamente seu sistema, baseada na exploração de propriedades e padrões não definidos previamente

### Beneficios da Observabilidade
 - A observabilidade desempenha um papel critico em operações de sistemas complexos e oferece diversos beneficios importantes. Aqui estão alguns pontos que destacam a importancia da observabilidade:
   - Identificação Rápida de problemas
   - Compreensão do estado de saúde
   - Resolução eficiente de problemas
   - Otimização de Desempenho
   - Tomada de Decisões baseada em dados
   - Plenajamento e Previsão
   - Segurança e conformidade
   - Melhoria contínua
   - Visibilidade de sistemas distribuidos
   - Experiencia do usuario aprimorada
   - Melhor visibilidade
   - Melhor Alerta
   - Melhor fluxo de trabalho
   - Menos Tempo em Reuniões (war-rooms)
 - SEM OBSERVABILIDADE SOMOS COMO PILOTOS DE AVIÕES COM TODOS OS INSTRUMENTOS DESLIGADOS

### Pilares da Obervabilidade
 - Metrics
 - Logs
 - Traces

 ### Medindo Confiabilidade
  - Engenharia de confiabilidade de Site utiliza SLIS, SLOs e Error Budget para medir a confiabilidade
  - Tem como objetivo demonstrar a satisfação do usuario
  - É comumente utilizado como um equibíbrio entre "Novas Funcionalidades" e "Confiabilidade"

### MELT (Métricas, Eventos, Logs e Traces)
 - Observabilidade é fundamental para entender a saúde e o desempenho do sistema e a estrutura MELT (Métricas, Eventos, Logs e Traces) oferece uma abordagem abrangente para observabilidade, fornecendo insights valiosos sobre a integridade, o desempenho e o comportamento do sistema.
 - Telemetria refere-se a coleta e transmissão automática de dados de fontes remotas para um local centralizado para monitoramento e análise.
   - Categorias de Dados de Telemetria:
     - Métricas (Metrics)
     - Eventos (Events)
     - Registros (Logs)
     - Traços (Traces)
   - Importância do MELT
     - Permite a detecção rápida de problemas, diagnósticos e resolução. Otimiza o desempenho geral do sistema.
 - Métricas:
   -  Medidas numéricas para o desempenho de alto nível do sistema
   -  Exemplos: Uso de CPU, Taxa de Erros.
   -  Vantagens: Retenção de dados, consulta simplificada, análise de tendências.
 - Eventos:
   - Ocorrências discretas com carimbos de data/hora
   - Usados para rastrear eventos cruciais e detectar problemas
   - Exemplos: Tentativas de login de usuário, Notificações de alerta
 - Logs:
   - Registros descritivos do comportamento do sistema.
   - Essenciais para depuração e segurança
   - Vários formatos (texto, JSON) para consulta.
 - Traces:
   - Captura o fluxo de solicitações de ponta a ponta em sistemas distribuídos.
   - Espansões representam operações individuais dentro dos traços.
   - Oferece insights sobre desempenho e comportamento.
   
 ### Como Monitorar e Observar ?
  - Os quatro sinais de ouro do monitoramento são:
  - Latência: o tempo necessário para atender a uma solicitação - "Slow is the new down."
  - Tráfego: quanto demanda está sendo colocada em seu sistema.
  - Erros: a taxa de solicitações que falham
  - Saturação: o quão "cheio" está o seu serviço.
  - Observação: Se você só pode medir quatro métricas do seu sistema voltado para o usuário, concentre-se nestes quatro.

      
      
