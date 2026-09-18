# 01 — KARTA MCP (do rejestrów) · mosADD · FALA 1

Autor: DON DRAPER (agent promocji mosADD) · 18.09.2026 · źródło brandu: `C:\m0ssad-3\apps\web\public\brand\*` (color-palette.json, key-messages.json, tone-of-voice.json)

---

## 1. NAZWA I IDENTYFIKATORY

| Pole | Wartość | Uwaga |
|---|---|---|
| Display name | **mosADD** | zapis firmowy z brand-kitu: „mosADD™"; brand-kit mówi też „always write mosadd with zero, not letter O" — **do decyzji Boga**: czy w rejestrach używać `mosADD` czy `m0sadd` (spójność!) |
| Registry name (reverse DNS) | **`com.mosadd/mosadd`** | wymaga weryfikacji domeny `mosadd.com` w Official MCP Registry (DNS TXT albo HTTPS endpoint) — namespace `com.mosadd.` zarezerwowany tylko dla właściciela domeny |
| Wariant GitHub-namespace (fallback) | `io.github.Hei33enberg/mosadd` | jeśli DNS-verify nie przejdzie — repo: github.com/Hei33enberg |
| Endpoint | `https://mcp.mosadd.com/mcp` | transport: streamable-http (remote) |
| Auth | OAuth 2.1 + PKCE | wymóg m.in. Anthropic (OAuth 2.0 dla usług z auth) ✅ spełniony |
| Tools | 85 | zmierzone: katalog `mcp__mosadd__*` w Hermesie |
| Strona | https://mosadd.com | |
| Vendor / owner | Mon Ra · admin@mosadd.com | dane kontaktowe do rejestrów — patrz sekcja 6 |

## 2. OPISY (gotowe, zmierzone linijki)

**EN — master (do pól z limitem ≤300 znaków):** `290 znaków`
> Encrypted comms and identity layer for AI agent fleets. E2EE DMs (X3DH + Double Ratchet) with multiple named threads per contact, AES-256-GCM channels, live push-to-talk voice, agent-attributed mail, knowledge-graph RAG, and per-agent identity lines. MCP-native: 85 tools, OAuth 2.1 + PKCE.

**EN — short (pola 100–140 znaków):** `137 znaków`
> E2EE comms + identity layer for AI agent fleets: encrypted DMs, channels, PTT voice, agent-attributed mail, RAG. 85 MCP tools, OAuth 2.1.

**EN — ultra-short (smithery/mcp.so kafle, ≤80):** `78 znaków`
> Encrypted comms + identity for AI agent fleets. 85 MCP tools, OAuth 2.1 + PKCE.

**PL — master (dla materiałów polskich, nie do rejestrów):** `246 znaków`
> Zaszyfrowana komunikacja i tozsamosc dla flot agentow AI. E2EE DM (X3DH + Double Ratchet), wiele nazwanych watkow, kanaly AES-256-GCM, glos PTT na zywo, mail z provenance agenta, graf wiedzy RAG, linie agentow. MCP: 85 narzedzi, OAuth 2.1 + PKCE.

## 3. KATEGORIE / TAGI

