# Landing Page · Hora Zero Ready

Brief de estrutura, copy e UX da landing page do produto SaaS **Hora Zero Ready**, derivado do sales deck (`deck-comercial-vendas/hora-zero-ready-vendas-pt-br.pptx`). Este documento é referência única para devs, copywriters e revisores.

- **URL prevista:** `https://ready.horazero.com.br/` (ou `horazero.com.br/ready`)
- **Idioma primário:** PT-BR · variante EN sob `?lang=en` ou rota `/en`
- **Objetivo de conversão:** agendar diagnóstico gratuito de 30 min com Líder de Crise (NÃO contratação direta — fluxo mais consultivo, alinhado ao deck de vendas)
- **Objetivo secundário:** download do deck comercial PDF
- **Stack-alvo:** HTML estático single-page · CSS inline · sem framework · IBM Plex via Google Fonts CDN

---

## Identidade visual

Paleta e tipografia herdadas da unidade Hora Zero | Cyber Recovery.

- **Cores principais:** navy `#050B1F` · cyan `#00D4FF` · azul `#1E6FFF` / `#0A4FCC` · verde `#00B870` · vermelho crítico `#FF3B5C` · âmbar `#FFB020`
- **Fontes:** IBM Plex Sans Condensed (display) · IBM Plex Sans (body) · IBM Plex Mono (timestamps, preços, refs)
- **Lockup:** `Hora Zero | Cyber Recovery` + badge `READY`
- **Imagens:** logo (`logo-on-dark.png`), ícone-cronômetro (`icon.png`)

---

## Estrutura da página · 12 seções

| # | Seção | Ancora | Origem no deck |
|---|---|---|---|
| 1 | Nav fixa | — | — |
| 2 | Hero | `#hero` | slide 1 (capa) |
| 3 | A realidade brasileira | `#realidade` | slides 2-3 |
| 4 | Os 5 furos da primeira hora | `#furos` | slide 4 |
| 5 | A solução · 4 pilares | `#solucao` | slides 5-6 |
| 6 | Os 5 módulos | `#modulos` | slide 7 |
| 7 | Régua de prontidão · 12 meses | `#como-funciona` | slide 8 |
| 8 | 7 diferenciais | `#diferenciais` | slides 9-10 |
| 9 | Investimento · 3 tiers | `#pricing` | slides 11-12 |
| 10 | ROI · 24 meses | `#roi` | slide 13 |
| 11 | Pacotes de incidente com desconto | `#descontos` | slide 14 |
| 12 | Add-on opcional · Cloud ADD IT | `#cloud` | (extra) |
| 13 | FAQ | `#faq` | (extra) |
| 14 | Como começar · CTA principal | `#diagnostico` | slides 15-16 |
| 15 | Footer | — | — |

---

## 1. Nav fixa

Sticky com glassmorphism leve (`backdrop-filter: blur(12px)` sobre navy a 92%).

- **Logo:** Hora Zero on-dark à esquerda + badge cyan `READY`
- **Links:** Módulos · Como funciona · Tiers · ROI · FAQ
- **CTA:** botão cyan `AGENDAR DIAGNÓSTICO →` que rola até `#diagnostico`

---

## 2. Hero · `#hero`

Bg navy com radial gradients sutis (cyan top-right + azul bottom-left). Barra cyan vertical à esquerda (6px).

**Eyebrow** (chip cyan outlined)
```
NOVO · CYBER RECOVERY AS A SERVICE
```

**H1** (IBM Plex Sans Cond Bold, 4-5rem, branco)
```
Pronto antes do incidente.
```
(palavra "antes" pode receber acento cyan, opcional)

**Subhead** (Plex Sans italic, gray-300, 1.2rem)
```
Mensalidade fixa para chegar à hora zero pronto — fast-track e desconto quando ela vier.
```

**CTAs**
- Primário (cyan, navy text): `AGENDAR DIAGNÓSTICO GRATUITO →`
- Secundário (outline cyan): `Ver planos`

**Hero stats** (4 mini-tiles, divisor superior, max-width 540px)
- `≤ 2 min` — Atendimento priority na Linha Hora Zero
- `−30%` — Desconto em pacotes de incidente para assinantes
- `12/12` — Meses de prontidão contínua, não snapshot
- `T+4h` — Mobilização do war-room após acionamento

