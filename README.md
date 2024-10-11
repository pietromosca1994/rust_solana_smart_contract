#
## Introduction
Sample Rust program for Solana based on [Anchor Framework](https://solana.com/docs/programs/anchor)
Here some useful resources:
- [Program Structure](https://solana.com/docs/programs/anchor/program-structure)
- [Program Examples](https://solana.com/docs/programs/examples)
- [Anchor by Example](https://examples.anchor-lang.com/docs/onchain-voting)


1. Install the required toolchain as described in [Installation](https://solana.com/docs/intro/installation)
2. 

## Testing
### Local Environment
1. Start a Local Solana Cluster:
``` bash 
solana-test-validator
```
In a different prompt 
``` bash 
solana config set --url http://127.0.0.1:8899
```

2. Deploy 
- 2.1 Configure the Anchor Project in Anchor.toml
```toml
[clusters]
localnet = "http://127.0.0.1:8899"
```
- 2.2 Build the Anchor Program
``` bash
anchor build
```
- 2.3 Deploy the program locally 
``` bash
anchor deploy --provider.cluster localnet
```

3. Test
``` bash 
anchor test
```

### Devnet Environment

## References
- [Account Constraints](https://www.anchor-lang.com/docs/account-constraints)
- [Account Types](https://www.anchor-lang.com/docs/account-types)