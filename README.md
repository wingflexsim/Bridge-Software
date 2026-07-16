# Wingflex Bridge Software

Wingflex Bridge is the standalone software application that connects Wingflex hardware with supported flight simulation software.

It acts as the communication layer between Wingflex devices and the simulator, allowing compatible hardware to send inputs, receive simulator data, synchronize displays, and provide a more realistic flight deck experience.

Wingflex Bridge is designed to support Wingflex products across supported simulator platforms, aircraft, and add-ons. Compatibility may vary depending on simulator version, aircraft implementation, firmware version, and third-party add-on behavior.

## How to Use

Wingflex Bridge does not require installation.

To use Wingflex Bridge:

1. Go to the **Releases** page of this repository.
2. Download the latest standalone `.exe` file.
3. Open the `.exe` file to launch Wingflex Bridge.
4. Connect your Wingflex hardware and start your supported flight simulator.

## System Requirements

Wingflex Bridge requires the **Microsoft Visual C++ 2013 Redistributable** to run.

If the application does not start, or if Windows reports a missing runtime DLL, please install the Microsoft Visual C++ 2013 Redistributable and try again.

No additional installation is required for Wingflex Bridge itself.

## What Wingflex Bridge Does

Wingflex Bridge helps Wingflex hardware communicate with flight simulation software by:

* Detecting and managing connected Wingflex devices
* Sending hardware inputs to the simulator
* Receiving simulator data for displays, indicators, LEDs, and other device functions
* Supporting aircraft-specific logic where available
* Providing firmware update and device management features
* Improving compatibility across supported simulators and add-ons

## Supported Use Cases

Wingflex Bridge may be used with supported Wingflex hardware products, including but not limited to:

* DAP
* FCU
* EFIS
* RMP
* Overhead Panel
* Other Wingflex flight deck hardware

Support may depend on the product, firmware version, Bridge version, simulator version, and aircraft or add-on being used.

## Reporting Bugs and Requesting Features

Please use GitHub Issues or the Wingflex Discord forum to report Bridge Software bugs, request aircraft or add-on compatibility, or suggest Bridge features and improvements.

### Bug Report Generator Required

All Bridge Software bug reports must be created using the **Wingflex Bug Report Generator**:

https://skylarkning.github.io/wingflex-bug-report-generator/

The generator collects the required technical information and produces a consistently formatted report for faster triage, clearer communication, and easier bug indexing.

After generating the report, paste the generated Markdown into either:

* A new GitHub Issue in this repository, or
* The Wingflex Discord **#bridge-bug-tracker** channel

Submit each bug in **one location only**. Do not post the same report to both GitHub and Discord.

**Bug reports submitted without using the generator will be deemed invalid and closed.**

Discord invite:
https://discord.com/invite/hB9faWgd3q

Before posting, please search first. If the same issue or request already exists, reply there instead of creating a duplicate.

These reporting channels apply only to Bridge Software issues. If you believe your issue is hardware-related, please contact Wingflex directly.

## Important Notes

All posts go through Wingflex triage. Wingflex staff will review reports and add or update tags based on status, category, priority, affected product, user impact, and technical feasibility.

Submitting a request does not guarantee that it will be accepted, planned, or implemented.

Aircraft compatibility can be complex. Some issues may be caused by third-party aircraft behavior, SimConnect or LVAR limitations, Microsoft Flight Simulator updates, aircraft updates, or changes outside the control of Wingflex Bridge. Compatibility may also break after simulator or aircraft updates.

## Status Tags

Tags are managed by Wingflex staff.

| Tag          | Meaning                                                             |
| ------------ | ------------------------------------------------------------------- |
| Need Info    | More details are needed                                             |
| Confirmed    | The issue has been reproduced or verified                           |
| Under Review | The report or request is being evaluated                            |
| Planned      | Accepted for a future update                                        |
| WIP          | Currently being worked on                                           |
| Fixed        | Implemented or in testing                                           |
| Released     | Included in a public release                                        |
| Duplicate    | Already tracked elsewhere and may be deleted after 72 hours         |
| Not Planned  | Not planned or outside Bridge control. May be marked as “Won’t Fix” |

## Priority Definitions

Priority labels are assigned and updated by Wingflex staff during triage. They indicate the urgency and order in which an issue or request may be addressed. Priority is based on user impact, affected scope, reproducibility, available workarounds, technical feasibility, and roadmap fit.

