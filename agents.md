# Sub-Agent Task Log

## Standing Rules
- **Always use `run_in_background: true`** for ALL agents — research, file updates, git, link checkers, everything. No exceptions.
- As each agent completes, merge its results into `itinerary.md` and commit to git
- Link checker agents should run after each city's research set is complete

One research agent per city. Each agent returns 3 hotel recommendations meeting: central location, ~£45/night, 4★ minimum.

| Agent | City | Nights | Dates | Output file |
|-------|------|--------|-------|-------------|
| 1 | Chongqing | 3 | 19–21 May | `hotels/chongqing.md` |
| 2 | Chengdu | 2 | 22–23 May | `hotels/chengdu.md` |
| 3 | Guangyuan | 1 | 24 May | `hotels/guangyuan.md` |
| 4 | Xi'an | 2 | 25–26 May | `hotels/xian.md` |
| 5 | Beijing | 4 | 27–30 May | `hotels/beijing.md` |

## Status
- [x] Chongqing — Walling Hotel, Yuexuan Hotel, Qianhe Rishan River View
- [x] Chengdu — Mercure Chunxi, Lyhn International Taikoo Li, Atour Taikoo Li
- [x] Guangyuan — Hampton by Hilton Lizhou Square, Wanda Realm, Tiancheng Grand
- [x] Xi'an — Holiday Inn Express Bell Tower, Jinmao Downtown, Eastern House
- [x] Beijing — Guo Ji Yi Yuan, Inner Mongolia Grand, Novotel Beijing Peace

## Consolidation
After all agents complete, results are merged into `itinerary.md` under the Hotels section.

---

## Round 2 — 2-bedroom suites

Budget ~£90/night (2-bedroom suite / two-room unit). Output file: `hotels/<city>_suites.md`.

- [x] Chongqing — Somerset Yangtze River, Voyul Guyu Li, Ascott Raffles City
- [x] Chengdu — Somerset Riverview, Ascott Raffles City, Fraser Residence
- [x] Guangyuan — no real 2-BR; fallback 2 rooms @ Wanda Realm / Hampton / Tiancheng
- [x] Xi'an — Citadines Central, Eastern House, Novotel Bell Tower
- [x] Beijing — base-Wangfujing Serviced Apt, Citadines Ritan, Novotel Peace

---

## Round 3 — deep-dive per city (3 angles)

Per city, 3 specialist agents run in parallel:
- **suites** → `hotels/<city>_suites_v2.md` (expanded suite inventory, 5 picks)
- **bedrooms** → `hotels/<city>_bedrooms.md` (expanded standard-room shortlist, 5 picks)
- **cool/splurge** → `hotels/<city>_cool.md` (unique/characterful, worth stretching budget)

### Chongqing
- [ ] suites
- [ ] bedrooms
- [ ] cool/splurge

### Chengdu
- [ ] suites
- [ ] bedrooms
- [ ] cool/splurge

### Guangyuan
- [ ] suites
- [ ] bedrooms
- [ ] cool/splurge

### Xi'an
- [x] suites (xian_suites_v2.md)
- [x] bedrooms (xian_bedrooms.md)
- [x] cool/splurge (xian_cool.md — 10 picks with photos)

### Beijing
- [x] suites (beijing_suites_v2.md)
- [x] bedrooms (beijing_bedrooms.md)
- [x] cool/splurge (beijing_cool.md — photos added)
