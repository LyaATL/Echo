# Echo
Echo is a service that provides the following components:
- **Echo Mesh**: A plugin for the game *Final Fantasy XIV* leveraging Dalamud's framework to allow users to synchronize their mods with other connected clients. Mesh can simultaneously connect to multiple service instances, effectively replacing what is known as "shells."
- **Echo Service**: A cloud-native Go application that acts as a broker/server for Mesh to connect to.
- **Echo Sledgehammer**: A centralized service that synchronizes major offenders. This service enables `Echo Service` instances to share global client bans and file bans.

## Roadmap

These are either planned features or conceptual ideas.

### Echo Mesh
- [ ] Add support for implementing a plugin-native "shell-guard."
  - Ensure collections are correctly set up to prevent crashes caused by improper configurations. This may involve checking attempted syncs for faults or using hooks to resolve issues before they occur, while notifying the service of invalid sync attempts.

### Echo Service
- [ ] Add support for opting in, instead of syncing everything by default. It remains the host's responsibility to ensure that a ban is valid.
  - Pedophilia is, and always will be, subject to a global ban. This is currently the only exception.
- [ ] Add support for implementing a central "shell-guard."
  - Ensure collections are correctly set up to prevent crashes caused by improper configurations.

### Echo Sledgehammer
- [ ] Add support for opting in, instead of syncing everything by default. It remains the host's responsibility to ensure that a ban is valid.
  - Pedophilia is, and always will be, subject to a global ban. This is currently the only exception.
- [ ] Add support for appeals.
- [ ] Add an administration panel to allow moderators/administrators to manage bans.
- [ ] Add support for custom ban reasons.

## Disclaimer

This project, **Echo Mesh**, **Echo Service**, **Echo Sledgehammer**, is an independent work and has **no affiliation, connection, or association with Mare Synchronos** or its developers.  
It does not use, depend on, or share any code or intellectual property from Mare Synchronos.

Echo Service is intended as a standalone learning and development project.  
Any resemblance in functionality or naming is purely coincidental and not indicative of any partnership, endorsement, or continuation of Mare Synchronos.

This software is provided **"as is"**, without a warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement.  
Use of this software is at your own discretion and risk.
