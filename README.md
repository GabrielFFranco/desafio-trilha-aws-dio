# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 21 de agosto de 2025  
**Empresa:** Abstergo Industries  
**Responsável:** Gabriel Ferreira Franco

## Introdução

Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Gabriel Ferreira Franco. O objetivo do projeto foi elencar 4 serviços AWS, com a finalidade de realizar diminuição de custos imediatos, além de aumentar a eficiência de processos logísticos, administrativos e de acesso a sistemas globais da empresa.

## Descrição do Projeto

O projeto de implementação de ferramentas foi dividido em 4 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

## Etapa 1
**Amazon EC2 + VPC (Virtual Private Cloud)**  
**Foco da ferramenta:** Hospedagem segura e escalável de aplicações internas.  
**Descrição de caso de uso:**  
A Abstergo utilizava servidores locais para rodar aplicações internas administrativas e sistemas de RH. Com a implementação de instâncias EC2 dentro de uma VPC personalizada, foi possível migrar essas aplicações para a nuvem, garantindo alta disponibilidade, segurança (com uso de NACLs e grupos de segurança) e controle de acesso por sub-redes privadas e públicas.

## Etapa 2
**Regiões, Zonas de Disponibilidade e Pontos de Presença (Edge Locations)**  
**Foco da ferramenta:** Redução de latência e aumento de disponibilidade global.  
**Descrição de caso de uso:**  
A Abstergo Industries possui unidades e usuários em diferentes partes do mundo, incluindo América, Europa e Ásia. Para garantir uma experiência de acesso rápido e confiável aos serviços hospedados na AWS, foi feito o uso estratégico de **Regiões** e **Zonas de Disponibilidade (AZs)** da AWS para distribuir cargas de trabalho entre diferentes localidades geográficas. Além disso, foram configurados **Pontos de Presença (Edge Locations)**, por meio do **Amazon CloudFront**, para distribuir conteúdo estático (como páginas da intranet, documentos e dashboards) com **menor latência** aos usuários finais. Essa abordagem também garante **redundância geográfica**, aumentando a resiliência da infraestrutura contra falhas locais e mantendo os sistemas críticos sempre acessíveis.

## Etapa 3
**Amazon S3 (Simple Storage Service)**  
**Foco da ferramenta:** Armazenamento seguro e escalável de documentos e dados clínicos.  
**Descrição de caso de uso:**  
A Abstergo Industries lida com grandes volumes de documentos, como laudos clínicos, dados de pesquisas, prontuários e registros de conformidade regulatória. Antes da migração para a nuvem, esses dados eram armazenados em servidores físicos caros e de difícil manutenção. Com a implementação do Amazon S3, os dados foram migrados para um ambiente altamente disponível, seguro e com custo otimizado. Além disso, o uso do **S3 Intelligent-Tiering**, permite mover dados menos acessados para classes de armazenamento mais baratas, reduzindo custos significativamente.

## Etapa 4
**Amazon RDS (Relational Database Service)**  
**Foco da ferramenta:** Gerenciamento de banco de dados para o sistema de controle de estoque e logística.  
**Descrição de caso de uso:**  
O sistema logístico da Abstergo dependia de um banco de dados local para rastrear medicamentos, insumos e matérias-primas entre os centros de distribuição e laboratórios. Com o Amazon RDS, foi possível migrar esse banco de dados relacional para a nuvem, automatizando backups, atualizações e escalabilidade. O desempenho do sistema irá aumentar e a equipe de TI foi liberada de tarefas operacionais, reduzindo custos com suporte técnico e melhorando a resposta em tempo real para o gerenciamento de estoque.

## Conclusão

A implementação de ferramentas na empresa Abstergo Industries tem como esperado a redução de custos com infraestrutura física, aumento da escalabilidade, automação de processos internos e melhoria na experiência dos usuários em diferentes localidades. O uso de regiões, zonas de disponibilidade e pontos de presença garantem desempenho e resiliência a nível global, o que aumentará a eficiência e a produtividade da empresa.

**Assinatura do Responsável pelo Projeto:**  
Gabriel Ferreira Franco
