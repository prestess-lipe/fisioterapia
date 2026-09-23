# FisioVida — Frontend Next.js

Migração do protótipo original em HTML/CSS/JavaScript puro para Next.js + React + TypeScript.

## O que foi preservado

- Mesma identidade visual, cores, tipografia, espaçamentos e componentes do HTML original.
- Login e retorno ao login.
- Mostrar/ocultar senha.
- Navegação entre Dashboard, Agenda, Pacientes, paciente, Consultas, Tipos de consulta, Horários, Clínica e Configurações.
- Menu lateral responsivo.
- Abas de configurações.
- Switches de preferências.
- Conteúdo e dados demonstrativos existentes no protótipo.

## Arquitetura preparada para o backend

O frontend está separado do backend e já possui `lib/api.ts` para consumir a API Java/Spring Boot através de `NEXT_PUBLIC_API_URL`.

Fluxo planejado:

Next.js / React / TypeScript
→ API REST
→ Java 21 + Spring Boot
→ PostgreSQL / Supabase

## Rodar

```bash
npm install
npm run dev
```

Depois abra `http://localhost:3000`.

## Observação

O backend Java ainda não foi conectado porque ele não faz parte do arquivo HTML enviado. Portanto, esta versão mantém as funcionalidades que já existiam no protótipo e deixa a integração REST preparada sem inventar endpoints.
