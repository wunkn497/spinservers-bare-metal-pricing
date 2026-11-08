# Cheap Bare Metal Server Hosting: What $79 a Month Buys, Which SpinServers Plan Fits Your Load, and the Add-Ons That Raise the Bill

Cheap bare metal server hosting starts at $79 a month if you want a current-generation Xeon, 32GB of ECC memory and an NVMe drive rather than a decade-old spinning disk. That is the entry price SpinServers lists for its Intel Xeon E3-1280 v5 in Dallas on monthly billing, and the box includes 30TB of transfer on a 10Gbps port instead of the 1Gbps link most budget providers cap you at.

The same search term also turns up a €4.99 Dedibox and a €1,546.77 enterprise machine. Both are real, both are bare metal, and neither tells you much about what you should pay. What follows is the current SpinServers lineup with prices, the parts of a bare metal invoice that are not in the headline number, and the point at which a cheaper option is genuinely the better buy.

> **Most readers should start here:** Intel Xeon E3-1280 v5 in Dallas at **$79.00/mo** on monthly billing. Four cores and eight threads at 3.7GHz, 32GB DDR4 ECC, 1TB M.2 NVMe, 30TB of monthly bandwidth on a 10Gbps port, one IPv4, auto-provisioned. It covers a busy website, a VPN endpoint, a game server or a stack of containers. 👉 [Check the current Dallas configuration and price](https://bit.ly/Spinservers)

## The SpinServers lineup as listed in late September 2026

Four configurations appear across the Dallas and San Jose store pages with published monthly rates. Every one of them is billed monthly, so there is no long contract to sign and no prepay discount to chase either.

| Plan (location) | CPU | RAM / storage | Network | Price | Order |
| --- | --- | --- | --- | --- | --- |
| Intel Xeon E3-1280 v5 (Dallas) | 4 cores / 8 threads, 3.7GHz turbo | 32GB DDR4 ECC / 1TB M.2 NVMe | 30TB on 10Gbps, 1 IPv4 | $79.00/mo, monthly | [Order the Dallas E3-1280 v5](https://bit.ly/Spinservers) |
| Intel Xeon E3-1280 v5 (San Jose) | 4 cores / 8 threads, 3.7GHz turbo | 32GB DDR4 ECC / 1TB M.2 NVMe | 30TB on 2×10Gbps, 1 IPv4 | $79.00/mo, monthly | [Order the San Jose E3-1280 v5](https://bit.ly/Spinservers) |
| Dual Intel Xeon Gold 6148 (Dallas) | Dual socket, 40 vCPU | 256GB / 3.8TB SSD | 30TB | $235.00/mo, monthly | [Order the dual Gold 6148](https://bit.ly/Spinservers) |
| Dual Intel Xeon Platinum 8173M (Dallas) | Dual socket, 56 vCPU | 512GB / 7.7TB SSD | 30TB | $390.00/mo, monthly | [Order the dual Platinum 8173M](https://bit.ly/Spinservers) |

A few things the table does not show. Inventory rotates: the store listed 43 dedicated configurations at the time of that check, so the exact SKUs available this week may differ from the four above. Both locations advertise 30TB of monthly transfer and one included IPv4 address, and the Dallas machines are marked "Ready To Go - Auto-Provisions". San Jose goes wider on network hardware, shipping two 10Gbps ports rather than one.

The secondary table matters more than it looks, because the San Jose catalogue reaches further down and further sideways than the four priced rows suggest:

| San Jose configuration | Cores / threads | RAM | Storage |
| --- | --- | --- | --- |
| Xeon, 2.6GHz base | 12 / 24 | 64GB DDR3 ECC | 1×240GB SSD |
| Xeon, 1.8GHz base | 16 / 32 | 64GB DDR4 ECC | 1×1.6TB SSD |
| Dual Xeon E5-2630L v3 (SJC-202) | 16 / 32 | 64GB DDR4 ECC | 1×1.6TB SSD |
| Xeon, 1.8GHz base | 24 / 48 | 64GB DDR4 ECC | 1×1.6TB SSD |
| Xeon, 1.8GHz base | 16 / 32 | 256GB DDR4 ECC | 2×1.6TB SSD, hardware RAID with cache |
| Xeon, 2.1GHz base | 32 / 64 | 512GB DDR4 ECC | 2×3.84TB SSD, RAID with battery-backed cache |

Notice the DDR3 line. A 12-core box with 64GB of DDR3 will be the cheapest thing on the page when it is in stock, and it is fine for backups, archival storage or a lab. It is a poor fit for a latency-sensitive database, and the listing does not shout about the memory generation.

## What counts as cheap in this category

Cheap spans roughly a 300-fold range depending on which provider you land on, and the numbers are quoted in different currencies and billing periods, which is why the comparison is so messy.

Scaleway publishes the lowest entry point of any provider reviewed here: Dedibox dedicated servers **starting from €4.99/month** across almost 100 hardware configurations, and its Elastic Metal line **starting from €27.99/month or €0.077/hour**. Those are "starting from" figures on the vendor's own page in euros, and the page does not state whether tax or renewal terms change them. At the other end, InMotion Hosting lists its Commercial Class range at **€270.69/mo** for the CC-1000 up to **€1,546.77/mo** for the CC-4000, with three different prices shown for each plan and no explanation of which billing cycle or data centre each one refers to.

HorizonIQ sits in between on paper but publishes no prices at all. Its three tiers (Essential, Advanced, Ultimate) are described by configuration range only: Advanced covers dual Xeon E5 and Silver chips with 16 to 28 cores and 64 to 128GB of RAM, Ultimate moves to Xeon Gold and AMD EPYC with up to 36 cores and 192GB. Nineteen ready-to-deploy configurations sit in its online store; the rest are build-to-order.

Against that backdrop, $79 for a 4-core Xeon with 32GB of DDR4 ECC, a 1TB NVMe drive and 30TB of transfer is inexpensive without being the cheapest thing that exists. You are paying roughly the price of a mid-range cloud instance for hardware nobody else touches.

## Where the bill grows after the headline price

Bare metal pricing is not one number. It is hardware plus everything the provider chose not to bundle, and the add-ons are where budget plans stop being budget.

**Operating system licensing.** A bare metal server has no hypervisor underneath it, so the OS is yours to install and, in the case of Windows, yours to license. Windows Server is typically a separate line item; Atlantic.Net notes that customers can either procure licences themselves or buy them through the provider. If your stack runs on Linux, this cost disappears entirely, which is one reason the $79 plan is realistically a $79 plan for most buyers.

**Bandwidth overage.** HorizonIQ's model is a useful benchmark for how providers structure this: 10TB of outbound traffic included per server, inbound transfers free, and anything beyond the contracted amount billed by actual usage. SpinServers advertises 30TB, three times that allowance, but the store listings do not spell out whether inbound counts against it or what the per-GB rate is once you exceed it. Ask before you push a backup or a video workload through the pipe. 👉 [See the current bandwidth terms on the SpinServers listings](https://bit.ly/Spinservers)

**DDoS protection.** Frequently an optional, separately priced service rather than a default. Atlantic.Net lists it as an "optional configurable service", and providers that include it usually say so loudly. Confirm what mitigation comes with the base plan.

**Contract length.** Atlantic.Net offers "generous discounts" for one, two and three-year terms, which is the standard trade: commit longer, pay less per month, lose the ability to walk away. SpinServers' published rates are monthly, so you keep the flexibility and forgo the discount. That is a fair exchange for a first purchase.

**Provisioning time.** "Instant" is a marketing word more often than an operational guarantee. Atlantic.Net's own FAQ says setup time depends on configuration, availability and custom requirements, and suggests a dedicated cloud host if you truly need instant. SpinServers marks its Dallas stock as auto-provisioning, which is a stronger signal than most, but a custom San Jose build with a hardware RAID controller is not going to appear in five minutes.

**Drive type.** NVMe is not automatically standard across the industry. HorizonIQ's ready-to-deploy servers all ship with a mirrored pair of 2×480GB SSDs, with NVMe available only on custom orders. The SpinServers entry plan includes a 1TB M.2 NVMe drive at $79, which is a genuine advantage at that price.

## Matching a plan to a workload

Pick by what the machine has to hold in memory, not by core count, because cores are cheap and RAM is not.

**A website, a VPN, a game server, a handful of containers.** The E3-1280 v5 at $79. Four fast cores at 3.7GHz with a 1TB NVMe drive will outperform a 16-core box on a mechanical disk for anything latency-bound, and the 10Gbps port means you will never blame the network. Choose Dallas or San Jose by where your users are; the two locations are the entire footprint.

**Virtualisation, a growing database, a dozen services on one box.** Move to the dual Xeon Gold 6148 at $235. Forty vCPUs and 256GB of RAM is the point where running KVM or Proxmox on bare metal starts to make sense, since the hypervisor overhead you removed by renting physical hardware now gets spent on your own guests instead.

**In-memory databases, analytics, HPC, large model inference on CPU.** The dual Platinum 8173M at $390 gives 512GB of RAM and 7.7TB of SSD. That is memory-bound territory: if your working set does not fit in 256GB, no amount of cores will save the query plan.

There is no GPU in any of the listed configurations. If your workload needs one, this is not the catalogue for it and you should be looking at a GPU-specific provider.

## Who should not rent bare metal here

Two groups are better served elsewhere, and neither should feel bad about it.

The first is anyone with spiky demand. Scaleway's Elastic Metal bills at **€0.077/hour**, and a seasonal business that needs twelve cores in December and two in February will spend less on hourly billing than on eleven months of an idle $235 server. Bare metal rewards steady load; it punishes the rollercoaster.

The second is anyone who needs a managed stack. Bare metal gives you root on physical hardware and nothing else: no automated backup regime, no managed failover, no control panel. One independent review of SpinServers flags exactly this, noting limited published detail on backup, disaster recovery and redundancy beyond power and network. If you want someone else to own the patching and the backups, a managed VPS or a cloud instance is the honest answer, even at a higher monthly rate.

Geography is the third constraint. Dallas and San Jose are the only two locations, so if your users or your compliance requirements sit in Europe or Asia, latency and data residency both become problems that no price cut solves.

## Four things to confirm before you pay

1. **Memory generation and drive type on the exact SKU.** The San Jose list mixes DDR3 and DDR4, and the price difference between two similarly named boxes can come down to memory that is a decade apart.
2. **How the OS gets installed and what Windows costs.** Bare metal has no pre-installed hypervisor, so you are installing the OS yourself or paying for a licence and an image.
3. **Whether 30TB counts inbound and outbound, and what the overage rate is.** The allowance is generous; the penalty clause is what you need to read.
4. **Setup fees, cancellation terms and the provisioning window.** None of these appear in the headline price, and all three affect the real first-month cost.

If you want a single rule: a steady workload that fits in 32GB goes on the E3-1280 v5 at $79; anything that needs more than 128GB of RAM or more than eight threads in one box moves up to the Gold 6148; memory-bound work goes to the Platinum 8173M. Everything else, from a two-week test to a seasonal traffic spike, belongs on hourly billing somewhere else.

👉 [Compare the current Dallas and San Jose bare metal listings](https://bit.ly/Spinservers)
