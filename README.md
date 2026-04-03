# fiap-mdi-cp1-sre-mobile

## a) Sobre o Projeto

O **FIAP Status & SRE Mobile** foi desenvolvido para atender ao desafio do Checkpoint 1 da disciplina de Mobile Development and IoT, com foco em monitoramento proativo de infraestrutura. A proposta do app e oferecer uma visao de bolso para o time de NOC acompanhar a saude dos servicos criticos e do datacenter da faculdade, reduzindo o tempo de resposta a incidentes e melhorando a confiabilidade operacional.

## b) Integrantes do Grupo

- Enzo Almeida RM556900
- Guilherme Moreira RM557290

## c) Como Rodar o Projeto

1. Clone este repositorio.
2. Acesse a pasta do projeto.
3. Instale as dependencias:

```bash
npm install
```

4. Execute o projeto com Expo:

```bash
npx expo start
```

5. Abra no emulador Android/iOS ou no app Expo Go via QR Code.

## d) Demonstracao

<!-- Inserir GIF da navegacao por abas (Uptime, Datacenter, Incidentes) -->
<!-- Inserir print da tela de Uptime com mudanca de status para Falha -->
<!-- Inserir print da tela de Datacenter com alerta de temperatura -->
<!-- Inserir GIF/print da acao de Reconhecer Falha em Incidentes -->

## e) Decisoes Tecnicas

- **Bottom Tab Navigator** foi escolhido para navegacao principal por permitir acesso rapido e direto as tres areas mais importantes do app (Uptime, Datacenter e Incidentes), alinhado ao uso operacional de times de infraestrutura.
- **useState** foi utilizado para controlar estados locais de servicos, sensores e incidentes, mantendo o comportamento reativo da interface.
- **useEffect** foi utilizado para simular comportamento assincrono, como verificacoes periodicas de disponibilidade e variacao de telemetria IoT (ex.: temperatura), reproduzindo cenarios reais de monitoramento.

## f) Proximos Passos

Como evolucao para um contexto de carreira e mercado corporativo, o proximo passo e integrar o app a fontes reais de observabilidade e sensores, com envio de metricas para nuvem via AWS CloudWatch (ou servicos equivalentes em Azure/GCP), implementando alertas em tempo real, dashboards mais robustos e rotinas de resposta automatizada. Essa evolucao aproxima o projeto das praticas modernas de DevOps/SRE, incluindo telemetria centralizada, automacao operacional, confiabilidade de servicos e cultura orientada a dados.
