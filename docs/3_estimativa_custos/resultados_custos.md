# Resultados de Custos Calculados

A plataforma gera vários indicadores e linhas de custo. As principais são:

- **CommPonderada** — composição ponderada de custos por praça (preço médio ponderado).
- **CustoSemBasica** — custo total da semente básica utilizada.
- **CustoRevena** — custo de revenda (aplicável a modelo B2B).
- **CustoBonif** — custo líquido após bonificações.
- **CustoMP** — custo da matéria‑prima (sementes).
- **DescBenef**, **DescQuebraTec**, **DescArmaz** — descontos por beneficiamento, quebras técnicas e armazenagem.
- **AjudaFrete**, **FreteCampo** — custos de frete.
- **TaxaMapa**, **Pessoal**, **Indiretos** — custos operacionais e regulatórios.
- **CustoBenef**, **RoyBio**, **RoyGerm**, **TSI**
- **TotalCOGM**, **CustoUnitKg**, **CustoUnit40Kg**, **CustoUnit60Kg**, **CustoUnitBB**

## Fórmulas de exemplo

### Preço médio ponderado por praça (CommPonderada)
```
Se Modelo = "B2B" -> 0
SENÃO:
PrecoMedio = SUMIF(Commodity[Praça], [@Praça], Commodity[ValorTotal]) / SUMIF(Commodity[Praça], [@Praça], Commodity[VolTotal])
```

### Custo da semente básica (CustoSemBasica)
```
Se Modelo = "B2B" -> 0
SENÃO:
CustoSemBasica = PrecoUnitarioCultivar * (SemBasHect * TotalHect)
```

!!! example "Ilustração"
    Modelo: Produção Própria  
    Cultivar: SOJA 58  
    Preço unitário: R$ 120,00/ha  
    SemBasHect: 1,2 sacas/ha  
    TotalHect: 500 ha  
    Resultado: R$ 72.000