**Card lateral à direita** (navy-mid com strip cyan superior) — preview dos 3 tiers
```
3 tiers · transparente
Essential     R$ 18.000 /mês
Advanced      R$ 55.000 /mês
Enterprise    R$ 75.000 /mês

Sem multa de saída após 12 meses · faturamento mensal · NF-e regular · sem letras miúdas.
```

---

## 3. A realidade brasileira · `#realidade`

Bg navy com barra vermelha à esquerda. Tipografia centrada.

**Section eyebrow** (vermelho/cinza, mono)
```
A REALIDADE DO INCIDENTE SEM PREPARAÇÃO
```

**Big stat** (Plex Cond Bold, 14rem, vermelho crítico)
```
76%
```

**H2** (branco, max-width 800px, centralizado)
```
das organizações brasileiras tiveram pelo menos um incidente de ransomware nos últimos 24 meses.
```

**Foot** (gray-300, italic, max 720px)
```
Tempo médio de parada operacional: 21 dias. Custo médio: R$ 9,8 milhões. Perda média de receita: 14% do trimestre.
Fontes abertas, mediana de estudos 2023-2025.
```

---

## 4. Os 5 furos da primeira hora · `#furos`

Bg branco. Lista numerada com badges navy + texto factual.

**Section eyebrow:** `POR QUE A MAIORIA FALHA`

**H2:** `Os 5 furos que aparecem na primeira hora`

**Section lead:** *Padrões que observamos repetidamente em incidentes maduros.*

**Items** (badge 01 a 05 + título + descrição)

1. **Sem comando único** — TI, jurídico e RI tomam decisões em paralelo · confusão amplia o dano.
2. **Backup descoberto na hora** — Empresa descobre no RTO que backup foi comprometido junto, ou que restore leva 14 dias.
3. **Templates sem aprovação** — Comunicado interno e regulatório passam 4-12h em comitê de aprovação.
4. **C-level despreparado** — Decisões críticas sob pressão sem ter sido praticadas em tabletop.
5. **Volta para o mesmo lugar** — Recuperação devolve a empresa à infraestrutura comprometida · reincidência em 60-90 dias.

---

## 5. A solução · 4 pilares · `#solucao`

Bg branco. Grid 2×2 de cards com strip colorida superior.

**Section eyebrow:** `A SOLUÇÃO`

**H2:** `Hora Zero Ready · quatro pilares, uma mensalidade`

**Section lead:** *O que sua empresa recebe todos os meses, com ou sem incidente.*

**Pilares**

| Card | Strip | Título | Texto |
|---|---|---|---|
| 1 | cyan | **PRONTIDÃO TÉCNICA** | Mapa de infra vivo · backups testados · runbooks atualizados · plano de hardening tracking. |
| 2 | azul deep | **PRONTIDÃO HUMANA** | C-level treinado em tabletop · TI treinada em runbooks · comunicação aprovada antes de precisar. |
| 3 | verde deep | **RESPOSTA PRIORITY** | Atendimento ≤ 2 min · Líder de Crise nomeado · F0 começa pronto · −15% a −30% em pacotes. |
| 4 | âmbar | **PROVA AUDITÁVEL** | Selo fit-for-recovery por sistema · evidência mensal · prêmio menor de seguro cyber. |

---

## 6. Os 5 módulos · `#modulos`

Bg branco. Grid responsivo (auto-fit, min 280px). Cards com numerador navy + freq badge + título Plex Cond + descrição.

**Section eyebrow:** `OS 5 MÓDULOS`

**H2:** `Como a prontidão é construída · mês a mês`

**Section lead:** *Cada módulo entrega valor isolado · juntos viram uma régua completa.*

| # | Módulo | Freq | Descrição |
|---|---|---|---|
| 01 | **Asset Pulse** | Mensal | Mapa de Infra e Matriz de Criticidade P0-P3 vivos · scans mensais leves · dashboard de drift. |
| 02 | **Backup Assurance** | Mensal | Testes mensais de restore com evidência auditável · cadeia 3-2-1 reforçada · selo fit-for-recovery por sistema. |
| 03 | **Comms Library** | Trimestral | Templates de comunicação interna, externa, RI e ANPD pré-aprovados pela diretoria · prontos para acionar. |
| 04 | **Drill & Runbook** | Trim/Sem | Runbooks vivos · tabletop semestral com C-level · tracking do Plano de Hardening. |
| 05 | **Linha Priority + Credit** | Sempre on | Atendimento humano ≤ 2 min · Líder de Crise nomeado · desconto de até 30% em pacotes de incidente. |

