# AGENTS.md — Com Amor GV

Instruções para agentes de IA trabalhando neste repositório.

## Stack

- Site estático de 1 página: `index.html` com CSS inline. **Sem frameworks, sem build, sem dependências externas, sem backend.**
- Deploy: arrastar a pasta no Netlify Drop. `netlify.toml` só tem headers de segurança.
- Dono do repo edita tudo localmente; a profissional (mãe dele) não edita nada.

## Convenções de conteúdo (não quebrar)

- Nome: **Com Amor GV — Companhia e Cuidado**. Cidade: Governador Valadares/MG.
- Termo padrão: **"idosos"** (nunca trocar por "sênior" sem pedir).
- Preço: sempre **"valor a combinar"** — varia por serviço, local em GV, horas/dias.
- WhatsApp: `+55 33 99171-7907` → links `https://wa.me/5533991717907?...` (há 4 no HTML; ao trocar o número, trocar todos).
- Regras fixas: atendimento masculino somente com referência; sem carro próprio (a pé, ônibus/app ou carro da família); bairros confirmados no WhatsApp; medicação só com orientação da família/profissional; sem procedimentos invasivos de enfermagem.
- Tom: acolhedor, simples, direto. Público: familiares (filhos) de idosos.

## Convenções técnicas

- Manter tudo em `index.html` (não criar arquivos CSS/JS separados sem pedir).
- Imagens em `assets/img/` com caminho relativo. Foto de perfil: `assets/img/foto-perfil.png`.
- Paleta: vinho `#8E2A4A`, vinho escuro `#6E1F39`, rosa `#FCECEF`, bege `#FFF8F3`, texto `#4A3540`, verde zap `#25D366`.
- Mobile-first: testar em 360px de largura. Não adicionar fontes externas (performance no 4G).
- Nunca commitar fotos de clientes, dados pessoais ou arquivos `*-ref.*` — o `.gitignore` já bloqueia esses padrões; se um novo tipo de dado pessoal surgir, adicionar o padrão ao `.gitignore` antes de commitar.

## Antes de finalizar qualquer mudança

1. Conferir os 4 links `wa.me` funcionando.
2. Conferir `src` das imagens (case-sensitive no deploy Linux).
3. Abrir o HTML e checar visual mobile + desktop.
