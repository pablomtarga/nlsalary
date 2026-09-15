# Loonstrook

Calculadora de salário líquido na Holanda para quem recebe por hora (€ 14,99 bruto).

Você informa as horas trabalhadas por semana ou no mês e a página mostra:

- total líquido da semana e do mês
- bruto, desconto e líquido por hora, dia, semana e mês
- quanto é descontado e por quê (loonbelasting, volksverzekeringen, heffingskorting e arbeidskorting)
- outros descontos esperados: pensão da horeca (PH&C, estimativa), seguro saúde e vakantiegeld
- horas diferentes em cada semana do mês

As horas ficam salvas no navegador (localStorage).

## Como usar

É um arquivo só, sem dependências. Abra o `index.html` no navegador.

Para publicar no GitHub Pages: suba o `index.html` na raiz do repositório, vá em Settings -> Pages, escolha a branch `main` e a pasta `/ (root)`.

## Como a conta é feita

Mesmo método do [thetax.nl](https://thetax.nl): o bruto da semana é projetado para o ano (x 52), o imposto anual é calculado com as faixas e créditos oficiais e dividido de volta. No modo mês, a projeção é x 12.

Tabelas fiscais incluídas: 2025 e 2026.

O valor do holerite pode variar alguns euros, porque o empregador usa a tabela do período de pagamento. O acerto final acontece na declaração anual (aangifte). A pensão da horeca é uma estimativa.

## Fontes

- [Belastingdienst, tarifas e créditos 2026](https://www.belastingdienst.nl/wps/wcm/connect/nl/voorlopige-aanslag/content/voorlopige-aanslag-tarieven-en-heffingskortingen)
- [Maqqie, pensão horeca 2026](https://maqqie.nl/kennisbank/arbeidsrecht-en-wetgeving/horeca-pensioen-2025-alles-wat-je-moet-weten)
- [Zorgwijzer, prêmios do seguro saúde 2026](https://www.zorgwijzer.nl/zorgverzekering-2026/zorgverzekering-2026-alle-premies-bekend-overzicht)

## Créditos

O cálculo de imposto usa código adaptado de [dutch-tax-income-calculator](https://www.npmjs.com/package/dutch-tax-income-calculator), o motor do thetax.nl, sob licença MIT. Veja `THIRD_PARTY_LICENSES.md`.
