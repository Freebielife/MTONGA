# Make TON Great Again Observatory

## О проекте / токене

MTONGA \(Make TON Great Again\) — токен сообщества в сети TON. На сайте проект описывает себя как мем-сообщество, вдохновлённое культурой TON и Telegram, и указывает, что не связан с Telegram, TON Foundation или Павлом Дуровым. В метаданных токена источником вдохновения назван пост Дурова https://t.me/durov/482.

Краткое описание по указанным первичным источникам.

Источники (проверены 2026-11-26):

- <https://www.mtonga.com/>
- <https://tonapi.io/v2/jettons/EQDuGgqZU7_AEgiOwEe-abozIefuoairTWLOyd7c_f8GhzMf>

Generated from https://github.com/Freebielife/TON-Observatory-Template.

Run python3 -m scripts.refresh_observatory; python3 build.py; python3 verify.py.
Publish index.html in TON Sites only after independent on-chain verification.
A live TonAPI snapshot is included. Collection time and per-section coverage are recorded in data/snapshot.json.
Only native TON swap pairs supported. Locks, staking and custom project NFT badges are configured through project.json and verified against TonAPI.
The generated update.yml accepts workflow_dispatch from the existing external scheduler and runs on source changes. Production Cloudflare registration has not been independently verified.

Foundation version: 1.3.0. Holders show 10, expandable to top 20.
`project.json` is the per-project specification. Contract/pool/precision changes require regenerating from the factory; do not reuse another token's snapshot.
Run `python3 build.py` for an atomic bundle and `build/report.json` size report.
No external fonts, scripts or images are needed to render the saved page. Fresh data checks and manual wallet lookups require network access.
Cloudflare dispatch registration and GitHub repository access remain separate deployment steps. No credentials go into HTML.

## MTONGA verification — 2026-11-26

- Exact contract and 9 decimals confirmed using TonAPI; official website displays the same friendly master.
- Successful native TON swaps confirmed for DeDust and STON.fi pools in project.json. Trading history remains partial and accumulates on each refresh.
- User-selected cap image is embedded as hero artwork. Section artwork is the explicitly selected TONecoFlags #196. No inherited project-specific NFT/DEV/staking rules are enabled.
- Shared OG, Fragment +888, 4-digit DNS and burn badge rules retained. Unconfirmed ownership is never inferred.
- Responsive browser QA: widths 320, 390, 768 and desktop 1363; document width did not exceed viewport. RU/EN and 10→20 holders checked; chart rendered. External rendering dependencies rejected by build guard.
- No verified lock/staking source is configured; UI states this explicitly.
- main publication is distinct from uploading index.html to TON Storage. No TON Storage upload or domain change was performed.
- The initial template commit remains recoverable in Git history: 15a07dff687f1494ce404a38684cffa4777eac4d.

Template: 1.3.0, source commit 65780137fa12eda7500f48d29c5b261411305274.

External link HTTP checks: project website returned 200; Telegram, X and gram.org returned 403 in this environment. Their availability was not established. URLs match user instructions and token metadata.
