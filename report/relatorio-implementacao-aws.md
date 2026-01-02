# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS CLOUD AWS

**Data:** 02/01/2026  
**Empresa:** Abstergo Industries  
**Responsável:** Leonardo Botelho

---

## Introdução

Este relatório apresenta o processo de implementação de serviços em nuvem na empresa **Abstergo Industries**, realizado por **Leonardo Botelho**. O objetivo do projeto foi elencar **serviços Cloud** com a finalidade de promover a **redução imediata de custos operacionais**, aumento da eficiência e maior escalabilidade dos sistemas utilizados no processo de distribuição de produtos farmacêuticos.

A Abstergo Industries atua como um **hub de distribuição**, comunicando-se com diversas farmácias, fornecedores, transportadoras e sistemas externos, o que exige uma infraestrutura tecnológica confiável, flexível e com controle rigoroso de custos.
Com base nessas premissas foram escolhidos os serviços da **Amazon Web Services (AWS)**

---

## Descrição do Projeto

O projeto de implementação de serviços AWS foi dividido em **três etapas**, cada uma com objetivos específicos voltados à otimização financeira e operacional da empresa.

---

### Etapa 1:
- **Nome da ferramenta:** AWS Lambda + Amazon API Gateway  
- **Foco da ferramenta:** Computação sob demanda (Serverless)  
- **Descrição de caso de uso:**  

Nesta etapa, foi proposta a implementação de APIs para integração entre a Abstergo Industries e seus parceiros comerciais, como farmácias, distribuidores e sistemas de ERP. O **Amazon API Gateway** é responsável por gerenciar e expor essas APIs, enquanto o **AWS Lambda** executa as regras de negócio sob demanda, sem a necessidade de servidores dedicados.

A utilização dessa arquitetura elimina a necessidade de investimento em infraestrutura física própria, como servidores, data centers, refrigeração e manutenção de hardware. Mesmo em cenários onde a empresa já possua infraestrutura on-premises, a migração gradual para um modelo serverless possibilita a redução de custos fixos com energia elétrica, contratos de suporte, atualização de equipamentos e mão de obra dedicada à administração de servidores. Além disso, o modelo de pagamento por uso elimina gastos com capacidade ociosa e superdimensionamento, resultando em uma operação mais eficiente e financeiramente sustentável.

**Principal ganho:**  
Escalabilidade automática e alta disponibilidade, com pagamento apenas pelos recursos efetivamente utilizados.

---

### Etapa 2:
- **Nome da ferramenta:** Amazon S3 + S3 Lifecycle + S3 Glacier  
- **Foco da ferramenta:** Armazenamento escalável e de baixo custo  
- **Descrição de caso de uso:**  

Nesta etapa, o **Amazon S3** é utilizado para armazenar documentos regulatórios, notas fiscais, históricos de pedidos, logs de integração e dados de rastreabilidade de lotes, essenciais para o setor farmacêutico. Com o uso das **políticas de lifecycle**, os dados mais antigos ou pouco acessados são automaticamente movidos para camadas de menor custo, como o **S3 Glacier** e o **Glacier Deep Archive**.

Essa estratégia reduz significativamente os custos de armazenamento, principalmente para dados que precisam ser mantidos por longos períodos devido a exigências legais e regulatórias.

**Principal ganho:**  
Redução expressiva dos custos de armazenamento com alta durabilidade, segurança e conformidade regulatória.

---

### Etapa 3:
- **Nome da ferramenta:** Amazon SQS + Amazon SNS  
- **Foco da ferramenta:** Mensageria e integração assíncrona  
- **Descrição de caso de uso:**  

A implementação do **Amazon SQS** permite o uso de filas para o processamento de pedidos e eventos de integração, garantindo que os sistemas internos e externos não sejam impactados por falhas ou picos de demanda. O **Amazon SNS** é utilizado para o envio de notificações a sistemas parceiros, transportadoras e áreas internas da empresa.

Essa abordagem desacopla os sistemas, reduz falhas em cascata e evita a necessidade de infraestrutura superdimensionada para suportar picos ocasionais.

**Principal ganho:**  
Maior resiliência, estabilidade operacional e redução de custos relacionados a falhas e retrabalho.

---

## Conclusão

A implementação dos serviços AWS na empresa **Abstergo Industries** tem como resultado esperado a **redução significativa de custos operacionais**, maior eficiência nos processos de integração e distribuição, além de escalabilidade e confiabilidade dos sistemas.

A adoção de uma arquitetura baseada em **pagamento por uso, computação serverless e integração assíncrona** permite que a empresa cresça de forma sustentável, mantendo controle financeiro e foco em seu core business. Recomenda-se a continuidade da utilização das ferramentas implementadas e a constante avaliação de novas tecnologias que possam aprimorar ainda mais os processos da empresa.

---

## Anexos

- Documentação oficial dos serviços AWS utilizados  
- Diagrama de arquitetura da solução  
- Planilha de estimativa de custos  
- Políticas de armazenamento e retenção de dados  

---

**Assinatura do Responsável pelo Projeto:**  

Leonardo Botelho 
