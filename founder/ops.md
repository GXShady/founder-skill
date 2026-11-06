# Operations: TODO Safe Return Kit (US, online, solo founder)

## 1. The daily cycle (👁 = customer sees it)
1. Check the app/cloud dashboard: any device offline, SOS failures or alerts overnight? (fix first)
2. 👁 Answer support messages and emails (target: under 4h; urgent safety issues immediately)
3. 👁 Run booked 10-minute setup calls
4. Pack and ship new orders (device, spare battery, wear kit, SOS card); print labels
5. 👁 Send shipping confirmation + setup-call booking link
6. Process returns: test, wipe data, refurbish or scrap
7. Check ads (cost per deposit) and stock level
8. 👁 Post one piece of content / answer one group question
9. End of day: log any device or connection problem in the issue tracker

## 2. Suppliers (get quotes; nothing here is a confirmed price)
| input | where | known price | MOQ / lead time | notes |
| --- | --- | --- | --- | --- |
| 4G body camera with GPS, 2-way audio, SOS, live stream | Alibaba / Global Sources factories (e.g. [listing](https://www.globalsources.com/Wearable-camera/body-camera-1226137271p.htm), [listing](https://electronics.alibaba.com/product/body-camera-with-live-streaming)) | ~$120–130/unit listed | often 1–2 units for samples; custom logo usually 100–500+ | **Ask every factory for:** a valid **FCC ID** (search it in the [FCC database](https://fccid.io/)), US LTE bands (AT&T/T-Mobile/Verizon), battery hours with streaming, SDK/API access to the video stream, and a white-label app option. Order samples from 3–4 factories. |
| Kids/elderly 4G GPS watch factories (alternative: same app ecosystem, video calls) | Shenzhen OEMs on Alibaba | quote | quote | Many come with a white-label app; check data-privacy and COPPA terms |
| Cellular data (IoT SIM) | [Hologram](https://hologram.io/pricing/) | ~$0.03/MB + $1/SIM/month + $3/SIM (self-service, check current page) | none | Alternatives: 1NCE, KORE, Twilio IoT. Get volume quotes. |
| Video relay / cloud | AWS Kinesis Video, Agora, or the OEM's platform | usage-based, quote | none | Pick based on what the factory's firmware supports |
| Spare batteries, harness, lanyards, armbands | Same factory (bundle) or accessory suppliers on Alibaba | quote | 100+ typical | |
| Retail box + SOS card | Packlane, Arka, or a local printer | quote | 50–100 | |
| Shipping | USPS Ground Advantage via Shopify Shipping / Pirate Ship | ~$9 est. | n/a | |

**Data cost check (important):** at $0.03/MB, 30 minutes of live video at ~1 Mbps (~225 MB) costs about **$6.75**, plus $1 SIM fee and very little for GPS. That's about $8/month, inside the CFO's $10 estimate. **But 2 hours of video a month (~900 MB) costs about $28**, more than the $24.99 plan. That's why the SOS-first camera matters: **cap live-video minutes per tier** (e.g. SOS tier: video during SOS only; Live tier: 60 min/month, then lower resolution). The CFO's numbers hold only with a cap. No change to `numbers.json` yet; re-run the CFO once you have real quotes.

## 3. People
- **Months 1–3 (≤ 0.3 customers/day):** founder only, about 15–20 h/week: support 1h/day, setup calls (2–3/week), packing 2h/week, content/groups 1h/day, factory and app work as needed.
- **At plan (1 customer/day ≈ 30/month):** about 30–35 h/week. Add a part-time contractor for support and setup calls (~10 h/week) when support passes 1.5h/day. Wage assumption: ~$20–25/h contractor (ESTIMATE; check local rates). This is not in `numbers.json` yet; it would add ~$1,000/month in fixed costs, so the CFO should re-run when you hire.
- **Engineering:** the riskiest gap. Someone must connect the factory's device to the app and cloud. Either the factory's white-label app works (cheapest), or you need a contract developer (budget unknown; likely $20k+ for a custom app, estimate). Decide this after the samples arrive.
- Payroll taxes and contractor rules: ask an accountant.

## 4. Routines
**A. Morning check (10 min)**
1. Open the device dashboard: list devices offline > 2h, or with battery < 15% and no charge overnight.
2. Message those families: "Just checking: [name]'s device has been offline since 7am. Need help?"
3. Check SOS logs: did every SOS reach the caregiver? Any failure gets investigated today and reported to the family.
4. Clear urgent support messages.

**B. Fulfilment (per order)**
1. Pull a kit; test it: power on, SIM active, GPS fix, test SOS to the test phone.
2. Register the device ID to the customer's account; ship with the SOS card on top.
3. Send tracking + "book your 10-minute setup call" link.

**C. Setup call (10 min)**
1. Caregiver installs the app; pair the device by QR code.
2. Choose the wear option; fit the harness if needed.
3. Run a test SOS together: caregiver sees, hears and talks.
4. Explain privacy mode, the viewing log and the spare battery.
5. Ask: "Who else should get the SOS alert?" Add backup contacts.

**D. Complaint or failure**
1. Reply within 24h (immediately if safety-related): apologise, ask what happened, offer a call.
2. Pull the device logs. Was it battery, signal, app or user setup?
3. Fix, replace or refund; the 30-day refund is honoured without argument.
4. Log it; if the same problem appears 3 times, stop selling until it's fixed.

**E. Weekly reorder (Fridays)**
1. Count kits in stock + on order.
2. If stock < 4 weeks of sales + lead time, order the next batch (factory lead time ~3–6 weeks, estimate).
3. Check the cash balance first: restocks are paid up front (see `cfo.md`).

## 5. Tools
| job | tool | price | why |
| --- | --- | --- | --- |
| Store + checkout | Shopify Basic | see [shopify.com/pricing](https://www.shopify.com/pricing) | Deposits, subscriptions (via app), shipping labels |
| Subscriptions | Shopify subscription app or Stripe Billing | Stripe 2.9% + $0.30 per charge (check [stripe.com/pricing](https://stripe.com/pricing)) | Month-to-month billing, cancel in-app |
| Setup calls | Calendly free + Google Meet / Zoom | free tier | Booking link in the box |
| Support inbox | Gmail / Google Workspace | ~$7/user/mo (check) | Simple start |
| Bookkeeping | Wave (free) or QuickBooks | check current prices | Keep inventory and subscription revenue separate |
| Issue tracker | Notion or a spreadsheet | free | Log every device problem |

## 6. Licences, permits, compliance (confirm each; not legal advice)
- **Business registration:** an LLC in your state (state Secretary of State website) + an [EIN from the IRS](https://www.irs.gov/businesses/small-businesses-self-employed/apply-for-an-employer-identification-number-ein-online) (free).
- **Sales tax:** register in your state and any state where you pass economic nexus thresholds; Shopify can calculate it.
- **FCC:** cellular devices sold in the US need FCC equipment authorization ([47 CFR 2.1204](https://www.law.cornell.edu/cfr/text/47/2.1204)). **Only buy a device that already has a valid FCC ID**; a white-label rebrand can often use the factory's grant, but confirm with the factory and the FCC rules.
- **Carrier certification:** check with your IoT SIM provider that the device module is approved on the US networks it will use.
- **COPPA (children's privacy):** the FTC treats children's **location, photos, video and audio** as personal information, and connected devices and apps are covered ([summary](https://adexchanger.com/data-exchanges/ftc-updates-coppa-with-new-restrictions-on-location-data-photos)). You need a clear privacy notice, **verifiable parental consent**, data security and deletion rules, and you're responsible for your vendors' SDKs. The FTC has warned kids' GPS-watch makers before. **Budget for a privacy lawyer review before launch.**
- **Recording consent laws:** about 11–13 states require all-party consent for audio recording (commonly listed: CA, DE, FL, IL, MD, MA, MT, NV, NH, PA, WA, with others in some lists) ([overview](https://www.getnexar.com/blog/dash-cam-privacy-laws-by-state)). Two-way calls the wearer joins are different from silent listen-in, but have a lawyer confirm. **Don't build a silent "listen-in" feature** without legal advice.
- **Health/medical claims:** don't market it as a medical device or claim it prevents harm, to stay clear of FDA medical-device rules and FTC advertising rules.
- **Insurance:** product liability + general liability + cyber/data breach. Get quotes from a small-business broker; $150/month in `numbers.json` is an estimate.
- **Battery shipping:** lithium batteries shipped inside or packed with equipment have carrier rules (USPS/UPS); check before shipping spares.

## 7. Risk register
| # | risk | likely | how bad | plan |
| --- | --- | :-: | :-: | --- |
| 1 | SOS or video fails in a real emergency | med | severe | Test every kit before shipping; morning log check; honest dead-zone messaging; stop sales after 3 repeat failures |
| 2 | Battery doesn't last a day with streaming | high | high | Test samples for real battery life before choosing a factory; spare battery in the box; SOS-first camera saves power |
| 3 | Factory app is poor or insecure | high | high | Test apps from all samples; security review; budget for a contract developer if needed |
| 4 | Data costs exceed plan price | med | high | Video-minute caps per tier; monitor MB per user weekly |
| 5 | Privacy/COPPA complaint or FTC issue | low–med | severe | Lawyer review pre-launch; parental consent flow; data minimisation; no silent listen-in |
| 6 | Wearers remove or refuse it | high | high | Locking harness, comfort tests with pilot families; 30-day refund catches it early |
| 7 | Ad cost per customer > $95 | med | high | Partners and groups first; kill ads that don't work; CFO shows the break point |
| 8 | Factory delays or quality drop on reorder | med | med | Two qualified factories; inspect samples from each batch |
| 9 | Cash runs out while waiting on restocks | med | high | Raise to ~$18–20k before launch; pre-orders with deposits; small batches |
| 10 | Founder burnout (support + calls + engineering) | med | med | Hire part-time support at 1/day; automate setup with videos |
