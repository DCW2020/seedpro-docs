# Exemplos Práticos

## Cálculo sequencial de volumes (repetição do exemplo)
- Volume bruto: 100 sacas  
- Umidade: 2%  
- Perda processo: 25%  
- Armazenagem: 7%  
- Sobra: 4%  
Resultado aproximado: **68 sacas**

## Verificação de consistência de custos
1. Calcule a demanda de semente básica: `SemBasHect * TotalHect`.  
2. Consulte a tabela `Cad_Preço_SemBasica` para obter `Preço` por cultivar.  
3. Multiplique para obter `CustoSemBasica`.

!!! tip
    Se algum resultado não bater com o orçado (ex.: gestor espera R$ 2.302.000 e sua planilha mostra outro número), confira:
    - valores unitários usados nas tabelas de referência,
    - se há custos externos ou impostos não contabilizados,
    - se houve troca de unidades (kg ↔ saca).
