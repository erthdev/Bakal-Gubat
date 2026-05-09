# Log 01 (May 9, 2026)

No hardware was touched today. What happened today was a full planning and design session, and somewhere in the middle of it the entire project changed shape. Not in a bad way. In the way that happens when you start actually thinking clearly about what you are building and why.

Let me back up a little.

This project started as a cyberdeck build. The HP Compaq 8200 SFF was going to be stripped down, fitted with a battery, a Pico PSU, a custom keyboard, and crammed into a compact portable enclosure. The dream was a portable hacker-style machine you could carry anywhere and set up on any desk. That dream is not dead tho, it is just paused. Because somewhere along the way I realized the HP 8200 motherboard is 27 by 21 centimeters, runs a full desktop CPU with a 65 to 95 watt TDP, and needs a proper ATX power chain with proprietary HP adapter connectors just to boot. That is not a cyberdeck. That is a desktop trying very hard to pretend it is something else:(

So the cyberdeck plan got shelved. The mini PC route is the smarter play for that project and it will come back when the budget allows.

What the HP 8200 became instead is something more interesting. An open-air wood PC. Inspired by a Reddit build using threaded rod columns, layered wood shelves, a copper IO panel, and fully exposed components. The aesthetic direction is dark and moody dark hardwood, metal rods, vines crawling up the frame, and the warm glow of components visible from every angle. The project now has a name. Bakal-Gubat. Steel Forest in Filipino. It felt right the moment I said it.

Today the architecture got locked in. The PSU sits at the bottom. The motherboard mounts vertically on its side like in the reference build. The threaded rods run floor to ceiling holding the whole structure together. Two 90mm intake fans push air across the board. The CPU cooler exhausts upward and out. No enclosure fighting the airflow. No panels blocking the wood grain. Everything visible, everything intentional.

There is still a lot to source. A generic ATX 400 to 500 watt PSU with HP proprietary adapter harness for the P1, P2, and P3 connectors. A low-profile GPU when the budget allows. Longer threaded rods once the final dimensions are measured. But the direction is clear and the parts I already have are enough to start building the frame.

This is the log where the project found its identity.

## What happened today
* Paused the cyberdeck build - mini PC is the better approach for that project
* Pivoted the HP 8200 to an open-air wood PC build
* Locked in the open-air threaded rod column design inspired by a Reddit reference build
* Named the project Bakal-Gubat - Steel Forest in Filipino
* Finalized cooling architecture - 90mm intake fans, LGA1155 CPU cooler, open-air exhaust
* Planned the vertical motherboard mounting orientation
* Inventoried all available wood boards and measured the motherboard
* Created the GitHub repository structure, README, license, and gitignore
* Began build log documentation

## What I can learn from this build

This is the part that matters long term. This build is not just about making something that looks good. Every problem you solve here teaches you something real. Old hardware does not retire. It teaches.

## Current status
Project identity confirmed. Repository created. Build direction locked. Ready to source the PSU and begin physical construction.

## Next steps
* Source generic ATX 400–500W PSU with HP adapter harness
* Measure PSU dimensions once purchased
* Calculate final threaded rod lengths based on component stack heights
* Cut and finish wood boards
* Begin threaded rod frame assembly
* Refresh CPU thermal paste before mounting cooler
* Test POST with new PSU and adapter harness before closing anything up
