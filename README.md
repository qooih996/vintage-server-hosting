# Best Vintage Story Server Hosting: How to Choose the Right Plan, How Much RAM You Really Need, and Is a Dedicated Host Worth It? (Setup, Mods, and Lag Fixes Included)

So you've fallen down the Vintage Story rabbit hole. You've survived your first winter, maybe tamed a few drifters, and now you want your friends to join the fun — except hosting a server on your own PC means your rig doubles as a radiator and your world dies the moment you close the game. Sound familiar? That's exactly the moment most players start Googling "best vintage story server hosting."

This guide walks through what actually matters when picking a host, how much RAM your world really needs, how to keep mods from turning your server into a slideshow, and where a provider like ExtraVM fits into the picture. No fluff, no fake discount claims — just the stuff that helps you decide.

## Why Hosting Your Own Vintage Story Server Gets Complicated Fast

Vintage Story's official site lays out three paths for multiplayer: free local hosting, free internet hosting (UPnP), and paid hosting. The first two work fine if everyone's in the same house or you enjoy wrestling with port forwarding. The moment your group spans time zones, or you want the server online 24/7, the DIY route stops being fun.

The official Vintage Story hosted servers exist too, but they have a real limitation — no mod support yet, and servers sit in central Europe. If you're in North America or Asia, that latency can cause the "crashing a lot" complaints you'll see pop up in Reddit threads from US-based players.

That's the gap third-party hosts fill: mod support, regional locations, and a control panel so you're not SSH-ing into a box at 2 AM trying to restart a process.

## What the Best Vintage Story Server Hosting Actually Needs

Vintage Story's dedicated server requirements aren't wild by modern standards, but they're specific:

- **Memory:** 1 GB base + 300 MB per player
- **CPU:** 4 threads recommended; clock speed matters more than core count (1 GHz base + 150 MHz per player)
- **Storage:** SSD strongly recommended — NVMe even better for chunk loading
- **OS:** Windows or Linux (on Linux you may need `sudo sysctl -w vm.max_map_count=262144` to avoid out-of-memory crashes)

That formula means a 4-player server needs roughly 2.2 GB of RAM, a 10-player server around 4 GB, and a 16-player modded world can push past 6 GB. Single-core CPU performance is the sleeper spec here — Vintage Story's tick loop cares about clock speed more than thread count, which is why old Xeon-based hosts feel sluggish even with "lots of cores."

Beyond raw specs, the things that separate a decent host from a frustrating one:

1. **DDoS protection** — game servers are targets. Unprotected hosts go down for hours when someone gets bored.
2. **NVMe storage** — vintage chunk loading on spinning disks is painful.
3. **Modern CPUs** — Ryzen 9 or Intel i9 class, not mystery "enterprise" chips.
4. **A real control panel** — web console, file manager, one-click mod installer, backups.
5. **In-house support** — outsourced tier-1 reading scripts is useless when your world won't boot.
6. **Regional locations** — pick one close to your players; ping over 150 ms makes combat feel broken.

## How ExtraVM Fits the Vintage Story Hosting Conversation

