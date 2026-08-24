# Dúvidas para alinhar com a cliente (Dra. Adriana)

Perguntas em aberto que dependem de informação/decisão dela antes de fechar a página.

## 1. SEO / estratégia de tráfego

Confirmado: a trava do vídeo (conteúdo só libera depois de assistir/pular) **fica como está** — foi pedido explicitamente pela cliente.

Isso tem uma consequência técnica: como o Google não clica em "assistir", ele não vê quase nenhum texto da página hoje (só o masthead e o título/lead antes do vídeo — todo o resto, ~90% do conteúdo, só aparece via JS depois de interação). Isso é normal e aceitável para páginas de VSL (vídeo de vendas) que rodam só em tráfego pago (Meta Ads, Google Ads).

**Perguntar para a cliente:** além do tráfego pago, ela espera/quer que essa página apareça em buscas do Google (SEO orgânico)?

- Se **não** → tudo certo, não precisa mexer em mais nada além do que já foi feito (meta description, Open Graph).
- Se **sim** → existe uma forma de resolver sem tirar a trava visual (trocar "revelar por clique" por "revelar por timer automático" ao carregar a página), mas é um ajuste técnico adicional que precisa ser combinado, já que muda o comportamento de quando o conteúdo é liberado.

## 2. Domínio / publicação

Para terminar o SEO básico da página falta:
- **Qual vai ser a URL final** (domínio) onde a página vai ficar publicada — necessário para preencher `canonical` e `og:url` no `<head>`.
- **Uma imagem de preview** (para `og:image`, o card que aparece quando o link é compartilhado no WhatsApp/Instagram/Facebook). Precisa ser um arquivo hospedado com URL pública — não dá pra usar a logo embutida em base64 que está no código hoje.

## 3. Garantia — ✅ Resolvido

Confirmado com a cliente: **7 dias**. Já atualizado no código (removido o placeholder `[X]` e o comentário `TODO`).

## 4. Preço

Os valores usados na seção de oferta hoje foram mantidos do site original (De R$ 2.997 → 12x R$149 no cartão ou R$1.497 à vista), já que o MD de copy deixava o preço em aberto ("ENTRA O PREÇO"). **Confirmar se esses valores continuam corretos** ou se ela quer atualizar.

## 5. Materiais pendentes (já sabidos, só reforçando)

- Vídeo real (hoje é uma simulação)
- Fotos/prints/depoimentos de pacientes (seção 11 do MD)
- Foto profissional da Dra. Adriana (seção "Quem será sua mentora") — ✅ já adicionada

## 6. Consentimento das pacientes nos depoimentos (IMPORTANTE)

A cliente enviou uma pasta do Drive com conversas reais de WhatsApp/Instagram entre pacientes e a Dra. Adriana. Usei apenas duas frases curtas e positivas dessas conversas na seção "O que dizem os pacientes", **sem nome, foto ou telefone** — atribuídas só como "Paciente".

Duas coisas que ainda precisam ser confirmadas com ela antes dessa seção ficar definitiva:

1. **Consentimento** — as pacientes autorizaram explicitamente o uso dessas mensagens (mesmo anonimizadas) em material de marketing? Dado de saúde é "dado sensível" pela LGPD; o ideal é ter essa autorização documentada (nem que seja um "pode usar sim" por WhatsApp mesmo).
2. **Publicidade médica (CFM)** — o Código de Ética Médica e resoluções do CFM sobre publicidade restringem bastante o uso de depoimentos de pacientes em propaganda de médicos. Vale ela (ou o contador/assessoria jurídica dela) confirmar se esse formato de depoimento é permitido, mesmo anonimizado.

Importante: **não usei** o material de uma das pacientes (4 das 6 imagens enviadas) porque era uma conversa de acompanhamento clínico real (complicação pós-cirúrgica, fístula, curativos, remédios) — isso não é depoimento de marketing e é sensível demais pra aparecer no site de qualquer forma, mesmo anonimizado.
