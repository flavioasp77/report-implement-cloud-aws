# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS  

**Data:** 25/02/2026  
**Empresa:** Abstergo Industries  
**Responsável:** Flávio Pires  

---

## Introdução  

Este relatório apresenta o processo de implementação de serviços AWS na empresa **Abstergo Industries**, conduzido por **Flávio Pires**.  

O objetivo do projeto foi selecionar e implementar **três serviços estratégicos da AWS** com foco em **redução imediata de custos operacionais em infraestrutura**, mantendo níveis adequados de desempenho, disponibilidade e segurança.

A iniciativa priorizou otimização de recursos computacionais, armazenamento e governança financeira em nuvem.

---

## Descrição do Projeto  

O projeto foi dividido em **três etapas**, cada uma direcionada a uma frente específica de otimização de custos.

---

## Etapa 1: AWS Compute Savings Plans  

- **Nome da ferramenta:** AWS Compute Savings Plans  
- **Foco da ferramenta:** Redução de custos com instâncias EC2 e workloads computacionais  
- **Descrição de caso de uso:**  

Após análise do histórico de consumo das instâncias EC2 da empresa, foi identificado padrão estável de utilização em ambientes de produção.  

A implementação do **Savings Plans** permitiu:

- Redução de até 30–40% nos custos de computação  
- Previsibilidade orçamentária  
- Manutenção da flexibilidade de instância (família, região e sistema operacional)  

**Impacto imediato:** Redução direta da fatura mensal de infraestrutura computacional.

---

## Etapa 2: Amazon S3 Intelligent-Tiering  

- **Nome da ferramenta:** Amazon S3 Intelligent-Tiering  
- **Foco da ferramenta:** Otimização automática de custos de armazenamento  
- **Descrição de caso de uso:**  

Foi identificado grande volume de dados armazenados no S3 sem política de ciclo de vida definida, incluindo arquivos acessados com baixa frequência.

A migração para a classe **S3 Intelligent-Tiering** possibilitou:

- Movimentação automática entre camadas de acesso frequente e infrequente  
- Redução de custos sem necessidade de análise manual contínua  
- Eliminação de riscos de escolha incorreta de classe de armazenamento  

**Impacto imediato:** Redução no custo por GB armazenado, especialmente em dados pouco acessados.

---

## Etapa 3: EC2 Auto Scaling + Instâncias Graviton  

- **Nome da ferramenta:** EC2 Auto Scaling com instâncias AWS Graviton  
- **Foco da ferramenta:** Eficiência computacional e otimização de capacidade  
- **Descrição de caso de uso:**  

Foram identificados servidores superdimensionados operando com baixa taxa média de utilização de CPU (<40%).

A estratégia aplicada envolveu:

1. Implementação de **Auto Scaling Groups**  
2. Substituição gradual por instâncias baseadas em **Graviton (ARM)**, com melhor custo-benefício  
3. Ajuste dinâmico de capacidade conforme demanda real  

**Resultados obtidos:**

- Redução de custos por instância  
- Escalabilidade automática conforme carga  
- Melhor aproveitamento de recursos  

**Impacto imediato:** Diminuição de desperdício de capacidade ociosa.

---

## Conclusão  

A implementação dos serviços AWS na **Abstergo Industries** resultou em:

- Redução imediata de custos operacionais  
- Melhor governança financeira em nuvem  
- Maior eficiência na utilização de recursos  
- Escalabilidade automática conforme demanda  
- Otimização contínua sem aumento de complexidade operacional  

A continuidade do monitoramento através de relatórios de custo (AWS Cost Explorer e Budgets) é recomendada para manter a eficiência financeira do ambiente.

Recomenda-se ainda a avaliação futura de:

- Rightsizing contínuo de instâncias  
- Uso de instâncias Spot para workloads tolerantes a interrupção  
- Implementação de políticas automatizadas de lifecycle em todos os buckets  

---

## Anexos  

- Relatório de consumo AWS (últimos 3 meses)  
- Planilha comparativa de custos antes/depois  
- Arquitetura atualizada da infraestrutura  
- Política de ciclo de vida S3 implementada  
- Documento de estratégia de Savings Plans  

---

**Assinatura do Responsável pelo Projeto:**  

Flávio Pires
