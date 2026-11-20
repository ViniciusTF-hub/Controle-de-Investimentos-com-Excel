# Simulador de Investimentos em Fundos Imobiliários (Excel)

Projeto do desafio **"Controle de Investimentos com Excel"** da [DIO](https://www.dio.me/), com o Expert Felipe Aguiar.

A planilha funciona como um pequeno aplicativo: o usuário informa quanto quer investir por mês, por quantos anos e a taxa de rendimento, e ela calcula o patrimônio acumulado, os dividendos mensais e a divisão do aporte entre tipos de fundo imobiliário (FII) conforme o perfil de investidor.

## Perguntas que a ferramenta responde

- Quanto investir por mês
- Por quantos anos
- Qual a taxa de rendimento mensal
- Quanto de patrimônio vai acumular
- Quanto vai receber de dividendos por mês

## Estrutura da planilha

| Aba | O que tem |
|---|---|
| **Simulador** | Banner, entradas (aporte, anos, taxa), resultados (patrimônio e dividendos), cenários de 2, 5, 10, 20 e 30 anos e divisão do aporte por perfil |
| **Configurações** | Salário, rendimento mensal da carteira e sugestão de aporte (30% do salário) |
| **Apoio** | Tabela de perfil × tipo de fundo × percentual, com chave composta e conferência de que cada perfil soma 100% |

## Recursos do Excel utilizados

- **`VF` (Valor Futuro)** para calcular o patrimônio acumulado com aportes mensais
- **Intervalos nomeados** (`aporte`, `anos`, `taxa_mensal`, `salario`, `sugestao_aporte`, `tabela_perfis`, `lista_perfis`) no lugar de endereços de célula
- **Referências absolutas** na tabela de cenários
- **Validação de dados** com lista suspensa de perfis (Conservador, Moderado, Arrojado)
- **`PROCV` com chave composta** (perfil + tipo de fundo) para buscar o percentual de cada fundo
- **`SOMASE`** para conferir se cada perfil soma 100%
- Layout de "aplicativo": linhas de grade ocultas e células calculadas em cinza

## Como usar

1. Baixe o arquivo `Simulador_FIIs.xlsx` e abra no Excel.
2. Na aba **Simulador**, preencha as células brancas: aporte mensal e número de anos.
3. Ajuste a taxa mensal e o salário na aba **Configurações**.
4. Escolha o perfil na lista suspensa para ver a divisão do aporte.

As células em cinza são calculadas automaticamente e não devem ser editadas.

## Aviso

Os percentuais de cada perfil são apenas um exemplo para fins de estudo e **não são recomendação de investimento**.
