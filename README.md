# Com Amor GV — Companhia e Cuidado

Site institucional de uma página para serviço de companhia e cuidado em **Governador Valadares/MG**: acompanhamento de idosos, apoio a neurodivergentes e cuidado de pets de pequeno porte. Venda 100% pelo WhatsApp.

- **Status:** MVP em desenvolvimento
- **Hospedagem:** Netlify (plano grátis, sem build, sem plugins) — deploy via GitHub conectado
- **Custo:** R$ 0

## Estrutura

```
com-amor-gv/
├── index.html          # site inteiro (HTML + CSS inline, sem dependências)
├── netlify.toml        # headers de segurança p/ Netlify
├── assets/
│   ├── img/
│   │   ├── foto-perfil.png   # foto real da profissional (publicada)
│   │   └── foto1-ref.jpeg    # referência local — ignorada pelo git (.gitignore)
│   └── logo.svg              # logo (coração + Com Amor GV)
├── .gitignore          # bloqueia dados pessoais e referências
├── README.md
├── AGENTS.md           # instruções p/ agentes de IA
└── kanban.md           # o que foi feito e próximos passos
```

## Ver localmente

Duplo clique em `index.html` — abre no navegador, sem servidor.

## Publicar / atualizar (Netlify Drop)

1. Acesse `app.netlify.com/drop`
2. Arraste a pasta `com-amor-gv` inteira
3. Pronto: link `*.netlify.app` (renomeável em Site settings → Change site name)
4. Para atualizar: edite os arquivos, arraste a pasta de novo em Deploys

> Arquivos de referência e dados pessoais nunca vão para o git: o `.gitignore` bloqueia
> `*-ref.*`, pastas `ref/`, `dados-pessoais/`, `clientes/`, `documentos/` e PDFs. Ver seção Segurança.

## Segurança e dados pessoais (LGPD)

- **Nunca commitar:** fotos de clientes, documentos (CPF, RG, endereço), prints com dados pessoais, arquivos `*-ref.*`.
- **Onde guardar esse material:** fora do repo (ex: pasta `Default Project/`, só local) ou nas pastas bloqueadas acima.
- **Exceções intencionais e públicas:** foto da profissional (`foto-perfil.png`), WhatsApp comercial e cidade — são o conteúdo do site.
- Antes de cada `push`, rode `git status` e confira que só entram arquivos do site.

## Editar conteúdo

- Textos: direto no `index.html` (seções: topo, sobre, serviços, como funciona, valores, FAQ, contato)
- Foto: substituir `assets/img/foto-perfil.png` mantendo o nome
- WhatsApp: trocar o número `5533991717907` nos links `wa.me/...` (4 ocorrências)
- Cores: variáveis CSS em `:root` (`--vinho #8E2A4A`, `--rosa #FCECEF`, `--bege #FFF8F3`)

## Convenções

- Termo padrão: **"idosos"** (não "sênior" — melhor busca e identificação do público)
- Valores sempre como **"a combinar"** (varia por serviço, local, horas/dias)
- Atendimento masculino **somente com referência**
- Sem carro próprio: deixar explícito (a pé, ônibus/app ou carro da família)
- Bairros: confirmar disponibilidade no WhatsApp (decisão da profissional)

## Roadmap

Ver `kanban.md`.
