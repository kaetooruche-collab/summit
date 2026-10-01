# Brevo campaign archive

Reference material for planning future campaigns. Account: HIBARR (German-language, hibarr.de).

## Layout
- `data/` raw pulls from the Brevo API (dated).
- `reports/<campaign-family>/` analysis per family.
  - `webinar-invites/` pre-webinar invitations by audience segment
  - `post-webinar/` follow-ups with recording
  - `cielo-vista-dto/` property promotion to German leads

## Snapshot (pull of 2026-10-01; 10 most recent sent of 417 total email campaigns)
| Family | Best open % | Clicks | Take-away |
|---|---|---|---|
| Post-webinar follow-up | 37.5 | 4 clickers / 22 | Warm audience + recording is the strongest performer |
| Webinar invite (attended list) | 10.3 | 1 / 686 | Outperforms never-attended list 2.4x |
| Webinar invite (never attended) | 10.6 -> 4.3 | 1 -> 0 | Declining; refresh angle/segment |
| Cielo Vista DTO | 14.4 | 1-2 per send | Same list mailed ~3x simultaneously; verify |

## Caveats
- Open rates include Apple Mail Privacy Protection opens; clicks are the more reliable signal.
- Brevo `linksStats` showed 0 per link even where clickers were reported, so link-level data is not trustworthy for these sends.
- Only email was pulled. SMS campaigns returned empty. Older campaigns (407 more) are not yet archived.
