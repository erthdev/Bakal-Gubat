# Log 03 (May 16, 2026)

— Defective in Transit — 

Not every log is about progress. Some logs are about hitting a wall, diagnosing why, and deciding to keep going anyway. This is one of those logs...

The ATX 24-pin to HP 6-pin harness adapter arrived. On paper it was the correct part. The product listing explicitly named the HP Elite 8200 as a compatible model. The connector physically fit the 6-pin socket on the motherboard. The 24-pin end seated correctly into the PSU output. Everything looked right. Nothing worked.

Upon powering on the system with the harness installed, the HP 8200 motherboard immediately displayed 4 blinking red diagnostic LEDs. On this specific motherboard the 4-blink code indicates a power delivery failure. The system was not receiving correct power through the main board connector despite the PSU being confirmed operational. The CPU 4-pin connector was functioning separately and the CPU heatsink fan was spinning, confirming that the CPU power rail was not the issue. The fault was isolated to the main board power delivery handled by the harness.

A clamp meter was used in DC voltage mode to probe the voltage on the motherboard side of the harness connector while the system was powered on. The reading was zero across all pins. The PSU was then tested standalone using the paperclip method, bridging the PS-ON green wire to a ground black wire on the 24-pin connector. The PSU fan spun up immediately and all voltage rails were re-verified. The 12V yellow rail, 5V red rail, and 3.3V orange rail all read within acceptable tolerance. The PSU was confirmed working correctly.

The conclusion from these two tests was definitive. The PSU was outputting correct voltage. Zero voltage was reaching the motherboard through the harness. The fault was inside the harness adapter itself, either a broken internal wire, a bad crimp connection, or incorrect internal pin mapping on the P2 signal side. The adapter was dead on arrival...

Additional troubleshooting was performed before reaching this conclusion to rule out all other possible causes. RAM was removed and reseated with a single stick in the primary slot only. All non-essential components including the WiFi PCIe card were removed from the board. The CMOS was cleared using the onboard jumper, moving it from pins 1-2 to pins 2-3 for 30 seconds before returning it to the original position. The CMOS battery was removed and reseated. The harness connector orientation was verified against the known HP 8200 6-pin motherboard pinout. None of these steps changed the result. The 4-blink fault code persisted and zero voltage continued to read on the motherboard side of the harness.

A return and refund request was filed with the seller with full technical documentation of the fault, the troubleshooting steps performed, and the meter readings confirming the defect. The item had been handled carefully and the fault was confirmed as a manufacturing defect and not user error.

This was a frustrating setback. A single defective cable stopped the first POST attempt cold. But the important result from this session is that the PSU is confirmed working, the board is confirmed to be responding to power inputs correctly based on the diagnostic LED behavior, and the fault has been fully isolated to one replaceable component. The build is not broken. One part was bad.

The harness will be replaced with a verified unit. In the meantime the build is moving forward on the physical side. With the PSU dimensions confirmed at 15 by 15 centimeters footprint and 8 centimeters height, and the motherboard dimensions confirmed at 27 by 21 centimeters, the open air wood frame measuring and layout planning can begin in parallel. The threaded rod column build does not depend on the harness being functional. Wood can be cut, shelves can be positioned, and standoff placement can be marked while the replacement harness is sourced.

The build continues.

## What happened in this log
* Received ATX 24-pin to HP 6-pin harness adapter
* Installed harness and powered on system for first POST attempt
* System displayed 4 blinking red LEDs indicating power delivery failure
* Probed motherboard side of harness with clamp meter on DC voltage mode, reading was zero across all pins
* Retested PSU standalone with paperclip method, all rails confirmed within acceptable tolerance
* Fault isolated definitively to internal defect inside the harness adapter
* Performed full secondary troubleshooting to rule out all other causes
* Single RAM stick tested, WiFi card removed, CMOS cleared, CMOS battery reseated, connector orientation verified
* All secondary troubleshooting confirmed no change, fault remained in harness
* Filed return and refund request with full technical documentation
* Confirmed PSU operational and board responding correctly to diagnostic inputs
* Decided to continue build on physical side while replacement harness is sourced

## Technical fault summary
* Symptom: 4 blink red LED diagnostic code on HP 8200 motherboard
* Code meaning: Power delivery failure on main board power connector
* PSU status: Confirmed operational, all rails within tolerance
* Harness status: Confirmed defective, zero voltage passing through to motherboard side
* Fault type: Internal manufacturing defect, broken wire or bad crimp or incorrect pin mapping
* Resolution: Return and refund filed, replacement unit to be sourced

## Current status
Harness return filed. PSU confirmed working. Board confirmed responsive. Physical build planning moving forward in parallel. First POST attempt pending replacement harness arrival.

## Next steps
* Source replacement harness from a verified supplier with confirmed HP 8200 compatibility reviews
* Begin measuring wood boards for shelf layout and threaded rod positioning
* Mark standoff hole positions on motherboard shelf
* Calculate threaded rod lengths based on full component stack height
* Plan PSU mounting position on bottom shelf with intake fan cutout
* Confirm M3 standoff fit against motherboard mounting holes once standoffs arrive
