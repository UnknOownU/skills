# 3-minute demo script — Veto (the accountant that says NO)

Recording setup: Claude Code full screen (font zoomed ~140%), phone ready
for the card payment, Qonto app open in a browser tab for proof shots.
One take per scene is fine — assemble cuts, keep total ≤ 3:00.

## 0:00–0:20 — Hook (voice-over on title card or Qonto app)
> "On September 1st, France's e-invoicing reform kicks in — every French
> business must be ready to receive e-invoices, and a French B2B invoice
> missing the client's SIREN won't even route. But here's the thing no API
> can know: whether YOU are allowed to charge VAT. Mine caught me — I'm a
> micro-entrepreneur, and charging 20% VAT would have been illegal. I built
> Veto, the accountant that says no. Then it goes and gets your money."

## 0:20–0:50 — Scene 1: audit before damage
Prompt: `Audit my client book for French e-invoicing readiness.`
- Show the complete client book classified READY / BLOCKED / OUTSIDE FR B2B
  SCOPE, with Blue Fox blocked for its missing SIREN and an exact fix.

## 0:50–1:15 — Scene 2: the agent says NO (compliance)
Prompt: `Invoice Blue Fox Studio €800 for logo design`
- Show: hard block — client has no SIREN → "cannot be routed on the French
  e-invoicing network", asks for the SIREN.
Prompt: `Invoice Qonto €1,200 with 20% VAT`
- Show: the agent catches the org is under **franchise de TVA** — charging
  VAT would be illegal — and corrects to 0% + "TVA non applicable,
  art. 293 B du CGI".
> "It just stopped me from breaking the law on my own account. Twice."

## 1:15–1:50 — Scene 3: compliant invoice, human in command
Prompt: continue → full summary table (SIREN, amounts, due date,
late-payment mentions injected) → agent asks "Shall I create it?"
- Confirm. Invoice created. Cut to Qonto app showing the real invoice.
> "Every write needs my explicit yes. The agent prepares — I decide."

## 1:50–2:25 — Scene 4: real payment proof
Prompt: `Create a €2 standalone test payment link and check it while this session is active.`
- Show link created → pay it on the phone (real card, on camera) → agent
  polls → **"🎉 Payment received — 2,00 € — paid ✅"** and correctly says
  no invoice was reconciled because the link was standalone.
> "Real money, real account, and an agent honest about what it did — and
> what it did not do. Invoice-linked reconciliation follows the same
> guarded flow when a legitimate invoice is used."

## 2:25–2:48 — Scene 5: Monday morning (relance)
Prompt: `Who owes me money? Draft reminders for anyone overdue.`
- Show: overdue table (client, amount, days late) + escalating reminder
  drafts (friendly → firm → mise en demeure) with penalties computed
  (contract rate + €40, calculation shown). Agent hands drafts — never sends.

## 2:48–3:00 — Close
- Flash: deterministic validator checks, eval definitions, repo structure,
  and security note. Only show "evals passing" if an actual run was recorded.
> "Veto — the invoice agent that says no, then gets you paid. Compliant by
> default, human in command. Built on the Qonto MCP. Repo linked below —
> try it on your own account."

## Backup plan
Record EVERY scene as soon as it works once. If the live payment fails on
the final take, use the backup recording — never re-shoot under stress.
