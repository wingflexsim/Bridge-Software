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

Discord invite:
https://discord.com/invite/hB9faWgd3q

Before posting, please search first. If the same issue or request already exists, reply there instead of creating a duplicate.

This forum only applies to Bridge Software issues. If you believe your issue is hardware-related, please contact Wingflex directly.

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

## What to Include in a Bug Report

For bugs, please include the following information:

```text
Product: DAP / FCU / EFIS / RMP / Overhead / Other
Bridge Version:
Firmware Version:
Simulator: MSFS 2020 / MSFS 2024
Aircraft/Add-on:
Issue:
Steps to Reproduce:
Expected Result:
Actual Result:
Screenshots/Videos/Logs:
```

Please provide clear steps to reproduce the issue. Screenshots, videos, and logs are very helpful when available.

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
