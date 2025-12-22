# NPS Web + Supabase

Projeto de coleta de NPS (Net Promoter Score) via interface web responsiva,
integrado ao Supabase para persistência e análise dos dados.

## 🧩 Tecnologias
- HTML5
- Tailwind CSS
- JavaScript (Fetch API)
- Supabase (PostgreSQL + RLS)
- GitHub

## 🚀 Funcionalidades
- Coleta de CPF/CNPJ
- Avaliação NPS (1 a 5)
- Envio via webhook
- Persistência no Supabase
- Estrutura preparada para dashboards e BI

## 📊 Modelo de Dados
Tabela principal: `nps_web`

Campos:
- `documento_cpf` (text, NOT NULL)
- `nota_nps` (smallint, 1–5)
- `hora_avaliacao` (timestamptz)

## 🔐 Segurança
- Row Level Security (RLS) habilitado
- Policy permitindo apenas INSERT anônimo
- Sem exposição de leitura pública

## 📦 Deploy
Pode ser hospedado em:
- GitHub Pages
- VPS / Nginx
- CDN estático

## 🧠 Observações
Projeto estruturado para fácil evolução:
- Dashboard de NPS
- Alertas automáticos
- Integração com BI
