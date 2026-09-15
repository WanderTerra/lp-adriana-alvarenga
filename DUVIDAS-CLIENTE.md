# Dúvidas para alinhar com a cliente (Dra. Adriana)

Perguntas em aberto que dependem de informação/decisão dela antes de fechar a página.

## 1. SEO / estratégia de tráfego

Confirmado: a trava do vídeo (conteúdo só libera depois de assistir/pular) **fica como está** — foi pedido explicitamente pela cliente.

Isso tem uma consequência técnica: como o Google não clica em "assistir", ele não vê quase nenhum texto da página hoje (só o masthead e o título/lead antes do vídeo — todo o resto, ~90% do conteúdo, só aparece via JS depois de interação). Isso é normal e aceitável para páginas de VSL (vídeo de vendas) que rodam só em tráfego pago (Meta Ads, Google Ads).

**Perguntar para a cliente:** além do tráfego pago, ela espera/quer que essa página apareça em buscas do Google (SEO orgânico)?

- Se **não** → tudo certo, não precisa mexer em mais nada além do que já foi feito (meta description, Open Graph).
- Se **sim** → existe uma forma de resolver sem tirar a trava visual (trocar "revelar por clique" por "revelar por timer automático" ao carregar a página), mas é um ajuste técnico adicional que precisa ser combinado, já que muda o comportamento de quando o conteúdo é liberado.

## 2. Domínio / publicação

Domínio definido: **suajornadacirurgica.com.br** (Hostinger). Já atualizado `canonical`, `og:url`, `og:image` e `twitter:image` no `<head>` apontando pra esse domínio.

Gerei uma imagem de preview (`preview.png`, 1200×630) com a logo e o selo "Acompanhamento médico completo · 8 semanas" — precisa subir junto com o `index.html` na raiz do site (veja instruções de publicação abaixo).

⚠️ **Pendência técnica:** o domínio ainda está como "Configuração pendente" no painel do Hostinger — falta apontar/conectar ele pra um plano de hospedagem antes de subir os arquivos.

## 3. Preço

Os valores usados na seção de oferta hoje foram mantidos do site original (De R$ 2.997 → 12x R$149 no cartão ou R$1.497 à vista), já que o MD de copy deixava o preço em aberto ("ENTRA O PREÇO"). **Confirmar se esses valores continuam corretos** ou se ela quer atualizar.

## 4. Materiais pendentes (já sabidos, só reforçando)

- Vídeo real (hoje é uma simulação)
- Fotos/prints/depoimentos de pacientes (seção 11 do MD)
- ~~Thumbnails das 8 aulas~~ — ✅ recebidas em 15/09 e já aplicadas nos cards (veja o item 8 sobre a divergência de títulos)

## 5. Consentimento das pacientes nos depoimentos (IMPORTANTE)

A cliente enviou uma pasta do Drive com conversas reais de WhatsApp/Instagram entre pacientes e a Dra. Adriana. Usei frases curtas e positivas dessas conversas (agora três, incluindo o depoimento pedido em 15/09) na seção "O que dizem os pacientes", **sem nome, foto ou telefone** — atribuídas só como "Paciente".

Duas coisas que ainda precisam ser confirmadas com ela antes dessa seção ficar definitiva:

1. **Consentimento** — as pacientes autorizaram explicitamente o uso dessas mensagens (mesmo anonimizadas) em material de marketing? Dado de saúde é "dado sensível" pela LGPD; o ideal é ter essa autorização documentada (nem que seja um "pode usar sim" por WhatsApp mesmo).
2. **Publicidade médica (CFM)** — o Código de Ética Médica e resoluções do CFM sobre publicidade restringem bastante o uso de depoimentos de pacientes em propaganda de médicos. Vale ela (ou o contador/assessoria jurídica dela) confirmar se esse formato de depoimento é permitido, mesmo anonimizado.

Importante: **não usei** o material de uma das pacientes (4 das 6 imagens enviadas) porque era uma conversa de acompanhamento clínico real (complicação pós-cirúrgica, fístula, curativos, remédios) — isso não é depoimento de marketing e é sensível demais pra aparecer no site de qualquer forma, mesmo anonimizado.

## 6. Seção "Mentora" — números de experiência (pendente)

Preenchi a seção "Quem está por trás da sua Jornada Cirúrgica" com dados reais e verificáveis (formação, CRM/RQE, atuação em Campo Grande/MS), buscados no site profissional dela.

**O que ainda falta:** o site de referência não publica números (anos de experiência, quantidade de pacientes acompanhados, quantidade de cirurgias realizadas). Removi os placeholders `+[X]` que existiam pra esses números — **se ela quiser esse tipo de estatística na página, preciso que me passe os números reais** (não posso estimar/inventar isso).

## 7. Novo depoimento — ✅ Resolvido

Pedido via WhatsApp (25/08): "Vamos acrescentar apenas mais um depoimento" na seção de Histórias/Depoimentos. Texto recebido em 15/09 ("Dra, eu amei ter você me dando total apoio e cuidado! Deus abençoe sua vida sempre.") e adicionado como terceiro card, atribuído como "Paciente" (mesmo padrão dos outros dois). Sujeito à mesma pendência de consentimento/CFM do item 5.

## 8. Botão de compra abaixo do vídeo — tempo de liberação (pendente)

Pedido via WhatsApp (15/09): adicionar um botão de compra logo abaixo do vídeo inicial, que aparece depois de um certo tempo de vídeo assistido — ✅ implementado.

Por enquanto ele aparece no mesmo instante em que o resto da página é liberado (18s dos 24s do vídeo simulado — `REVEAL_AT_SECONDS` no código). **A cliente vai definir depois em qual segundo exato do vídeo real esse botão deve aparecer** (pode ser diferente do momento de liberação do resto do conteúdo). Quando ela decidir, é só me passar o tempo em segundos que eu ajusto.

## 9. Capas das aulas x títulos dos cards — divergência (IMPORTANTE)

As 8 capas das aulas foram recebidas em 15/09 e aplicadas nos cards conforme a numeração enviada. **Mas o título escrito dentro de cada capa não bate com o título que está escrito no card ao lado:**

| Semana | Título na capa (imagem) | Título atual no card (texto) |
|---|---|---|
| 01 | Decodificando o Diagnóstico | Antes de tudo, preparar você |
| 02 | Organizando a sua Cirurgia | Preparar a mente |
| 03 | Preparando Você | Preparar quem estará ao seu lado |
| 04 | Preparando seu Retorno | O dia da cirurgia |
| 05 | Dia D — Sua cirurgia chegou! | A alta hospitalar |
| 06 | O Retorno | A recuperação |
| 07 | Resultado Chegou | Recuperando sua confiança |
| 08 | O Depois da Cirurgia | Uma nova forma de viver |

Os títulos atuais dos cards vieram do MD de copy original. As capas parecem refletir uma estrutura mais nova do curso. **Não alterei os textos por conta própria** — preciso que a cliente confirme qual versão vale:

1. As capas estão certas → atualizo os títulos e os textos dos 8 cards pra acompanhar (nesse caso preciso do texto descritivo de cada aula nova); ou
2. Os textos estão certos → as capas precisam ser refeitas com os títulos corretos; ou
3. As capas estão na ordem errada → me diga a ordem certa que eu reposiciono.
