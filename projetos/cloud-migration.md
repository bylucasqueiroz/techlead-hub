# Projeto: Cloud Migration AWS

## 📌 Visão Geral
Migração dos serviços internos on-premise para infraestrutura AWS. Envolve pipelines de CI/CD, segurança, IAM, redes, e modernização de containers.

- Status atual: Planejamento final
- Responsável: João Silva
- Time envolvido: Pedro, Carla, Bia

## 🎯 Objetivos da Sprint
- Validar arquitetura em ambiente de staging
- Finalizar Terraform de infraestrutura de VPC
- Configurar pipelines com CodePipeline e ECS

## ✅ TO-DO

- [ ] Finalizar revisão de arquitetura com segurança
- [ ] Criar runbook de fallback em caso de rollback
- [ ] Validar custo estimado da infraestrutura provisionada
- [ ] Documentar modelo de logs e métricas
- [x] Finalizar PoC de CodePipeline

## 📅 Marcos Importantes

| Data       | Entrega                              |
|------------|---------------------------------------|
| 2025-05-03 | Infraestrutura pronta em staging      |
| 2025-05-10 | Aplicações migradas (1ª leva)         |
| 2025-05-17 | Infraestrutura em produção            |

## 🧠 Anotações Técnicas
- Uso de EKS foi descartado inicialmente por custo e complexidade
- CodeBuild terá acesso IAM restrito com roles específicas
- Monitoramento será feito via CloudWatch + Grafana

## 🗣️ Decisões Tomadas
- Adotado padrão GitHub Actions para testes locais
- Log centralizado via CloudWatch + Firelens no Fargate
