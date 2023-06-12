# Docker file for project setup and testing
- Included:
- solana-cli
- solana-test-validator
- anchor-cli
- rustup
- rustc
- cargo
- nodejs@18
- npm
- yarn

## Clone the repository from Git:

```bash
git clone https://github.com/berkayoztunc/anchor-dev-container
```
Then, open the command palette in VS Code with `cmd+shift+p` and select "Remote-Containers: Open Folder in Container". VS Code will automatically create the Docker container and enter into it.

## Solana CLI commands
Creating a Solana wallet:

```bash
solana-keygen new
```
Requesting Solana Airdrop:

```bash
solana airdrop 2
```
Changing the Solana network:

```bash
solana config set --url https://api.devnet.solana.com
```
Viewing the Solana wallet address:

```bash
solana address
```
Viewing the Solana wallet balance:

```bash
solana balance
```
Viewing the Solana config:

```bash
solana config get
```
## Anchor CLI commands
Creating an Anchor project:

```bash
anchor init <project-name>
```
Building an Anchor project:

```bash
anchor build
```
Testing an Anchor project:

```bash
anchor test
```
Deploying an Anchor project (Note: This step requires a sufficient amount of SOL, so an airdrop may be necessary):

```bash
anchor deploy
```