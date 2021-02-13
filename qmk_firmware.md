---
layout: page
title: QMK Firmware
---

QMK Firmware runs on a keyboard and is responsible for translating key presses into scancodes. It is written in C and distributed under the GNU GPL. While I do contribute code to the firmware itself my primary role is to act as TPM, helping to coordinate work where needed and to entire that the administrivia required to keep the project moving happens.

## Technical Contributions

My first contribution to QMK was a feature called [Grave Escape](https://docs.qmk.fm/#/feature_grave_esc). This allows you to share the Escape key with the Grave/Tilde key, a very useful feature on compact keyboards. I have contributed several other small features, but my most substantial contributions to date are [LED Matrix](https://docs.qmk.fm/#/feature_led_matrix) and [Direct LED Matrix](https://github.com/qmk/qmk_firmware/pull/7026). These are features which allow keyboard designers to control a matrix of single-color LEDs, either using an LED IC or wiring the matrix directly to the MCU.

## Technical Project Management

In a volunteer driven project you don't have traditional TPM's. You have no stick, only carrot, and this limits the approaches you can take. However, like any other software project we still have relationships to manage, projects to drive, and administrivia to attend to.

When QMK was smaller we ran monthly meetings to discus and progress QMK business. These meetings were held over voice chat and generally consumed 1-2 hours per month. As QMK grew and our Collaborators spanned more timezones finding time to hold these meetings became more difficult. We were having great difficulty with scheduling meetings and getting all of our business done when the pandemic hit and made scheduling a time impossible for several collaborators. To address this challenge I setup Discourse and we now handle decision making and voting asynchronously. This allowed us to continue growing the number of Collaborators without locking anyone out of discussions and decision making.

We also have an ongoing relationship with [VIA](https://caniusevia.com/), which is a graphical keyboard configuration tool built on top of QMK. I have played ambadassor many times, helping to shepperd changes each team needed that the other team was resistant to.

## Bylaws and Code of Conduct

QMK's first bylaws were written in May 2017. It was a collaborative effort between myself, Jack Humbert, and Erez Zukerman. As part of that process I wrote the first version of our Code of Conduct. While we could have adopted the Contributor Covenant (and if I were starting a project today that's exactly what I'd do) we wanted to emphasize kindness in our Code of Conduct.

Since enacting the CoC we have had to enforce it a few time, but we are fortunate that our community is largely self-regulating. I think the simplicity and straightforwardness of our Code of Conduct contributes to that dynamic.

## Data Driven QMK

Data Driven QMK is a project I have been working on to make QMK more flexible, maintainable, and scalable. It involves removing data from source code files and into structured JSON. End users and developers will be able to modify and consume this structured data using sophisticated tooling, making it easier to maintain keyboards. As part of this process I wrote a [Python CLI](qmk_cli.md) and tooling to generate source code, documentation, and other files from a JSON source of truth.

## Documentation

Over the years I have taken on several projects to improve our documentation. Like any community documentation effort it is a challenge to keep documentation organized as it organically grows. Additionally, in a project as complex and technical as QMK onboarding new users and developers is a continual challenge. To address that challenge over the years I have taken on several projects:

* Organizing the documentation in a more logical way
* Migrate from Github Wiki to Gitbook
* Migrate from Gitbook to Docsify
* Writing developer focused documentation:
    * [Understanding QMK](https://docs.qmk.fm/#/understanding_qmk)
    * [QMK Contributor's Guide](https://docs.qmk.fm/#/contributing)
    * [Breaking Changes](https://docs.qmk.fm/#/breaking_changes)
    * [C Coding Conventions](https://docs.qmk.fm/#/coding_conventions_c)
    * [Python Coding Conventions](https://docs.qmk.fm/#/coding_conventions_python)
    * [Keyboard Guidelines](https://docs.qmk.fm/#/hardware_keyboard_guidelines)
    * [Documentation Best Practices](https://docs.qmk.fm/#/documentation_best_practices)
* Writing user focused documentation:
    * [QMK Tutorial](https://docs.qmk.fm/#/newbs).
