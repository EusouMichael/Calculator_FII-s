# FII Investment Tracker

MVP local de acompanhamento e simulação educacional de investimentos em Fundos de Investimento Imobiliário (FIIs).

## Objetivo

O projeto separa duas finalidades:

- **Acompanhamento:** registrar lançamentos e acompanhar posições próprias.
- **Simulação/educação:** testar cenários matemáticos e consultar conceitos sobre FIIs.

A aplicação não fornece recomendação personalizada de compra ou venda.

## Origem do MVP

A lógica inicial foi baseada no protótipo `Treinamento FIIs.xlsx`, especialmente na calculadora da aba `CALCULADORA` e na tabela de apoio de composição por perfil. Os valores presentes na planilha são tratados como exemplos de preenchimento, não como dados de mercado.

A fórmula de valor futuro foi preservada e ampliada com:

- capital inicial;
- aporte mensal;
- prazo;
- taxa mensal hipotética;
- inflação anual;
- patrimônio nominal;
- patrimônio em valores reais;
- total aportado;
- rendimento matemático da simulação;
- cenários comparativos.

A tabela de percentuais por perfil não foi convertida em recomendação automática. A aplicação evita apresentar uma alocação como adequada apenas porque o usuário foi classificado em um perfil.

## Funcionalidades

- Dashboard;
- carteira baseada em lançamentos;
- compras, vendas, dividendos, juros/rendimentos, taxas, aportes e resgates;
- atualização manual de preço atual por posição;
- cálculo de valor atual, resultado e rentabilidade;
- metas de patrimônio;
- meta matemática de renda passiva;
- simulador com cenários;
- educação sobre FIIs;
- indicadores e riscos;
- botão **Fontes Oficiais**;
- persistência local via `localStorage`;
- sem API paga e sem dependências externas.

## Como executar

Não é necessário instalar dependências.

1. Abra `index.html` em um navegador moderno.
2. Para uma experiência mais consistente, opcionalmente sirva a pasta por um servidor local, por exemplo com VS Code Live Server.

## Fontes oficiais utilizadas como referência

- B3 — Fundos de Investimento Imobiliário: https://www.b3.com.br/pt_br/produtos-e-servicos/negociacao/renda-variavel/fundos-de-investimento-imobiliario-fii.htm
- B3 — FIIs listados: https://www.b3.com.br/pt_br/produtos-e-servicos/negociacao/renda-variavel/fundos-de-investimentos/fii/fiis-listados/
- CVM — Fundos de Investimento Imobiliários: https://www.gov.br/cvm/pt-br/assuntos/regulados/envio-de-informacoes-a-cvm-calendario/sse/fundos-de-investimento-imobiliarios-fiis
- CVM — Consulta de fundos: https://www.gov.br/cvm/pt-br/assuntos/regulados/consultas-por-participante/fundos-de-investimento
- Portal do Investidor — FIIs: https://www.gov.br/investidor/pt-br/investir/tipos-de-investimentos/fundos-de-investimentos-imobiliarios-fii
- Portal do Investidor — Riscos: https://www.gov.br/investidor/pt-br/investir/tipos-de-investimentos/fundos-de-investimentos-imobiliarios-fii/principais-riscos

## Limitações do MVP

- Não há integração automática com cotações ou dados de mercado.
- Preço atual das posições é informado manualmente.
- Os dados da carteira ficam apenas no navegador utilizado.
- Não há autenticação, backend, sincronização ou pagamentos.
- Os cenários são matemáticos e dependem das premissas inseridas pelo usuário.

## Responsabilidade

Esta ferramenta é informativa e educacional. FIIs são investimentos de renda variável e estão sujeitos a riscos. Consulte os documentos oficiais do fundo, seu regulamento, informes e demais informações disponibilizadas pelos canais oficiais antes de qualquer decisão de investimento.

## Abertura rápida

O `index.html` desta entrega é autocontido: CSS e JavaScript estão embutidos no próprio arquivo. Portanto, para testar o MVP, extraia o ZIP e abra `index.html` diretamente no Chrome/Edge. Os arquivos `styles.css` e `app.js` permanecem na pasta como fontes de manutenção.
