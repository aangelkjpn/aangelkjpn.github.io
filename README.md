# Angelo Gabriel · Portfólio

Meu portfólio pessoal, publicado em **https://aangelkjpn.github.io**.

Reúne quem eu sou, os projetos que desenvolvi (Controle de TI, Chamada dos Notebooks, GameFinder e Meu Fluxo), minha trajetória no estágio PROATI, na Unoeste e no SENAI, a stack que uso e meus certificados.

## Como é feito

- **HTML e CSS** puros, sem build, sem framework e sem JavaScript
- **Meu próprio Design System**, no modo Editorial: tokens, componentes e regras ficam em [`design-system/`](./design-system/)
- Fontes **Gloock**, **Geist** e **Geist Mono**, carregadas do Google Fonts
- Publicado com o **GitHub Pages**

## Estrutura

```
├── index.html          # A página
├── design-system/      # Cópia do Design System (não editar aqui)
│   ├── DESIGN.md       # Regras de design
│   ├── tokens.css      # Cores, fontes, espaçamentos e raios
│   └── components.css  # Componentes com prefixo an-
├── assets/
│   ├── css/site.css    # Estilos só deste site, usando os tokens
│   └── img/            # Foto, ícones e imagens dos projetos
└── CLAUDE.md           # Instruções para o Claude ao mexer no site
```

Para ver localmente, é só abrir o `index.html` no navegador.