ExtraVM is a Delaware-registered hosting company (LLC #6623925) that's been around since 2014. They operate three product lines — VPS, game servers, and web hosting — across eight datacenters: Dallas, Los Angeles, Miami, New Jersey, Amsterdam, Singapore, Tokyo, and Sydney.

For Vintage Story specifically, they run the game on their standard game-server stack:

- AMD Ryzen 9 and Intel i9 processors
- NVMe RAID storage
- Enterprise DDoS protection (provided by Global Secure Layer in Dallas/LA, Datapacket in Miami/Singapore/Tokyo, Royale Hosting in NJ/Amsterdam; Sydney has local eBPF/XDP filtering only)
- A custom-built game panel with web console, file manager, SFTP access, backup system, and mod installer
- Free subdomain on `.gamedns.net`
- Instant deployment after payment
- 5-day money-back guarantee (fiat payments only)
- In-house US-based support with sub-30-minute ticket responses and live chat during US daytime

Their game servers are priced on a per-GB-of-RAM model — $3.00/GB for US and Europe locations, $5.00/GB for Singapore and Australia. That's the same pricing structure they use for Minecraft, and it carries over to Vintage Story. A real-world data point: a Reddit user in r/VintageStory reports paying $15/month for 5 GB of RAM and 100 GB of disk space, which lines up exactly with the $3/GB rate. They noted rarely seeing more than 15% CPU usage, which tracks given the strong single-core performance of Ryzen 9 chips.

If you want to dig into their VPS side instead (useful if you'd rather run the server yourself with full root access), the KVM NVMe VPS lineup runs from 1 GB RAM at $4.50/mo up to 64 GB RAM at $192/mo, with most of the larger tiers currently showing as sold out on the Dallas page.

## ExtraVM Vintage Story Plan Comparison

Game-server RAM tiers are selectable on the order page, so the table below reflects the per-GB pricing across common configurations. US/EU pricing is $3/GB; Singapore and Australia are $5/GB.

| Plan (RAM) | Estimated Players (Vanilla) | Estimated Players (Modded) | US / EU Price | Singapore / Australia Price | Get Started |
| --- | --- | --- | --- | --- | --- |
| 2 GB | 3–4 | 2 | $6.00/mo | $10.00/mo | [Order 2 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 3 GB | 6–7 | 3–4 | $9.00/mo | $15.00/mo | [Order 3 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 4 GB | 10 | 5–6 | $12.00/mo | $20.00/mo | [Order 4 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 5 GB | 12–13 | 6–7 | $15.00/mo | $25.00/mo | [Order 5 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 6 GB | 16 | 8–10 | $18.00/mo | $30.00/mo | [Order 6 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 8 GB | 20+ | 12–16 | $24.00/mo | $40.00/mo | [Order 8 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 10 GB | 25+ | 16–20 | $30.00/mo | $50.00/mo | [Order 10 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 12 GB | 30+ | 20–25 | $36.00/mo | $60.00/mo | [Order 12 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 16 GB | 40+ | 25–30 | $48.00/mo | $80.00/mo | [Order 16 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |
| 20 GB | 50+ | 30–40 | $60.00/mo | $100.00/mo | [Order 20 GB](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) |

> Player counts are rough estimates based on the official "1 GB base + 300 MB per player" formula and community feedback. Mods, world age, view distance, and player spread all shift these numbers — sometimes a lot. Start smaller and upgrade if you hit RAM limits; ExtraVM allows plan upgrades at any time via support ticket (downgrades aren't possible due to technical constraints).

If you want to look at the full VPS lineup as an alternative (full root access, you install and run the Vintage Story server binary yourself), the KVM NVMe VPS tiers run from 1 GB RAM at $4.50/mo up to 64 GB RAM at $192/mo. You can 👉 [view the complete VPS plan list](https://extravm.com/billing/aff.php?aff=769&pid=22) for current availability.

## How Much RAM Does Your Vintage Story Server Actually Need?

This is the question every hosting guide gets wrong by either over-provisioning ("get 8 GB to be safe!") or under-provisioning ("2 GB is plenty!"). The honest answer depends on three things: player count, mod count, and world age.

**Vanilla servers, small group (2–8 players):** 2–4 GB is comfortable. A fresh world with 3 players will idle under 1.5 GB used. The 1 GB base + 300 MB per player formula is conservative — most vanilla servers run lighter than that in practice.

**Modded servers, small-medium group (4–16 players):** 4–8 GB. Mods like *Wildcraft*, *Better Ruins*, *Carry Capacity*, and *Prospect Together* add up. A community Reddit thread on 4-player servers with ~50 mods lands on 8–10 GB as "comfortable," though 6 GB is usually fine if you trim your mod list.

**Heavy modpacks, larger communities (20+ players):** 8 GB minimum, 12–16 GB if you're running 100+ mods and an old, sprawling world.

The trap to avoid: throwing RAM at lag that isn't a RAM problem. Vintage Story's server tick loop is CPU-bound, and a lot of "my server is lagging" reports trace back to single-core CPU performance or specific mod configurations, not memory pressure. Check your actual usage in the game panel's console before upgrading.

## Setting Up Your Vintage Story Server on a Hosted Box

Once your server is deployed (ExtraVM does this automatically after payment — usually within seconds), the workflow looks like this:

1. **Log into the game panel.** You'll get credentials by email. The panel includes a web console, file manager, and SFTP details.
2. **Pick your server software.** Vanilla, or a modded setup. ExtraVM's panel supports mod installation through the built-in installer; you can also upload mods via SFTP or the file manager.
3. **Configure `serverconfig.json`.** This is where you set world name, password, max clients, world type, and whether UPnP is enabled (turn it off on a hosted box — the host handles networking).
4. **Set the server port.** Vintage Story defaults to `42420` TCP+UDP. Most hosts pre-open this; you shouldn't need to touch it.
5. **Start the server from the panel.** Watch the console for the line indicating the world is ready.
6. **Share the IP.** Players connect via `Direct Connect` in the multiplayer menu using the server IP (or your free `yourserver.gamedns.net` subdomain).

If you're migrating a world from official hosting or single-player, copy the contents of your `Saves` folder into the server's save directory via SFTP, then point `SaveFileLocation` in `serverconfig.json` at it. Restart and you're back in your old world.

## Mods, Lag, and Server Settings That Actually Matter

Mods are the single biggest cause of "best vintage story server hosting" searches turning into "why is my server lagging" searches. Here's what to actually tune before throwing more RAM at the problem:

**Server-side settings in `serverconfig.json`:**

- `MaxClients` — defaults to 16. Lower it if you're under-provisioned.
- `MapSize` — smaller worlds = less chunk loading. A 500k² world is plenty for most groups.
- `SpawnCapMultiplier` and `CreatureHostilityMemoryTime` — drifters and creatures eat CPU. Reducing spawn pressure helps a lot on busy servers.
- `TickTime` — a lower value means smoother simulation but more CPU use; a higher value is the opposite.

**Mod hygiene:**

- Avoid stacking multiple mods that do the same thing (three weather mods, four food expansions, etc.).
- Client-side-only mods (like *OptiTime*) don't affect server load — don't worry about them.
- Server-side worldgen mods (*Better Ruins*, *RiverGen*, etc.) hit hardest during initial generation, then settle.
- Test new mods in a staging world before dumping them on your live server.

**Hardware red flags:**

If your server is lagging and `htop` (or the panel's resource view) shows RAM usage under 70% but CPU is pinned to one core, you have a single-core performance problem. No amount of RAM fixes that — you need a host running modern high-clock CPUs, which is why Ryzen 9 / Intel i9 class hardware matters for Vintage Story specifically.

## How ExtraVM Compares to Other Vintage Story Hosts

The Vintage Story Wiki maintains an unofficial list of third-party hosts, and a few names come up repeatedly in community discussions. Here's how ExtraVM stacks up against the most-mentioned alternatives:

| Host | Starting Price | Per-GB RAM | Locations | DDoS | Notable |
| --- | --- | --- | --- | --- | --- |
| ExtraVM | $6/mo (2 GB) | $3/GB (US/EU), $5/GB (SG/AU) | 8 worldwide | Included (enterprise) | Custom panel, in-house US support, Ryzen 9 / i9 |
| WinterNode | $3.98/mo (2 GB) | $1.99/GB | US, EU | Included | 45-day backups, no CPU limits |
| BisectHosting | ~$5/mo | Varies | 21 locations | Included | Popular, frequently out of stock |
| Host Havoc | $4/mo (8 slots) | Per-slot model | US, EU, others | Included | Unlimited RAM allotment, $0.50/slot |
| Akliz | Varies | Per-GB | US, EU, others | Included | Built-in ModDB installer |
| Nodecraft | Varies | Per-GB | Multiple | Included | 1-click ModDB install |

ExtraVM sits in the middle of the pack on raw price — WinterNode is cheaper per GB, BisectHosting has more locations — but it differentiates on hardware class (Ryzen 9 / i9 across the board), in-house US support rather than outsourced tier-1, and a custom control panel rather than a rebranded Pterodactyl install. If you've ever waited three days for a support ticket response from a host that outsources to a script-reading MSP, that last point matters more than $2/month.

## What Real Users Say

Community sentiment on ExtraVM for Vintage Story is thin but positive. The clearest signal is from r/VintageStory, where a user running a solo-plus-mods server reports $15/month for 5 GB RAM / 100 GB disk and CPU usage rarely above 15%. That's a single data point, but it matches the published pricing and the hardware claims.

On Trustpilot, ExtraVM LLC sits at 4.8/5 across reviews spanning VPS, game, and web hosting customers — the recurring themes are fast support response, stable uptime, and straightforward billing. The complaints that exist tend to focus on stock availability (some VPS tiers are frequently sold out, particularly the larger RAM configurations in Dallas) and the lack of a formal uptime SLA, which ExtraVM addresses by saying they credit affected customers directly rather than publishing a marketing SLA they consider misleading.

The honest read: ExtraVM isn't the cheapest, isn't the biggest, and doesn't have the most locations — but the hardware, support model, and pricing transparency are solid for someone who wants a Vintage Story server that just works without surprises.

## Discount Codes and Promotions

ExtraVM runs periodic promotions that show up on third-party coupon sites. The codes that appear consistently across multiple sources:

- **GAME30** — 30% off your first month on any game server plan
- **THR12** — another 30% off first-month game server code referenced in GitHub-hosted promo lists
- **25SWITCH** — 25% off your first month (general)
- **WHT30VPS** — 30% off lifetime for KVM NVMe VPS plans

These come from third-party coupon aggregators, not the official site, so treat them as "try at checkout" rather than guaranteed. ExtraVM's pricing is already flat per-GB with no hidden CPU or storage fees, so even without a code the math is straightforward.

To grab any of these at checkout, head to 👉 [the ExtraVM Vintage Story order page](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) and apply the code in the promo field.

## Final Verdict: Is ExtraVM the Best Vintage Story Server Hosting for You?

There's no universal "best" — it depends on your group size, location, and budget. But the decision tree is pretty simple:

**Pick ExtraVM if:**
- You want modern Ryzen 9 / i9 hardware and NVMe storage without paying premium-cloud prices
- You value in-house US-based support over the cheapest possible price
- You want a custom game panel with mod installer and backups rather than fighting with a generic panel
- You're in North America, Europe, or Singapore (best DDoS coverage and pricing)

**Look elsewhere if:**
- You're on a strict budget and want the cheapest per-GB rate — WinterNode at $1.99/GB is hard to beat on price
- You need 20+ locations for a globally distributed community — BisectHosting covers more regions
- You want unlimited RAM allotment on a per-slot model — Host Havoc's $0.50/slot pricing is unique

For most small-to-medium Vintage Story groups (4–16 players, a mod list of 20–80 mods, a world that'll live for months), a 4–6 GB ExtraVM plan at $12–18/month hits the sweet spot of performance, support, and not having to think about your server. The 5-day money-back guarantee means you can deploy, test, and bail if it doesn't feel right — no long-term risk.

If you're ready to pull the trigger, you can 👉 [start your Vintage Story server here](https://extravm.com/billing/store/game-server-hosting/vintage-story?aff=769) and have it online before you finish your coffee.

## Quick FAQ

**How fast is setup?** Instant after payment. You'll get panel credentials by email within seconds for credit card, PayPal, Apple Pay, Google Pay, or Alipay. Crypto payments may take longer to confirm.

**Can I add mods?** Yes. ExtraVM's game panel includes a mod installer, and you also get full SFTP access to upload mods manually. The official Vintage Story hosted servers don't allow mods — this is a key reason people switch to third-party hosts.

**Can I upgrade later?** Yes, anytime, via support ticket. Upgrades are prorated. Downgrades aren't possible due to technical limitations.

**Is there a refund?** Yes, 5-day money-back on all plans, fiat payment methods only (crypto refunds aren't processed). Transaction/refund fees may be deducted.

**Where are the servers?** Dallas, Los Angeles, Miami, New Jersey, Amsterdam, Singapore, Tokyo, Sydney. Pick the one closest to most of your players.

**Do I need DDoS protection?** Yes, and it's included at no extra cost on all US, EU, and Singapore locations. Sydney has basic local filtering only. Don't skip this — unprotected game servers get hit constantly.

**What payment methods work?** Visa, MasterCard, AMEX, Discover, China UnionPay, PayPal, Apple Pay, Google Pay, Alipay, plus dozens of cryptocurrencies including Bitcoin, Ethereum, and Litecoin.

**What if I'd rather run the server myself with full root access?** ExtraVM's KVM NVMe VPS line gives you full root on Linux/Windows/BSD with NVMe storage and DDoS protection. You'd install and run the Vintage Story server binary yourself. Plans start at $4.50/mo for 1 GB RAM — 👉 [check VPS availability here](https://extravm.com/billing/aff.php?aff=769&pid=22).
