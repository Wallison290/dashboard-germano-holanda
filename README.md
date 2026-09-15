# Dashboard Estratégico da Imobiliária Germano Holanda

Manual estratégico de posicionamento digital do perfil
[@imobiliariagermanoholanda](https://instagram.com/imobiliariagermanoholanda)
(imóveis de médio e alto padrão, João Pessoa e Cabedelo/PB, CRECI 640J).

Site estático de página única (`index.html`), sem dependências e sem build.

## Conteúdo

1. Resumo do plano
2. Como o perfil está hoje
3. O site no celular
4. O que mudar no perfil
5. Calendário editorial (12 publicações)
6. Números para acompanhar

## Decisões de construção

**Página 03 é sobre o site, não sobre concorrência.** A análise recebida não trazia
levantamento de perfis concorrentes, e inventar imobiliárias e números de seguidores seria
dado falso. O espaço foi ocupado pela análise da experiência mobile de `germanoholanda.com.br`,
que é o ponto onde a jornada do visitante se perde hoje.

**O dourado dos textos foi escurecido.** O dourado da marca (`#BA962C`) tem contraste de
2,8:1 sobre fundo branco e reprova nos critérios de acessibilidade. Textos, links e botões usam
`#8C6F17` (4,8:1, aprovado em AA). O dourado original segue aplicado nos elementos decorativos,
onde a leitura não depende dele.

**As cores de status são terracota, não âmbar.** O âmbar usado normalmente para "atenção"
desapareceria dentro do dourado da marca. As classes mantêm o nome `.amber`, mas os valores são
terracota (`#9A4B2E`).

**As fontes são aproximações.** DM Sans e Poppins foram escolhidas por legibilidade; não são as
fontes oficiais da marca.

## Limitações

Os números do perfil (11,1 mil seguidores, 6.185 publicações, 7 destaques) são a foto de um dia
e não têm histórico semanal organizado. A tabela da página 06 existe para construir essa linha
de base a partir do primeiro mês.

A análise do site é de observação visual da experiência no celular. Não inclui medição de
velocidade, teste em múltiplos aparelhos nem leitura do código.

As marcações de post e os números digitados ficam salvos apenas no navegador de quem acessa
(`localStorage`). Não são enviados a lugar nenhum e não aparecem em outro aparelho. Por isso a
página oferece o download da planilha.

## Publicação

Hospedado na Vercel como site estático. Qualquer push na branch `main` gera um novo deploy
automaticamente.

Para rodar localmente, basta abrir o `index.html` no navegador.
