# Sistema do Angelo — regras de design

Cópia do Design System do Angelo. A fonte da verdade é o Design System no Claude; se algo mudar lá, copie esta pasta de novo.

Este site usa o **modo Editorial**.

Padrão para sites, landing pages e interfaces pessoais e de portfólio.

Projetos de clientes podem ter sistema próprio; quando houver, ele vence este.

## Princípios

- Tipografia é a estrutura: hierarquia vem de tamanho, peso e espaço — não de caixas, ícones ou cor.
- Uma ideia por seção. Muito espaço vazio; seções com no mínimo 96px (desktop) / 64px (mobile).
- Layouts com grid claro e assimetria intencional; evitar tudo centralizado.
- Um único acento de cor por tela. O resto é neutro.
- Detalhe > decoração: alinhamento preciso, hover pensado, microinterações sutis.
- Conteúdo específico e real. Nada de "Unlock the power of…" ou copy genérica.

## Evitar (o visual padrão de IA)

- Gradientes roxo→azul, texto com gradiente, blobs e glows de fundo
- Hero centralizado com badge pílula "✨ Novo" + dois botões lado a lado
- Grade de 3 cards iguais com ícone em quadrado arredondado
- Glassmorphism, emoji como ícone, sombras difusas grandes em tudo
- Inter/Poppins como única fonte; border-radius alto em tudo
- Depoimentos, números e logos de clientes inventados

## Usando tokens

- Fundo: neutros-bg em áreas grandes; neutros-surface para cards e camadas elevadas; neutros-border para bordas de 1px.
- Texto: neutros-text para o principal, neutros-muted para o secundário; neutros-subtle só para placeholder e desabilitado.
- Acento: azul (acento-base), único, reservado para links, foco e o CTA principal. Texto sobre ele sempre em acento-on.
- Estados (estados-success, estados-error, estados-warning) só para feedback do sistema, sempre com ícone ou texto.
- Tipografia: dois sets. "editorial" (Gloock + Geist + Geist Mono) e "tecnico" (Archivo + JetBrains Mono). Nunca misturar os dois na mesma interface. Usar sempre os estilos definidos, sem inventar tamanhos fora da escala.
- Espaçamento: só valores da escala space-1 a space-10, nada de números soltos. Seções em space-9 (desktop) e space-8 (mobile).
- Raio pequeno (0–6px) por padrão.
- Profundidade vem de bordas de 1px e contraste entre superfícies; sombra só quando necessária.

## Usando componentes

- Um único botão primário por tela; rótulos diretos, sem ícone decorativo.
- Links sempre identificáveis sem depender só da cor (sublinhado ou estado claro).

## Acessibilidade

- Texto de corpo com contraste mínimo 4.5:1; texto grande, 3:1.
- Foco sempre visível: anel de 2px em acento-base, com offset.
- Nunca comunicar estado só por cor.
- Respeitar prefers-reduced-motion em toda animação.

## Referências

Capturas em Assets são a referência visual. Extrair delas grid, escala

tipográfica e ritmo de espaçamento — nunca copiar layout literal.

## Modos — escolher pelo tipo de projeto

Antes de desenhar, identificar o modo. Se não estiver claro, perguntar.

Valem em TODOS os modos: "Evitar", "Acessibilidade" e conteúdo real.

Os "Princípios" acima valem integralmente só no modo Editorial.

**Editorial** (padrão) — portfólio, landing page, projeto pessoal ou criativo

- Tema escuro com os tokens neutros, um acento azul.
- Tipografia: set "editorial". Tipografia como protagonista, muito espaço vazio.

**Produto** — dashboard, sistema, app de uso diário

- Tipografia: set "tecnico"; display só no logo ou título principal.
- Densidade acima de respiro: espaçamento compacto (até space-7 entre seções), tabelas e formulários em destaque.
- Números e valores em tecnico-data.
- Cores de estado sempre acompanhadas de ícone ou texto.
- Oferecer tema claro e escuro.

**Catálogo** — loja, vitrine, produtos

- Tipografia: set "tecnico", discreta.
- A foto é a protagonista: grid limpo, fundo neutro.
- Nome, preço e chamada para ação (ex.: WhatsApp) sempre visíveis.
- Tema claro por padrão.

**Cliente** — marca de outra pessoa

- A identidade do cliente vence esta estética: cores, fontes e tom vêm da marca dele.
- Mantêm-se só as regras universais.

**Identidade própria** — gadget, game, interface de hardware ou projeto com assinatura visual forte
- A assinatura do projeto (cor, brilho, materiais) fica; este sistema entra em tipografia, espaçamento, acessibilidade e consistência.
- "Evitar" vale só no que não for a assinatura.

## Neste site

- Fontes: Gloock (títulos), Geist (texto) e Geist Mono (rótulos), carregadas do Google Fonts no `<head>`.
- Classes de componente com prefixo `an-` vêm de `design-system/components.css`. Estilos só do site ficam em `assets/css/site.css`, sempre usando as variáveis de `tokens.css`.
- Hero: só o nome em destaque, sem frase gigante. Contato em lista de linhas (rede em mono, usuário sublinhado, seta ↗).
- Nada de barras de porcentagem, números de enfeite, texto digitando, cards de serviço ou blobs de fundo.

