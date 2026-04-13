## Architecture

- ### Client side

  - `Next.js` (React framework)
  - `pnpm` (package manager)
  - deploy on `Vercel`

- ### Onchain side

  - `Anchor` (Rust framework)
  - `cargo` (package manager)
  - deploy on `Solana`

- ### JSON RPC layer

  - `@solana/web3.js` (sdk for js)

![alt text](APPLICATION_ARCHITECTURE.png)

## Development Flow

1. ### Create branch

- Follow [git-flow](https://datasift.github.io/gitflow/IntroducingGitFlow.html)
- Branch name format:
  - **<git_flow_prefix>/<client | onchain>/<task_description>**
- Examples
  - feature/client/add-wallet-provider
  - build/onchain/setup-cargo

2. ### Commit and push your changes

- `husky` - for pre-commits hooks
- Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.4/)
- Examples
  - feat: add language selection
  - chore: cleanup code

3. ### Create MR and merge to develop

- push branch into repo
- create Merge Request
- do code review by YOURSELF
- request code review from TEAM MEMBER
- request code merge from TEAM LEAD
