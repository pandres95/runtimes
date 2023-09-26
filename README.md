# Work In Progress

Do not modify the `relay/` or `system-parachains/` folder. They are currently read-only.

## Folder Structure

<!-- tree -I 'target' -d -L 3 -->
```pre
.
├── relay
│   ├── kusama
│   │   ├── constants
│   │   └── src
│   └── polkadot
│       ├── constants
│       └── src
└── system-parachains
    ├── asset-hubs
    │   ├── asset-hub-kusama
    │   └── asset-hub-polkadot
    ├── bridge-hubs
    │   ├── bridge-hub-kusama
    │   └── bridge-hub-polkadot
    └── collectives
        └── collectives-polkadot
```

## Approval rights

The approval rights are configured in [`review-bot.yml`](.github/review-bot.yml). The rights are configured as:

- All files in `.github` require two approvals from fellow members of rank 4 or higher.
- `CHANGELOG.md`, `relay/*` or `system-parachains/*` require four approvals from fellow members of rank 3 or higher.
- All other files require the approval from one fellow member of rank 2 or higher.

The review-bot uses the on-chain identity to map from a github account to a fellowship member. This requires that each fellowship member add their github handle to their on-chain identity. Check [here](docs/github-on-chain-identity.md) for instructions.
