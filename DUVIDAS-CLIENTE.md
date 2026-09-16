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

## 9. Capas das aulas x títulos dos cards — ✅ Resolvido

Em 15/09 as capas chegaram com títulos que não batiam com o texto dos cards (os cards ainda usavam a estrutura do MD de copy original). Confirmado: **as capas estavam certas e os textos é que estavam desatualizados.**

Em 16/09 a cliente enviou a arte nova das 8 capas (versão em fundo oliva escuro) junto com o texto definitivo de cada semana. Tudo já aplicado: título, frase-gancho e descrição de cada aula agora acompanham a capa correspondente.

Estrutura final das 8 semanas: Decodificando o diagnóstico · Organizando sua cirurgia · Preparando você · Preparando seu retorno · Dia D · O retorno · Resultado chegou e agora? · Qual caminho seguir?
