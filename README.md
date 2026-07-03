# Calculadora AC4 - 19º Comando Regional PMGO

Ferramenta web para auxiliar o policial militar no cálculo de horas e do valor estimado a receber em escalas AC4, com identidade visual do **19º Comando Regional da Polícia Militar de Goiás**, geração de relatório em PDF e previsão de importação da Agenda Google.

> Base normativa declarada: Portaria SSP nº 621/2026 — vigência a partir de 01/07/2026.

## Objetivo

Facilitar ao policial:

- calcular horas de escala;
- diferenciar horas diurnas e noturnas;
- estimar quanto irá receber conforme a tabela oficial vigente;
- lançar escalas manualmente;
- importar eventos do Google Agenda conforme parâmetros definidos;
- gerar relatório em PDF para salvar, imprimir ou anexar em conferência administrativa.

## Identidade visual

O projeto deve utilizar o brasão do **19º CRPM/PMGO** no cabeçalho da aplicação e no relatório gerado em PDF.

Caminho recomendado para o arquivo:

```txt
assets/brasao-19crpm.png
```

## Como usar — MVP previsto

1. Acessar a versão online pelo GitHub Pages.
2. Preencher dados do policial.
3. Configurar a tabela oficial de valores AC4 vigente.
4. Lançar escalas manualmente ou importar agenda.
5. Conferir horas e valor estimado.
6. Clicar em **Gerar PDF / imprimir** e selecionar **Salvar como PDF** no navegador.

## Importação da Agenda Google

A primeira versão deve usar importação por arquivo `.ics`, exportado pelo próprio policial no Google Agenda.

Parâmetros mínimos:

- período inicial e final;
- palavras-chave como `AC4`, `extra`, `escala` ou `serviço extraordinário`;
- pré-visualização dos eventos importados;
- confirmação antes de adicionar ao cálculo.

A integração direta com Google Agenda por OAuth fica prevista para fase futura, pois exige credenciais Google, consentimento, política de privacidade e tratamento seguro de tokens.

## PDF

O relatório em PDF deve conter:

- brasão do 19º CRPM;
- dados do policial;
- mês de referência;
- lista de escalas;
- horas diurnas e noturnas;
- valor estimado por escala;
- valor total estimado;
- aviso de conferência administrativa.

## Documentação

- [`docs/ESCOPO_MVP.md`](docs/ESCOPO_MVP.md) — escopo funcional do MVP com brasão, cálculo, PDF e importação da agenda.

## Observação

Esta ferramenta é de apoio e simulação. O pagamento final depende da conferência administrativa, da escala validada e da tabela oficial vigente.
