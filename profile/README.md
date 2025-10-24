# 🏢 Política de Acesso & Governança

## 🔑 Princípios
- **Tudo privado**: repositórios privados por padrão.
- **Conta corporativa**: use seu e-mail `@sperotto.com.br` no Git e no GitHub. 
- **2FA obrigatório**: autenticação de dois fatores em todas as contas.
- **Registro e trilha**: mudanças passam por PR e ficam auditáveis.

## 🔒 Segurança (obrigatório)
- ✅ Ative **2FA** na sua conta GitHub.
- ✅ **Nunca** faça commit de senhas/tokens. Use **Secrets** (GitHub) + `.env` local.
- ✅ Habilite *secret/dependency scanning* quando disponível.
- ✅ Chaves SSH com *passphrase*; revogue chaves antigas.
- ✅ Não altere visibilidade de repo sem aprovação do Owner.

## 🧩 Integração com Notion
- Repositório → README com link para **página do projeto** no Notion.  
- Notion → embed de PRs/issues e visão geral do roadmap.  
- Status de PR no Notion (propriedade “GitHub PR”) opcional.

## 📚 Documentação
- README do repo: setup rápido, como rodar, como testar, link do Notion.
- Detalhes extensos → Notion (arquitetura, decisões, ADRs).
- Mantenha exemplos atualizados (/examples, requests.http, swagger/openapi quando aplicável).

## 🧰 Ambiente do Git (pessoal corporativo)
- `git config --global user.name "Seu Nome"`
- `git config --global user.email "seu.nome@sperotto.com.br"`   # use e-mail corporativo

## ⚡ Guia Rápido (TL;DR)
1. **Crie uma branch**: `feature/…` ou `fix/…`  
2. **Commits pequenos** e descritivos  
3. **Abra uma PR** para `main`  
4. **Peça revisão** (code review)  
5. **Checks OK** → **Merge** (Squash)  
6. **Feche a issue** e atualize o Notion

## 🌳 Estratégia de Branches
- `main` → produção/estável (protegida)  
- `feature/<slug>` → novas funcionalidades  
- `fix/<slug>` → correções  
- `chore/<slug>` → ajustes não funcionais (lint, build, deps)

## 🔐 Segredos & Configuração
- Nunca commit `.env`, chaves, tokens.
- Use GitHub Secrets (Actions) e `.gitignore`.
- Rotacione segredos periodicamente.