---

## 7. Régua de prontidão · 12 meses · `#como-funciona`

Bg gray-100. Timeline horizontal com 5 pontos (com responsive para vertical no mobile).

**Section eyebrow:** `COMO O CLIENTE FICA PRONTO`

**H2:** `Sua empresa em outro patamar em 12 meses`

**Section lead:** *Cada mês traz uma evidência concreta de prontidão a mais.*

| Marco | Entregável |
|---|---|
| **Mês 1-2** | Onboarding · primeiro Asset Pulse · backup baseline · Comms Library v1. |
| **Mês 3** | Primeiro tabletop · runbooks v1 · Plano de Hardening priorizado. |
| **Mês 6** | Selo fit-for-recovery em 80% dos P0 · seguro cyber renegociável. |
| **Mês 9** | DR drill parcial · MTTD/MTTR medidos · hardening ajustado. |
| **Mês 12** | Empresa em outro patamar · prontidão medida · renovação anual. |

---

## 8. 7 diferenciais · `#diferenciais`

Bg branco. Grid 2 colunas × 4 linhas (última só com 1 item). Numeração cyan grande à esquerda.

**Section eyebrow:** `DIFERENCIAIS`

**H2:** `Por que Hora Zero`

**Section lead:** *Não é módulo lateral de uma consultoria. Não é seguro financeiro. É a única unidade brasileira dedicada 100% à hora mais cara da história da sua empresa.*

| # | Diferencial | Descrição |
|---|---|---|
| 01 | **Foco único** | 100% do nosso negócio é cyber recovery — não é módulo lateral. |
| 02 | **Linha 24/7 humana** | Atendimento humano em ≤ 5 min · ≤ 2 min para assinantes. |
| 03 | **Mobilização T+4h** | Líder de Crise sênior + war-room em até 4h após assinatura. |
| 04 | **Pacotes claros** | Comando fixo · Recuperação T&M transparente · Migração modular. |
| 05 | **Comunicação tripla** | Interna, externa (RI/mercado) e regulatória (LGPD/ANPD) integradas. |
| 06 | **Cloud no fim do trajeto** | ADD IT como parceira preferencial declarada · cyber integrada por design. |
| 07 | **Hand-off documentado** | Cliente fica com runbook completo · independência total em T+90d. |

---

## 9. Investimento · 3 tiers · `#pricing`

Bg branco. 3 cards lado-a-lado. Tier do meio (Advanced) destacado como "Mais escolhido" (badge cyan acima).

**Section eyebrow:** `INVESTIMENTO`

**H2:** `Três planos, transparência total`

**Section lead:** *Cliente escolhe pelo porte. Pricing em MRR fixo. Sem cláusulas escondidas. Saída sem multa após 12 meses.*

### Essential
- Porte: Até R$ 500M de faturamento
- Preço: **R$ 18.000 /mês** · R$ 216k/ano
- Inclui: Asset Pulse mensal · Backup Assurance mensal · Comms Library trimestral · Linha Priority ≤ 2 min · −15% em pacotes
- CTA: `Escolher Essential` (outline)

### Advanced **★ Mais escolhido**
- Porte: R$ 500M – R$ 3 Bi de faturamento
- Preço: **R$ 55.000 /mês** · R$ 660k/ano
- Inclui: Tudo de Essential · Drill & Runbook semestral · Tabletop com C-level · 40h consultoria pré-paga/ano · −25% em pacotes
- CTA: `Escolher Advanced` (cyan primary)

### Enterprise
- Porte: R$ 3 Bi – R$ 15 Bi de faturamento
- Preço: **R$ 75.000 /mês** · R$ 900k/ano
- Inclui: Tudo de Advanced · Líder de Crise nomeado · Drill & Runbook trimestral · DR drill anual completo · −30% em pacotes
- CTA: `Escolher Enterprise` (outline)

**Pricing foot** (gray-500, italic, centralizado)
```
Faturamento > R$ 15 Bi? Fale com a gente para um plano customizado.
```

---

## 10. ROI · 24 meses · `#roi`

