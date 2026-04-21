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

### Por que Monitorar e Observar Proativamente?
 - Monitoramento proativo se dá através de Alerts, Incidents, Anomalies, Monitors, Triggers and Notifications
 - Analisar tendências e antecipar o futuro
 - Comparar dados dos sistemas ao longo do tempo
 - Alertas
 - Dashboads, visualização dos dados
 - Análise de causa raiz (Root cause Analysis - RCA)

 ### Alertas
  - Monitoramento Reativo
    - Alertar apenas quando existe um problema
    - ex: Alta taxas de erros 500 há mais 10 minutos
  - Monitoramento Proativo
    - Alertar antes da falha
    - ex: Uso de CPU acima de 90% pelos últimos 10 miutos, podendo causar lentidão na aplicacão
  - Monitoramento Preditivo
    - Alertar sobre possíveis falhas que ocorrerão no futuro
    - ex: Algoritmos Machine Learning para previsão de falha em memória ou disco
  - Monitoramento Preditivo
    - Monitoramento proativo se dá através de Alertas, Incidents, Anomalies, Monitors, Triggers e Notifications
    - Monitoramento Proativo Através de Alertas
      - Monitorar e alertar são ações essenciais que permitem que um sistema nos avise quando está com problemas, ou até mesmo nos informe quando algo está prestes a falhar
    - O Papel dos Alertas
      - Quando o sistema não pode se corrigir automaticamente, é importante que um humano investigue o alerta, determine se há um problema real, mitigue o problema e identifique a causa raiz
    - Design de Alertas Eficazes
      - Ao criar um alerta, é fundamental pensar em planos de ação e nas pessoas responsáveis por respondê-los.
    - Considerações na Criação de Alertas
      - Qualidade é mais importante que quantidade - AQM (Alert Quality Management)
      - Alertas devem ser reconhecidos.
      - Procedimentos operacionais padronizados (runbooks) são essenciais. Um runbook é um guia detalhado sobre como realizar uma tarefa comum nas operações de TI de uma empresa
      - O objetivo final é, quase sempre, a automação, incluindo automação com AIOps.

### Incident Response
 - O gerenciamento de incidentes restaura o serviço o mais rápido possível usando uma equipe de plantão (first responders) equipada com automação e procedimentos bem definidos, como por exemplo os runbooks.
 - Utiliza alertas e monitoramento proativo para detectar falhas
 - Em casos de incidentes complexos, especialistas no assunto (Subject Matter Experts - SMEs) colaboram na investigação e resolução
 - As capacidades incluem: correlação de eventos, monitoramento, monitoramento de logs, colaboração, notificação, dashboards e procedimentos operacionais padronizados (runbooks).
 - O Gerenciamento de Incidentes desempenha um papel crucial na manutenção da qualidade e disponibilidade do serviço, alinhando-se com os princípios da observabilidade, como monitoramento, correlação de eventos e registros

### Postmortem
 - Aprendendo com Falhas
 - Também conhecido como Blameless PostMortem, ou "Pós-Mortem Sem Culpa"
 - A ideia não é atribuir culpa a alguém, mas encontrar a causa raiz de um incidente e criar ações para resolvê-lo.
 - Objetivos Principais de um PTM:
   - Garantir que o incidente seja documentado.
   - Root Cause Analysis (RCA): compreender bem todas as causas raiz que contribuíram para o incidente.
   - Action Items: implementar ações preventivas eficazes para mitigar ou evitar a probabilidade de recorrência.
 - Um bom PTM só é possível com observabilidade, monitoramento e alertas configurados.
 - Do ponto de vista de um SRE, sempre que esgota-se o error budget de um serviço, deve-se realizar um PTM
 - Sempre que ocorre um incidente de Severidade 1, que afete um serviço crítico ou afete muitos usuários, um PTM é recomendado.
 - Apontar Dedos - Errado
 - Sem Culpa - Correto

 ### AIOps
  - O que é AIOps?
    - AIOps (Artificial Intelligence for IT Operations) é uma abordagem que combina Inteligência Artificial (IA) e aprendizado de máquina com operações de TI tradicionais para aprimorar o monitoramento e a resolução de incidentes.
  - Benefícios do AIOps:
    - Tempo Médio de Resolução (Mean Time do Resolve - MTTR) e Tempo Médio de Detecção (Mean Time do Detect - MTTD) mais rápidos
    - Menores Custos Operacionais
    - Mais Observabilidade e Melhor Colaboração
    - Auxilia no monitoramento proativo e preditivo
  - Como o AIOps Funciona:
    - O AIOps usa uma plataforma de big data para agregar dados de operações de TI, incluindo histórico de desempenho, registros de eventos em tempo real, métricas de sistema e muito mais
    - Ele aplica análises e recursos de machine learning para separar alertas significativos do ruído, identificar causas raiz e sugerir soluções.( Ambos New Relic e Datadog fazem isso com Alerts & AI e Watchdog)
    - A automação permite respostas rápidas, incluindo resolução proativa em tempo real.
  - Casos de Uso de AIOps:
    - Análise de Causa Raiz: Identifica e remedia as causas raiz dos problemas.
    - Detecção de Anomalias: Identifica outliers nos dados para prever eventos problemáticos.
    - Monitoramento de Desempenho: Acompanha o desempenho e otimiza a infraestrutura de TI.

### APM & Observabilidade 
 - New relic (é pago)
 - DataDog (é pago)
 - Dynatrace
 - Honeycomb.io
 - Grafana (Open Source, gratuita)
 - Elastic (Open Source, gratuita)

 ### OpenTelemetry vs APM agents
  - OpenTelemetry é uma estrutura de observabilidade de código aberto para rastrear métricas, eventos, logs e traços em sistemas distribuídos.
  - O agente OTeL instrumenta o código da aplicação para capturar dados do sistema. Todas as ferramentas de APM também seus agentes proprietários.
  - Benefícios do OpenTelemetry (OTel) vs Agents proprietários do New Relic,Datadog, etc:
    - Padrão Aberto
      - Padronização universal vs Soluções proprietárias para observabilidade.
    - Customização
      - Permite controle total sobre quais dados são coletados e como são usados.
      - Permite agregação de dados e sampling na camada do OTeL collector
    - Potencial redução de custos
      - Operação e Manutenção
        - Pois padrão universal não requer aprender as especificidades de cada APM agent
        - evita overhead e complexidade dos times se aprender vários padrões
      - Licenças
        - custo de licenciamento de agentes
      - Sampling
        -  Agregação e amostragem diminui muito a quantidade de dados ingeridos e sobrecarga computacional
      
      
