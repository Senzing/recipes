# Patient Fraud - synthetic ingredient set

Four synthetic source systems from **UK private healthcare in London**, built for the
[Patient Fraud Detection in UK Private Healthcare](../../recipes/patient-fraud-uk.md) recipe.

**Synthetic - no real people, no PII.** NHS numbers use the 999 test prefix, phone numbers come from
Ofcom's drama ranges, and every person, clinic, company number and bank account is invented.

| File | Rows | What it is |
|---|---|---|
| `gp_registrations.csv` | 511 | NHS GP practice registrations. One row per registered patient; the most trusted source. |
| `pharmacy.csv` | 241 | Community pharmacy dispensing records, with the item and last dispensed date. |
| `clinic_billing.csv` | 240 | Private clinic claims billed to an insurer. One row per claim, with the treatment, amount and sometimes a refund bank account. |
| `providers.csv` | 28 | The private clinics (company number, business details), their directors and other clinicians (GMC number, home details). `provider_type` says which. |

The four files deliberately **don't share field names** - mapping them to the Senzing spec is part
of the recipe. Seeded in the data: medical identity theft, ghost patients billed by a colluding
clinic, and one NHS number used by two different people, alongside innocent lookalikes (households,
house moves, nicknames) that should not be flagged.