Bg gray-100. Tabela centrada com cabeçalho navy, linhas alternadas, linha total navy com cyan.

**Section eyebrow:** `ROI · 24 MESES`

**H2:** `Sua empresa gasta menos · com mensalidade fixa`

**Section lead:** *Custo esperado em 24 meses para cliente porte G · probabilidade 60% de incidente material (mediana de estudos públicos 2023-2025).*

| Item | Sem Ready | Com Ready (Advanced) | Δ |
|---|---|---|---|
| Mensalidade SaaS (24m) | R$ 0 | R$ 1.320.000 | +R$ 1,32M |
| Custo esperado de incidente | R$ 2.100.000 | R$ 1.500.000 | −R$ 600k |
| Custo de parada operacional | R$ 4.000.000 | R$ 1.500.000 | −R$ 2,5M |
| **TOTAL ESPERADO 24 MESES** | **R$ 6.100.000** | **R$ 4.320.000** | **−R$ 1,78M · −29%** |

**Foot**
```
Bônus não contabilizados: prêmio menor de seguro cyber · C-level treinado · redução de churn em B2B (clientes do cliente percebem prontidão) · selo de prontidão para auditoria e compliance.
```

---

## 11. Pacotes de incidente com desconto · `#descontos`

Bg branco. Tabela 5 colunas mostrando pacotes Hora Zero originais + desconto por tier.

**Section eyebrow:** `QUANDO O INCIDENTE REAL VIER`

**H2:** `Você paga menos`

**Section lead:** *Pacotes Comando, Recuperação e Migração continuam disponíveis · com desconto contratual e fast-track operacional para assinantes.*

| Item | Não-assinante | Essential −15% | Advanced −25% | Enterprise −30% |
|---|---|---|---|---|
| Engagement fee (V-01) | R$ 50k | R$ 42,5k | R$ 37,5k | R$ 35k |
| Comando F1 · porte M | R$ 280-450k | R$ 238-383k | R$ 210-338k | R$ 196-315k |
| Comando F1 · porte G | R$ 450-780k | R$ 383-663k | R$ 338-585k | R$ 315-546k |
| Recuperação F2 · rate Pleno | R$ 580/h | R$ 493/h | R$ 435/h | R$ 406/h |
| Líder de Crise | R$ 2.000/h | R$ 1.700/h | R$ 1.500/h | R$ 1.400/h |

**Foot**
```
Fast-track operacional incluso: Líder de Crise já conhece seu ambiente · mapa atual · templates de comunicação prontos · backups recentemente testados. Resultado: F0+F1 mais rápido e menor consumo de horas em F2 — economia direta no pacote de Recuperação.
```

---

## 12. Add-on Cloud ADD IT · `#cloud`

Bg navy com radial verde sutil. Layout 2 colunas — lista + callout.

**Section eyebrow:** `ADD-ON OPCIONAL` (verde)

**H2:** `Migração para Cloud ADD IT`

**Section lead:** *Mesmo sem incidente, assinante Hora Zero Ready pode migrar para a nuvem privada ADD IT com pricing especial e cibersegurança integrada por design.*

**Lista (com + verde)**
- Migração estruturada sem precisar esperar um incidente para destravá-la.
- Cibersegurança integrada por design no ambiente novo — não bolt-on.
- Pricing especial para assinantes Hora Zero Ready.
- Hora Zero coordena · ADD IT entrega a infraestrutura.
- A subscription Hora Zero Ready continua entregando os 5 módulos no ambiente novo.

**Callout** (navy-mid com borda cyan à esquerda)
```
SEM LOCK-IN
Cliente pode optar por outra cloud ou modelo híbrido. A preferência declarada pela ADD IT é honestidade comercial baseada em integração técnica — não imposição. A Hora Zero coordena de qualquer modo.
```

---

## 13. FAQ · `#faq`

Bg branco. Accordions com `<details>` nativo, marker custom (`+` cyan).

**Section eyebrow:** `PERGUNTAS FREQUENTES`

**H2:** `O que costuma vir antes da decisão`

### Perguntas + respostas (8 entradas)

**1. Hora Zero Ready substitui o pacote de incidente?**
Não. Os pacotes Comando (V-03), Recuperação (V-04) e Migração (V-05) continuam sendo contratados quando o incidente real acontece — com desconto contratual de 15% a 30% para assinantes do Ready, e com fast-track operacional (Líder de Crise já conhece o ambiente).