The examples and estimated resolution targets below are provided as general guidance. Actual timelines may change depending on engineering capacity, technical complexity, external dependencies, simulator or aircraft updates, and changes to the Wingflex development roadmap. The estimated timeline begins after an issue has been confirmed and assigned a priority.

| Priority | Definition | Estimated Resolution Target | Examples |
| -------- | ---------- | --------------------------- | -------- |
| **Priority 1** | **Critical. Must be fixed as soon as possible. Do not use for most issues. Priority 1 can only be assigned by Wingflex staff.** A core function is unavailable, a release causes a major regression, or the issue has widespread and severe user impact. | **Current release cycle.** A hotfix will be provided as soon as reasonably possible. | Bridge crashes on startup for most users after an update; supported Wingflex devices cannot connect or exchange simulator data; a Bridge-managed firmware update prevents normal device operation. |
| **Priority 2** | **Important and should be addressed.** The issue has meaningful impact but lower urgency, affects a narrower group of users, or has a reasonable workaround. | **Within the next one or two version updates, typically one to two months.** | Dual MCDU operation does not work while a single MCDU remains usable; an FCU or EFIS display remains active after cold and dark but can be cleared by restarting the Bridge or device; a major function is broken only for one supported aircraft or add-on version. |
| **Priority 3** | **Valid issue or request on the backlog.** It may be promoted to Priority 2 if capacity allows, user impact increases, or the request becomes more relevant to the product roadmap. | **Up to six months.** | Add DAP-500 compatibility for the COWS DA40 or DA42; support an additional less-common aircraft or add-on; improve a device-management workflow that does not block normal operation. |
| **Priority 4** | **Low priority.** The issue is minor, uncommon, cosmetic, or unlikely to receive active engineering work in the near term. | **At least six months.** No specific release commitment is provided. | Minor alignment or spacing issues in the Bridge interface; a small display or LED behavior difference that does not affect operation; a typo or label inconsistency. |
| **Priority 5** | **Unlikely to be implemented.** The request is outside the scope of Wingflex Bridge, has poor roadmap fit, is disproportionately complex, or is likely to be marked **Not Planned** or **Won’t Fix**. | **No estimated resolution time.** The issue or request may not be implemented. | Support for an unsupported or discontinued simulator platform; behavior that a third-party aircraft does not expose through available simulator APIs; a major custom integration for one-off unsupported hardware. |

**Priority 1 is reserved for severe, high-impact failures. A problem affecting only an unsupported aircraft, simulator, add-on, or hardware configuration will not normally qualify as Priority 1.**

**Estimated resolution targets are not guarantees. Assignment of a priority does not guarantee that an issue will be resolved within the stated period or included in a particular release.**

## What to Include in a Bug Report

Use the required **Wingflex Bug Report Generator** to prepare your report:

https://skylarkning.github.io/wingflex-bug-report-generator/

The generator will prompt you for the required product, Bridge version, firmware version, simulator, aircraft or add-on, issue description, reproduction steps, expected result, actual result, and supporting media or logs.

Provide clear and repeatable steps. Attach screenshots, logs, and preferably a video showing the issue whenever available. Reports without enough information to reproduce or investigate the problem may be marked **Need Info** or closed.

## What to Include in a Feature or Compatibility Request

For feature requests or aircraft/add-on compatibility requests, please include:

```text
Request:
Affected Product:
Simulator/Aircraft:
Use Case:
Expected Behavior:
References:
```

Please explain what you are trying to achieve and how the requested feature or compatibility improvement would help.

## One Issue Per Post

Please keep one issue or request per GitHub Issue or Discord forum post so Wingflex staff can track status clearly.

If you have multiple unrelated bugs or requests, please create separate posts for each one.

## Hardware Support

This repository is for Wingflex Bridge Software only.

If your issue appears to be related to hardware damage, shipping damage, physical buttons, connectors, power, displays, cables, or other non-software problems, please contact Wingflex directly instead of opening a Bridge Software issue.

## Disclaimer

Wingflex Bridge compatibility depends on simulator APIs, aircraft implementations, add-on behavior, firmware versions, and software updates. Some behaviors may be outside Wingflex’s direct control.

Wingflex will review reports and requests, but not every request can be accepted or implemented.

