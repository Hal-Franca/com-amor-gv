# Com Amor GV — Companhia e Cuidado

Site institucional de uma página para serviço de companhia e cuidado em **Governador Valadares/MG**: acompanhamento de idosos, apoio a neurodivergentes e cuidado de pets de pequeno porte. Venda 100% pelo WhatsApp.

- **Status:** MVP em revisão (não divulgar o link até aprovação)
- **Hospedagem:** Netlify Drop, plano grátis (sem build, sem plugins)
- **Custo:** R$ 0

## Estrutura

```
com-amor-gv/
├── index.html          # site inteiro (HTML + CSS inline, sem dependências)
├── netlify.toml        # headers de segurança p/ Netlify
├── assets/
│   ├── img/
│   │   └── foto-perfil.png   # foto real da profissional
│   └── logo.svg              # logo (coração + Com Amor GV)
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

> Não commitar nem publicar arquivos de referência (`foto1-ref.jpeg`, `textos-para-canva-ref.txt` ficam fora desta pasta, em `Default Project/`).

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