**2. E se a empresa nunca tiver um incidente?**
A assinatura paga por si mesma com Asset Pulse (CMDB vivo), Backup Assurance (selo fit-for-recovery útil para seguro cyber), Comms Library (templates aprovados) e drills periódicos. O incidente é um possível evento, não a única razão para ter o plano. Bom argumento adicional: prêmio de seguro cyber tipicamente cai com evidências auditáveis.

**3. Como funciona o onboarding?**
O onboarding dura 4-6 semanas. Semana 1: kick-off + acesso aos sistemas. Semanas 2-3: primeiro Asset Pulse + análise de backups baseline. Semana 4: Comms Library v1 customizada à voz e regulatório do cliente. A partir do mês 2, ciclo mensal/trimestral roda normalmente.

**4. Existe contrato de fidelidade?**
Mínimo de 12 meses (necessário para o ciclo completo dos 5 módulos fazer sentido). Após o 12º mês, qualquer parte pode encerrar com 60 dias de aviso prévio, sem multa. Não há renovação automática vinculante.

**5. O cliente pode migrar entre tiers?**
Sim — upgrade a qualquer momento (a diferença é cobrada pro-rata). Downgrade ao final do ciclo mensal, com aviso prévio de 30 dias. Tier escolhido é sugerido pelo porte declarado, mas o cliente decide.

**6. Como o pricing dos pacotes de incidente é descontado?**
Descontos contratuais aplicados na ordem: −15% para Essential, −25% para Advanced, −30% para Enterprise. Aplicáveis sobre engagement fee, Pacote Comando (fixo), Pacote Recuperação (rates do time blendado) e Pacote Migração. Pacotes em si seguem regras do MSA V-06.

**7. Cobertura geográfica?**
Todo o Brasil. Linha Priority 24/7/365. War-room virtual ≤ 4h após acionamento. Presencial em ≤ 48h quando aplicável, em qualquer capital ou cidade com aeroporto comercial.

**8. E a LGPD durante o serviço SaaS?**
Hora Zero Ready é Operador de dados estritamente para finalidades técnicas (Asset Pulse, Backup Assurance). Contrato traz DPA padrão ANPD. O cliente continua sendo o Controlador. Nenhum dado pessoal sai do território brasileiro.

---

## 14. Como começar · CTA principal · `#diagnostico`

Bg navy. Eyebrow cyan, H2 branco, 5 passos em cards verticais, form de agendamento embaixo.

**Section eyebrow:** `AGENDE O DIAGNÓSTICO GRATUITO`

**H2:** `30 minutos com nosso Líder de Crise`

**Section lead:** *Sem compromisso. Você sai com diagnóstico inicial em mãos.*

### 5 passos · roadmap de decisão

| Passo | Quando | Entrega |
|---|---|---|
| 01 | **Hoje** | Conversa de 30 min com nosso Líder de Crise · alinhamento de porte e necessidade. |
| 02 | **Em 1 dia útil** | Proposta com tier sugerido, MRR, cronograma de onboarding e SLA específico. |
| 03 | **Em 5 dias úteis** | Contrato assinado digitalmente · primeiro pagamento autorizado. |
| 04 | **Em 7 dias** | Kick-off de onboarding · acesso aos sistemas · cronograma de 4 semanas. |
| 05 | **Em 30 dias** | Primeiro entregável: Asset Pulse + Backup Assurance + Comms Library v1. |

### Form de agendamento

Inputs (todos required exceto observações):
- **Tier de interesse** (radio): Essential / Advanced / Enterprise / Não sei ainda
- **Razão social**
- **CNPJ**
- **Faturamento estimado anual** (select: até 100M / 100-500M / 500M-1Bi / 1Bi-3Bi / 3-15Bi / > 15Bi)
- **Setor** (select: indústria / varejo / financeiro / saúde / tech / energia / logística / agro / outro)
- **Responsável técnico** (nome + cargo)
- **E-mail técnico**
- **Responsável comercial** (nome + cargo)
- **E-mail comercial**
- **Observações** (opcional, textarea)

**Submit:** `AGENDAR DIAGNÓSTICO GRATUITO →` (cyan primary, navy text)

