# Competitors: TODO (US launch assumed)

Public sources only, read 2026-11-06. Prices come from vendor pages and review sites and shift often. Re-check before quoting. Raw data: `competitors.csv`.

## 1. Who is there (most direct first)

| name | type | device | monthly | what it does | camera for caregiver? |
| --- | --- | --- | --- | --- | --- |
| [AngelSense](https://www.angelsense.com/help/pricing-plans-explained/) | direct | device + $59 activation (month-to-month) | $44.99–$64.99 ([SafeWise](https://www.safewise.com/angelsense-watch-review)) | Special-needs GPS, auto-answer 2-way voice, listen-in, SOS, lock-on strap | No (audio listen-in only) |
| [Amber Alert GPS](https://www.bmc.org/sites/default/files/2024-05/Tracking%20Devices.pdf) | direct | from $229 | $44.99 | GPS, SOS, voice to caregiver | No |
| [Theora Connect](https://caring.com/resources/tracking-devices-for-dementia-patients) | direct | not found | not found | Dementia watch, safe zones, elopement alerts, SOS | No |
| [TickTalk 5](https://www.myticktalk.com/blogs/news-1/ticktalk-vs-gabb-kids-smartwatch-features-and-pricing-comparison-smartphone-alternatives) | indirect | $159.99 | $9.99 | Kids 4G watch, **video calls**, GPS, SOS | Video call only (wearer must answer and hold it up) |
| [Bark Watch](https://www.safewise.com/social/best-smartwatches-for-kids/lp/) | indirect | $129–$169.99 | ~$15 | Kids watch, video calling, GPS | Video call only |
| [Gabb Watch 3e](https://www.safewise.com/social/best-smartwatches-for-kids/lp/) | indirect | $149.99 + $30 activation | $17.99 | Kids watch, GPS, SOS, calls | No |
| [Jiobit](https://www.jiobit.com/product) | indirect | $99.99–$149.99 | $8.33–$14.99 | Small GPS tag, kids and seniors | No |
| [Bay Alarm Medical](https://www.caring.com/senior-products/best-medical-alert-systems/bay-alarm-medical/) | indirect | ~$79–$149 | $29.95–$39.95 (+$10 fall detection) | Senior SOS pendant/watch, GPS, monitored call centre | No |
| [Medical Guardian](https://www.caring.com/senior-products/best-medical-alert-systems/medical-guardian-vs-bay-alarm-medical) | indirect | $149.95–$199.95 | $39.95–$46.95 | Senior mobile alert, GPS, monitored centre | No |
| [4G body cams (OEM)](https://www.globalsources.com/Wearable-camera/body-camera-1226137271p.htm) | indirect | ~$120–$130 wholesale | SIM/platform | Live-streaming body cam, GPS, 2-way audio, for security/police | Yes, but built for security, not families |

**Substitutes:** [Project Lifesaver](https://www.leecountysheriff.net/project-lifesaver) via local sheriffs (~$300 transmitter + $10–$25/mo, often grant-funded); [Apple AirTag](https://www.theshortcut.com/p/airtags-price) hidden in clothing ($29); [Life360](https://www.itechguides.com/what-is-life360-how-it-works-features-and-free-vs-paid-plans/) on a phone ($0–$24.99/mo, needs the wearer to carry a phone); or simply supervising in person.

## 2. Price range (comparable wearable with voice, GPS and SOS)
- **Device:** lowest ~$100 (Jiobit on sale), median ~$150, highest ~$230 (Amber Alert GPS). $200–$300 for TODO sits **at or above the top** of this range.
- **Monthly plan:** lowest $8.33 (Jiobit annual), median ~$30, highest ~$65 (AngelSense month-to-month). Special-needs and senior-alert products charge **$30–$65/mo**. Kids' watches charge $10–$18.

## 3. Positioning map
Axes: **how much the caregiver can see** (location only → voice → live video) × **who it's built for** (general kids → vulnerable or special needs).

```
                  built for vulnerable / special needs
                              |
   AngelSense (voice)         |          [EMPTY: TODO's spot]
   Amber Alert (voice)        |          live video + voice + SOS
   Theora, Bay Alarm,         |          built for vulnerable people
   Medical Guardian (voice)   |
location ---------------------+--------------------- live video
   Jiobit, AirTag,            |   TickTalk, Bark (video *calls*)
   Life360, Gabb              |   4G body cams (security, not families)
                              |
                   general kids / security
```

## 4. What customers complain about (AngelSense, the closest direct competitor)
1. **Battery: daily charging, about 16–24h** (strong: [PCWorld](https://www.pcworld.com/article/3268564/wearables/angelsense-gps-review.html) ~18h, "be diligent about charging … every night"; [G2](https://www.g2.com/products/angelsense/reviews) "typically lasts only a day"; [Trustpilot](https://www.trustpilot.com/review/angelsense.com?page=2) "needs charging daily"; [Choosing Therapy](https://www.choosingtherapy.com/?p=105185) 16–24h).
2. **Limited voice minutes and contract lock-in** (thin: [Trustpilot](https://www.trustpilot.com/review/angelsense.com?page=4) "only comes with 60 minutes of voice time"; 12-month contract with remaining payments due).
3. **Location errors and charging glitches** (thin: [Trustpilot](https://www.trustpilot.com/review/angelsense.com?page=7) "places the child in the wrong location", reboot through the app to fix charging).
4. **Lock-on strap: both loved and hated** (thin: praised for keeping a child with high-level autism safe, criticised because it can't be switched off; [Trustpilot](https://nl-be.trustpilot.com/review/angelsense.com)).
5. **Listen-in raises privacy and legal concerns** ([PCWorld](https://www.pcworld.com/article/3268564/wearables/angelsense-gps-review.html)).
6. Kids' watches (Bark, Gabb) "struggled to make it through a full school day" in one test ([source](https://digikidz-com.pages.dev/best-kids-smartwatches)), thin.

Overall sentiment for AngelSense is high (4.5 on Trustpilot from 321 reviews), so the incumbent is liked, not hated.

## 5. The gap
**No product found gives a caregiver a live view from the wearer's body plus voice, SOS and GPS in a device built for vulnerable people.** Special-needs trackers stop at audio listen-in. Kids' watches do video *calls*, which need the wearer to answer and hold up their wrist, and that fails for the very people TODO is for. Body cams have the hardware but are built and sold for security. A search for dementia wearable cameras turned up only research prototypes ([Duquesne study](https://dsc.duq.edu/faculty/962)).

The catch is that **battery life is already the #1 complaint for audio-only devices**. Live video uses far more power and data, so TODO's gap only holds if it solves battery better than AngelSense, not worse. The privacy concerns around listen-in will be stronger for video, which makes TODO's privacy mode a selling point.

## 6. The threat
- **AngelSense** is the fastest copier. It already owns the buyer, the channel (special-needs parents) and a monthly plan. Adding a camera to its next device would erase TODO's gap.
- **TickTalk / Bark** could add a caregiver-initiated "auto-answer video" mode in software.
- **OEM body-cam factories** already sell 4G live-stream + GPS + 2-way audio hardware for ~$120–$130 wholesale, so a copycat brand could launch quickly. This is also good news, because TODO's white-label route looks feasible.
