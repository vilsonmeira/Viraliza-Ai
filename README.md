# Viraliza AI — Vilson Vibes

Aplicativo pessoal para criação de conteúdo com IA.

## Recursos do MVP
- Gerador de conteúdo para Instagram Reels, TikTok, Kwai e Feed.
- Roteiro, gancho, legenda, hashtags, CTA e ideias extras.
- Geração de imagens pela API da OpenAI.
- Biblioteca local de rascunhos no navegador.
- Estrutura de conexão OAuth com Instagram profissional.

## Configuração na Vercel
Variáveis necessárias:
- OPENAI_API_KEY
- META_APP_ID
- META_APP_SECRET
- META_REDIRECT_URI

O callback deve ser exatamente `https://SEU-DOMINIO/api/instagram/callback`.

## Segurança
As chaves ficam somente no servidor. Tokens do Instagram são guardados em cookie HttpOnly, Secure e criptografado com AES-256-GCM. Não publique segredos no GitHub.

## Desenvolvimento
Aplicação estática na raiz e funções serverless em `api/`.