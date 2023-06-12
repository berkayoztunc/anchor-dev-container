

# Proje kurma ve test çalışması için docker file 

## içerisinde 

- solana-cli
- solana-test-validator
- anchor-cli
- rustup
- rustc
- cargo
- nodejs@18
- npm
- yarn


## Nasıl kullanılır 
Git üzerinden repoyu klonlayın
```bash
git clone https://github.com/berkayoztunc/anchor-dev-container
```

Sonra vs code üzerinden `cmd+shift+p` ile komut paletini açın ve `Remote-Containers: Open Folder in Container` seçiyoruz. Sonrasında VS code otomatik olarak docker container'ını oluşturup içerisine giriyor.


## Solana CLI komutları

Solana cüzdan oluşturma
    
```bash
solana-keygen new
```

Solana Airdrop isteme
```bash
solana airdrop 2
```

Solana ağı değiştirme
```bash
solana config set --url https://api.devnet.solana.com
```
Solana cüzdan adresi görüntüleme
```bash
solana address
```
Solana cüzdan bakiyesi görüntüleme
```bash
solana balance
```
Solana config görüntüleme
```bash
solana config get
```

## Anchor CLI komutları

Anchor proje oluşturma
```bash
anchor init <project-name>
```
Anchor proje build etme
```bash
anchor build
```
Anchor proje test etme
```bash
anchor test
```
Anchor proje deploy etme (! bu noktada biraz fazla SOL'a ihtiyaç duyuluyor o yüzden airdop yapmak gerekebilir !)
```bash
anchor deploy
```

