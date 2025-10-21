# Cálculo dos Volumes

O módulo de cálculo de volumes tem como objetivo estimar o volume bruto recebido e o volume líquido disponível para venda, considerando fatores de desconto.

## Metodologia sequencial

Aplicamos descontos de forma sequencial e acumulativa, na ordem que melhor reflete o processo operacional:

1. **Volume Bruto Recebido** — quantidade total de sacas recebidas.  
2. **Desconto por Umidade** — redução por umidade acima do padrão.  
3. **Perda de Processo** — perdas durante beneficiamento.  
4. **Perdas de Armazenagem** — perdas em estoque.  
5. **Sobra de Inventário** — percentual reservado como estoque residual.

### Fórmula (sequencial)
Seja `V0` o volume bruto. Aplicando sucessivos descontos `d1, d2, ...`:

```
V1 = V0 * (1 - d1)
V2 = V1 * (1 - d2)
...
Vn = V(n-1) * (1 - dn)
```

### Exemplo prático
Volume bruto recebido: **100 sacas**  
Desconto de umidade: **2%**  
Perda de processo: **25%**  
Perda de armazenagem: **7%**  
Sobra de inventário: **4%**

Aplicando sequencialmente, obtém-se o volume líquido ≈ **68 sacas**.

!!! tip
    Use planilhas auxiliares para versionar cálculos e comparar resultados entre cenários.
