# Meta Ads Reporter

Ferramenta para gerar relatórios completos de campanhas do Facebook/Meta Ads a partir de arquivos exportados do Ads Manager.

## Como usar

1. Acesse o site (GitHub Pages)
2. Exporte seu relatório do Meta Ads Manager em `.csv`, `.xlsx` ou `.xls`
3. Arraste o arquivo para a tela
4. O relatório completo é gerado automaticamente no browser — nenhum dado é enviado para servidor

## O que é gerado

- KPIs: gasto total, impressões, alcance, CPM médio, CTR, leads, compras, receita, ROAS, custo por compra
- Gráficos: gasto por campanha, ROAS ranking, gasto × receita, distribuição de impressões
- Insights automáticos: avaliação de ROAS, melhor campanha, alertas de custo alto, CTR
- Tabela detalhada por campanha com todas as métricas

## Como subir no GitHub Pages

```bash
# 1. Crie um repositório no GitHub (ex: meta-ads-reporter)

# 2. Clone e adicione os arquivos
git clone https://github.com/SEU_USUARIO/meta-ads-reporter.git
cd meta-ads-reporter
# copie o index.html para esta pasta

# 3. Faça o push
git add .
git commit -m "initial commit"
git push origin main

# 4. Ative o GitHub Pages
# GitHub → Settings → Pages → Source: main branch → Save
# Seu site estará em: https://SEU_USUARIO.github.io/meta-ads-reporter
```

## Colunas suportadas (Meta Ads Manager)

O sistema detecta automaticamente as colunas em português e inglês:

| Métrica | Coluna no CSV |
|---|---|
| Nome | Nome da campanha |
| Gasto | Valor usado (BRL) |
| Impressões | Impressões |
| Alcance | Alcance |
| CPM | CPM (custo por 1.000 impressões) (BRL) |
| Cliques | Cliques no link |
| CTR | CTR (taxa de cliques no link) |
| Leads | Leads |
| Compras | Compras |
| Receita | Valor de conversão da compra |
| Custo/compra | Custo por compra (BRL) |

## Tecnologias

- HTML/CSS/JS puro — sem framework, sem backend
- [Chart.js](https://www.chartjs.org/) — gráficos
- [PapaParse](https://www.papaparse.com/) — leitura de CSV
- [SheetJS](https://sheetjs.com/) — leitura de Excel

## Privacidade

Todos os dados são processados localmente no browser. Nenhuma informação é enviada para servidores externos.
