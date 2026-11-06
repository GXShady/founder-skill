# CFO's note: TODO Safe Return Kit

**Every cost is an estimate** (there are no supplier quotes yet; see `cfo-sources.md`). One sale = one new customer: the $249 device plus the plan they pay in their first year (on average 9.19 months × $24.99, assuming 5% cancel each month). Revenue is before US sales tax, which varies by state. Not financial, tax or legal advice: have an accountant check the structure and tax before money moves.

- **The margin:** each new customer leaves **$130.88 (27%)** after their own costs. At the plan of 1 new customer a day, the profit margin is **24%**, and year 1 operating profit is **$19,511** on $95,493 revenue. Break-even is about 1 customer a day.
- **The line to watch: what ads cost per customer.** That number is a guess ($60). At $120 per customer, year 1 profit falls to $7,541. At $180, year 1 **loses $4,429** and the business never covers its costs. Nobody knows this number until a real ad test runs.
- **Cash:** the tool says **$12,807** before it pays for itself, more than your $10,000. In practice you'll need **more like $18–20k**, because:
  - the tool counts a customer's first-year plan the moment they sign up, but it really arrives month by month;
  - after the first 50 kits you have to pay for each new batch of devices (~$155 each) before you sell them.

  Not included: building your own app (if the factory's app isn't good enough; likely $20k+, estimate) and any extra certification work. Ask each factory for its FCC certificate.
- **Three ways to improve the margin (from the tool):**
  1. **Get the device under $100.** At $95 per unit, contribution rises from $130.88 to $160.88 per customer and year 1 profit from $19,511 to $25,496. Get quotes from 3–4 factories.
  2. **Cut ad cost per customer with referrals and partners** (special-needs schools, therapists, parent groups). Every $60 saved per customer adds about $12,000 to year 1 profit.
  3. **Keep customers longer.** The plan is where the profit is. The price -10% what-if shows how thin it gets: a $30 smaller first-year take drops year 1 profit from $19,511 to $13,526. Push annual plans ($19.99/mo paid up front) to cut cancellations.
- **Board's money conditions:**
  - *"Positive unit economics including connectivity":* **met on paper** ($130.88 per customer after mobile data). Not proven until there are real factory quotes, a real data-plan quote and a real ad test.
  - *"Define the subscription from the data cost":* done ($24.99/mo against ~$10/mo estimated data and cloud).

---

# Unit economics: TODO Safe Return Kit (white-label 4G body camera + app), US online

Every number below comes from the input file. Nothing is looked up or guessed.

## One new customer (device + first-year plan)

| line | per new customer (device + first-year plan) |
| --- | ---: |
| Price | $478.66 |
| Plan revenue counted in price: 9.19 avg paid months x $24.99 (5%/mo cancel, ESTIMATE); device $249 | -$0.00 |
| Device from OEM factory, branded (ESTIMATE) | -$125.00 |
| Freight + US import duty (ESTIMATE) | -$12.00 |
| Box + wear kit incl. locking harness (ESTIMATE) | -$10.00 |
| Spare battery pack (ESTIMATE) | -$8.00 |
| Outbound shipping (ESTIMATE) | -$9.00 |
| Card fees: 2.9% + $0.30 x 10 charges | -$16.88 |
| Mobile data + video relay: 9.19 months x $10 (ESTIMATE) | -$91.90 |
| 30-day refund + warranty reserve (ESTIMATE: 10% return, ~$150 loss each) | -$15.00 |
| Paid ads per customer (ESTIMATE; unknown until tested) | -$60.00 |
| **Contribution** (what each new customer (device + first-year plan) leaves to pay the fixed costs) | **$130.88** (27%) |

## The margin that matters

Fixed costs: $550 a month (App backend + cloud (ESTIMATE) $300, Online store + tools (ESTIMATE) $100, Product liability insurance (ESTIMATE) $150).

- **Break-even: 1 new customer (device + first-year plan)s a day.** Below that you lose money every month.
- **Profit margin at your plan** (1 a day): **24%** of every sale, after every cost.
- Capacity: 5 a day.

## Year 1, month by month

| month | new customer (device + first-year plan)s a day | revenue | profit | cumulative (after $12,650 startup) |
| ---: | ---: | ---: | ---: | ---: |
| 1 | 0 | $1,436 | -$157 | -$12,807 |
| 2 | 0 | $2,154 | $39 | -$12,768 |
| 3 | 0 | $2,872 | $235 | -$12,533 |
| 4 | 0 | $4,308 | $628 | -$11,905 |
| 5 | 0 | $5,744 | $1,021 | -$10,885 |
| 6 | 0 | $7,180 | $1,413 | -$9,471 |
| 7 | 1 | $8,616 | $1,806 | -$7,666 |
| 8 | 1 | $10,052 | $2,198 | -$5,467 |
| 9 | 1 | $11,488 | $2,591 | -$2,876 |
| 10 | 1 | $12,924 | $2,984 | $108 |
| 11 | 1 | $14,360 | $3,376 | $3,484 |
| 12 | 1 | $14,360 | $3,376 | $6,861 |

- **Year 1 operating profit: $19,511** on $95,493 of revenue.
- After the $12,650 startup spend: $6,861.
- Startup money earned back: month 10.
- Cash you need before it pays for itself: **$12,807**.

## What if

| scenario | margin at plan | break-even a day | year 1 profit |
| --- | ---: | ---: | ---: |
| Base plan | 24% | 1 | $19,511 |
| Price -10% | 15% | 1 | $9,961 |
| Volume -20% | 23% | 1 | $14,288 |
| Unit costs +15% | 13% | 1 | $9,103 |

No red flags in these numbers. They are only as good as the inputs: check every cost against a real quote.
