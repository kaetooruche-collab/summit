# Email copies

Full HTML as sent, pulled from the Brevo API on 2026-10-01. Personalisation tokens (`{{contact.FIRSTNAME}}`) are left as-is.

| File | Campaign | Subject | Preview text |
|---|---|---|---|
| `1438_...` | Tue webinar invite, past registrants (Sep 29) | Heute 19:00: 391 Seiten Belege, Konto trotzdem gekündigt | Ein Kunde lieferte alles, was die Bank verlangte – 32.000 Euro blieben eingefroren. |
| `1447_...` | Post-webinar follow-up (Sep 30) | 391 Seiten Belege: Warum Legalität nicht mehr schützt | BaFin-Strafe & Kontosperrungen: Warum Banken durchgreifen und was das für Sie bedeutet (Aufzeichnung). |
| `1458_...` | Thu webinar invite, past registrants (Oct 1) | Gestern hat Deutschland Bankdaten mit 118 Ländern geteilt | Das war nicht die einzige wichtige Entwicklung, die diese Woche den Zugang zu Ihrem Geld betrifft. |
| `1442_...` | Cielo Vista DTO German leads (Sep 29) | Studio-Apartment in Nordzypern ab £52.000 (~£260/Monat) | 0 % Bauträgerfinanzierung bis 2032. Individuellen Zahlungsplan prüfen & Beratung buchen. |

## Not saved separately
- 1443, 1444, 1450 (Cielo Vista): same subject/preview as 1442; only the UTM campaign name differs. Not fetched individually, so identical body is assumed, not verified.
- 1456 (Thu invite, attended list): same subject as 1458 with a different audience and `utm_term=teilgenommen_tag1`. Body not fetched, so it may differ.
- 1448, 1449: single-recipient resends of 1447.

## Notes for reuse
- The 1447 file starts with an HTML comment carrying a different subject/preview ("391 Seiten Belege. Konto trotzdem eingefroren.") than the one actually sent.
- The 1458 CTA points to `hibarr.de/en/webinars/faszination-nordzypern-investment-oder-neue-heimat` (English path, Cyprus webinar slug) while the email body is about German bank data; the fallback link text shows `hibarr.de/webinar`. Worth checking the destination matches the message.
- The 1442 CTA label ends with a stray `→;` and the Outlook (VML) button has a different UTM campaign name than the standard button.
- Brevo's SMS endpoint returned nothing.