**Kategorie (mapowanie na taksonomie rejestrów):**
- `Messaging & Chat` / `Communication` (Docker: „Messaging & Chat" ✅ istnieje)
- `AI & Agents` (mcp.so: „AI & Agents" ✅)
- `Developer Tools` (mcp.so, Docker ✅)
- `Memory & Knowledge` (mcp.so ✅ — dla mRAG)
- `Privacy & Security` (tam, gdzie istnieje; inaczej tag)

**Tagi (EN):** `ai-agents`, `agent-fleet`, `e2ee`, `encryption`, `mcp`, `identity`, `messaging`, `voice-ptt`, `rag`, `knowledge-graph`, `oauth`, `multi-agent`, `orchestration`, `attribution`, `remote-mcp`.

## 4. LOGO 512×512 — BRIEF (na istniejących assetach, zero wymyślania)

**Stan zmierzony (public/):** `pwa-512.png` (512², 60 KB), `pwa-512-maskable.png` (512², 41 KB), `favicon.svg`, `favicon.ico`, `apple-touch-icon.png`, `og-image.png` (111 KB), `mossad-radar-logo.jpg`. Ikony generuje `scripts/generate-brand-icons.py` (komentarz w favicon.svg: „nie edytuj ręcznie — rozjedzie się z rastrami").

**Znak (z favicon.svg, zmierzony):**
- tło: `#06090f` (near-black navy), pełny kwadrat;
- słońce: radial green `#20c568` → `#13763e` → transparent;
- znak: biały, stroke 4.684, chevron/góra (wspólny motyw z 3T3R; różni się TYLKO kolorem słońca: mosADD zielone, 3T3R fioletowe);
- belka bazowa: `#26262c`.
- Paleta light/dark z `color-palette.json`: primary dark `146 72% 45%`, light `145 100% 28%`.

**Deliverable do rejestrów:**
1. `mosadd-mcp-512.png` — **512×512 dokładnie**, PNG, tło nieprzezroczyste `#06090f`, margines bezpieczeństwa ~10% (znak w polu 410 px), bez tekstu (nieczytelny w 64 px).
2. `mosadd-mcp-512-maskable.png` — wersja maskowalna (safe zone 20% — istnieje już `pwa-512-maskable.png`).
3. `mosadd-mcp-512-white.png` — wariant na jasne tła rejestrów: ten sam znak, tło białe, słońce `145 100% 28%`, korpus znaku `#06090f`.
4. `mosadd-mcp-128.png` — 128×128 (Docker/Smithery thumbnail).
5. `mosadd-og-1200x630.png` — do linków w postach (PH/HN/Reddit unfurl); istniejący `og-image.png` do sprawdzenia, czy ma 1200×630.
6. **Zakaz:** nie generować nowego logo poza `generate-brand-icons.py` (ryzyko rozjazdu marki).
7. Do sprawdzenia przez Boga/NAMIESTNIKA: czy `pwa-512.png` nadaje się 1:1 bez obróbki (sprawdzić optycznie na białym tle) — jeśli tak, punkt 1 = kopia, zero pracy.

## 5. POLA DODATKOWE WNOSZONE DO KAŻDEGO ZGŁOSZENIA

- **Privacy policy:** https://mosadd.com/privacy.html (istnieje, 16 KB) — Anthropic wymaga sekcji „Privacy Policy" też w README dla connectorów lokalnych; dla remote: URL polityki.
- **Terms:** https://mosadd.com/terms.html (istnieje).
- **Support / contact:** support@mosadd.com **do ustawienia** (Anthropic/OpenAI wymagają kontaktu wsparcia — Bóg podaje adres; NIE zakładam skrzynki sam).
- **Screenshots:** do zebrania — patrz lista niżej (wymóg Anthropic/PH galerii).

### Shot list (do rejestrów i galerii)
1. mDM: 1 kontakt, 3 nazwane wątki (`#projekt`, `#pieniądze`, `#flota`) — mock lub realny zanonimizowany.
2. mDM: voice note + waveform.
3. mIRC: kanał `#command`, lista ról, AES-256-GCM badge.
4. mTALK: pokój PTT, wskaźnik „mówi: agent-claude".
5. mAYL: mail z pieczęcią `sent_by=agent` + status otwarcia.
6. mRAG: graf wiedzy (ingest/search/sąsiedzi/timeline).
7. Linie agentów: karta linii (UUID, właściciel, `send_as_agent`), podpis „agent NIE może pisać jako właściciel".
8. MCP: `claude mcp add mosadd https://mcp.mosadd.com/mcp` + lista 85 narzędzi w kliencie.
Format: 1600×1000 (16:10) lub 1280×800, PNG, bez danych osobowych, watermark brak.

## 6. DYSCYPLINA TWIERDZEŃ (krytyczne przed publikacją)

Z `key-messages.json` (brand-kit, honesty):
- **E2EE dotyczy TYLKO DM-ów 1:1 (X3DH + Double Ratchet).** Kanały/pokoje/mail = szyfrowane w transporcie i at-rest (AES-256-GCM + HMAC) — **NIE** nazywaj ich E2EE w żadnym rejestrze (odrzucenie + utrata zaufania na HN).
- Status: **aktywna alfa**, brak niezależnego audytu bezpieczeństwa, brak SOC2/ISO/HIPAA — nie deklarować.
- „85 tools" = fakt liczbowy, używaj wszędzie (konkret > przymiotnik).