**Consent (gray-500, 12px):**
```
Ao enviar, você concorda com o uso dos dados acima exclusivamente para preparação da reunião de diagnóstico, conforme nossa Política de Privacidade LGPD. Nenhum dado é compartilhado com terceiros sem novo consentimento explícito.
```

**Backend stub** (a integrar):
- POST para CRM da ADD IT
- E-mail confirmação ao cliente
- Slack `#vendas-horazero`
- Tarefa no pipeline com SLA 1 dia útil

---

## 15. Footer

Bg navy, 4 colunas (responsivo 2×2 em mobile).

| Coluna | Conteúdo |
|---|---|
| **1 · Marca** | Logo + tagline: "Hora Zero Ready é um serviço da unidade Hora Zero \| Cyber Recovery, vinculada à ADD IT Cloud Solutions. Operação 100% brasileira · cobertura nacional." |
| **2 · Produto** | Módulos · Como funciona · Tiers · ROI · Cloud ADD IT |
| **3 · Contato** | ready@horazero.com.br · 0800-XXXXXXX (24/7) · Agendar diagnóstico |
| **4 · Legal** | Termos de Uso · Política de Privacidade · LGPD · DPA padrão ANPD · SLA público |

**Footer base** (linha inferior, mono, gray-500, 11px):
- `© 2026 Hora Zero | Cyber Recovery · ADD IT Cloud Solutions`
- `CONFIDENCIAL · documento de oferta sujeito a aprovação comercial · v1.0`

---

## Diretrizes de copy

- **Tom:** direto, factual, sem bravata. Sem jargão de marketing. Sem promessa de "tudo resolvido em 24h".
- **Voz:** Hora Zero fala em primeira pessoa para o cliente ("sua empresa", "você").
- **Linguagem técnica:** ok em CTA secundário e seções avançadas. Hero e CTAs primários devem ser legíveis por CEO/CFO.
- **Números:** sempre com unidade clara (R$, %, dias, min). Mediana > média quando disponível, com fonte.
- **Sem emoji.** Sem ícones genéricos de stock.
- **Português brasileiro padrão formal** com leveza pontual (ex.: "letra miúda" é aceitável; gírias não).

---

## SEO básico

- `<title>`: `Hora Zero Ready · Cyber recovery como serviço mensal`
- `<meta description>`: `Mensalidade fixa para chegar à hora zero pronto — fast-track e desconto quando ela vier. Hora Zero Ready, a partir de R$ 18.000/mês.`
- `<meta og:title>` e `<meta og:description>` espelhando
- `<link rel="icon">` apontando para `icon.png`
- `<html lang="pt-BR">`
- Cabeçalhos semânticos (H1 → H2 → H3 sem pular níveis)
- Imagens com `alt` descritivo
- `<meta theme-color content="#050B1F">` para mobile

## Performance e acessibilidade

- Critical CSS inline (sem requests externos exceto Google Fonts)
- Preconnect a fonts.gstatic.com
- Cores combinadas atendem WCAG AA (já validado na palette.md do projeto)
- Focus visible em todos os elementos interativos
- `scroll-behavior: smooth` para âncoras internas
- Form com labels associadas, placeholders descritivos
- Detalhes/sumários do FAQ funcionam sem JS (progressive enhancement)

---

## Eventos de tracking sugeridos (Google Analytics / GTM)

| Evento | Quando disparar |
|---|---|
| `cta_primary_click` | clique em qualquer CTA "Agendar diagnóstico" |
| `cta_pricing_select` | clique em "Escolher [Tier]" no pricing |
| `faq_open` | abertura de qualquer pergunta do FAQ |
| `scroll_50` / `scroll_80` | scroll milestones |
| `form_start` | primeiro foco em campo do form |
| `form_submit` | submissão do form de diagnóstico |
| `cloud_addon_view` | scroll até seção Cloud ADD IT |

---

## Próximos passos

1. ✅ MD aprovado · construir HTML inicial
2. ⬜ Revisar copy com time de vendas ADD IT (2-3 dias)
3. ⬜ Integrar form com CRM ADD IT (HubSpot/Salesforce)
4. ⬜ Setup analytics + GTM
5. ⬜ A/B test do hero (variante: "Pronto antes do incidente" vs "Cyber recovery como serviço mensal")
6. ⬜ Publicar em `ready.horazero.com.br`
