# Echo
Echo is a service providing the following:
- Echo Mesh: A plugin for the game FFXIV leveraging Dalamud's framework to allow people to sync their mods towards other connected clients. Mesh has the power to simultaneously connect to multiple service instances at once. Effectively replacing something known as "sync shells".
- Echo Service: A cloud-native Go application that acts as a broker/server for mesh to connect too.
- Echo Sledgehammer: A centralized service that synchronizes heavy offenders. This service allows `Echo Service` instances to sync global client bans and file bans.

## Roadmap

These are either planned ideas or rough ideas.
### Echo Mesh
- [ ] Add support to implement a plugin native 'shell-guard'.
  - Ensure collections are correctly setup, removing crashes due to poor setups. Either by checking the attempted sync on faults or utilizing hooks to 'fix' crashes before they happen, reacting upon this bad sync towards the service.

### Echo Service
- [ ] Add support to opt-in instead of syncing everything. It's still the responsibility of the host to make sure the ban is valid.
  - Pedophilia is and always will be a global ban. This will currently be the only exception.
- [ ] Add support to implement a central 'shell-guard'.
  - Ensure collections are correctly setup, removing crashes due to poor setups.

### Echo Sledgehammer
- [ ] Add support to opt-in instead of syncing everything. It's still the responsibility of the host to make sure the ban is valid.
  - Pedophilia is and always will be a global ban. This will currently be the only exception.
- [ ] Add support for appeals
- [ ] Add a panel to manage bans for moderators/administrators
- [ ] Add support for custom ban reasons
