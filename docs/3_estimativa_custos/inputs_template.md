# Inputs do Template

Os principais campos de input esperados no template:

- **Versão** → Identificação da versão do modelo ou cenário.  
- **Cultivar** → Variedade de soja utilizada.  
- **Obtentor** → Empresa responsável pela obtenção genética da cultivar.  
- **Tecnologia** → Tecnologia embarcada (ex: Intacta, Convencional, RR, etc.).  
- **Período** → Safra ou ciclo de produção.  
- **Modelo** → Estrutura de simulação (padrão, stress test, otimista, etc.).  
- **Fornecedor** → Fornecedor da semente.  
- **Destinação** → Finalidade (grão, exportação, semente, etc.).  
- **Praça** → Localidade de plantio.  
- **QuantComBB** → Quantidade de sementes comerciais em big bags.  
- **QuantTSIBB**, **QuantSemTSIBB** → Quantidades por tipo.  
- **PMS** → Peso de mil sementes.  
- **RendHectPlantio**, **RendHectComercial** → Rendimento esperado (kg/ha).  
- **SemBasHect** → Semente básica necessária por hectare.  
- **PerdaProcess**, **PerdaArm**, **PerdaQualidade** → Percentuais de perda.  
- **Bonific**, **QuebraTec**, **CampoCancProd**, **Secagem** → Outros ajustes de custo.

!!! example "Verificação rápida"
    Faça uma checagem simples: multiplique `SemBasHect * TotalHect` para validar a demanda total de semente básica.
