---
title: "Velo — PIX Recorrente"
date: 2024-01-15T10:00:00-03:00
draft: false
language: pt-br
description: App mobile para cobranças recorrentes via PIX, focado em freelancers e profissionais autônomos
status: "MVP 75%"
status_color: "yellow"
tags: ["React Native", "Firebase", "Mercado Pago", "TypeScript", "PIX"]
---

## O Problema

Freelancers, MEIs e profissionais autônomos enfrentam um desafio recorrente — literalmente. Gerenciar cobranças mensais de clientes de forma manual é ineficiente, propenso a erros e consome tempo precioso que poderia ser usado para crescer o negócio.

Soluções tradicionais exigem maquininhas de cartão, contratos com bancos ou sistemas complexos de ERP. O **Velo** nasceu para resolver isso: uma ferramenta mobile simples e direta que automatiza cobranças recorrentes via PIX, o meio de pagamento mais popular do Brasil.

## Público-alvo

- Freelancers que cobram clientes recorrentes mensalmente
- MEIs e pequenos prestadores de serviço com contratos de manutenção/recorrência
- Profissionais autônomos (personal trainers, consultores, designers, desenvolvedores)
- Pequenos negócios que precisam de faturamento recorrente sem burocracia

## A Solução

O **Velo** é um aplicativo mobile para **cobranças recorrentes via PIX** que automatiza todo o ciclo de faturamento: do cadastro do cliente à cobrança, do acompanhamento ao recebimento. Com poucos toques na tela, o profissional configura a recorrência, valor e forma de cobrança, e o Velo cuida do resto — gera o QR Code PIX, envia a cobrança via WhatsApp, notifica o cliente e registra o pagamento.

## Funcionalidades em Detalhe

### Autenticação e Segurança
Login simplificado com email/senha ou Google Sign-In, com autenticação via Firebase. Dados protegidos e isolados por usuário.

### Gestão de Clientes
Cadastro completo de clientes com nome, telefone, email e valor do contrato. Busca em tempo real para localizar rapidamente qualquer cliente. Cada cliente pode ter múltiplos contratos e histórico de pagamentos.

### Cobranças Recorrentes
Configure a periodicidade da cobrança (semanal, mensal, personalizado). O sistema gera automaticamente a cobrança no vencimento, sem necessidade de ação manual. A cada ciclo, o QR Code PIX é gerado e enviado ao cliente.

### Geração de QR Code PIX
Integração direta com Mercado Pago e Efi Pagamentos para gerar QR Codes PIX dinâmicos. O cliente aponta a câmera, paga, e o sistema registra automaticamente.

### Dashboard Financeiro
Acompanhe métricas em tempo real: total faturado no mês, taxa de inadimplência, clientes ativos, histórico de pagamentos. Gráficos interativos com Victory Native mostram a evolução financeira.

### Notificações Inteligentes
Push notifications avisam o profissional quando um pagamento é recebido. O cliente recebe lembrete automático antes do vencimento.

### Integração com WhatsApp
Envio automático da cobrança via WhatsApp com QR Code PIX incluso. O cliente recebe a mensagem, paga, e pronto — sem precisar abrir outro app.

### Sistema Premium
7 dias grátis para testar todas as funcionalidades. Planos mensais e anuais com benefícios exclusivos.

## Roadmap

| Fase | Descrição | Status |
| ---- | --------- | ------ |
| **MVP Core** | Autenticação, CRUD de clientes, cobranças manuais, dashboard básico, notificações push, integração Mercado Pago | ✅ Completo |
| **Automação** | Webhooks Efi, cobranças automáticas recorrentes, monitoramento em tempo real, WhatsApp, sistema premium, dashboard admin | 🔄 Em andamento |
| **Expansão** | Emails transacionais, relatórios PDF, emissão de NFS-e, cartão de crédito, multilíngue, backups | 📅 Planejado |
| **Scale** | API pública, white-label, analytics avançado, multi-moeda, integração ERP, insights com IA | 📅 Futuro |

## KPIs de Referência

- **99%** de uptime garantido
- Resposta da API **<500ms**
- Notificações push entregues em **<5s**
- **50+** usuários ativos na base
- **20%** de conversão trial → plano premium
- **NPS >8**
- Churn mensal **<5%**
