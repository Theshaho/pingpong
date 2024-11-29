# pingpong

new [PingPong](https://app.pingpong.build/trading?invite_code=JMu26PTfcNTQ) version is ready to use now, and it will mine some new tokens like [Blockmesh](https://app.blockmesh.xyz/register?invite_code=iamshaho), Dawn , [Gradient](https://app.gradient.network/signup?code=R32C3T), [Grass](https://app.getgrass.io/register/?referralCode=HZNHg3zmPo9MePr) and Teneo(0CH20).

## If you previously ran Pingpong follow these steps:

find Pingpong screen name and then attach to it

```bash
screen -r pingpong
```

press Ctl + C and then Ctl + D

remove previous folder

```bash
cd $HOME && sudo rm -rf PINGPONG
```


## Install new version and Configuration

create a screen 

```bash
screen -S pingpong
```
and then

```bash
sudo rm -rf PINGPONG && wget https://pingpong-build.s3.ap-southeast-1.amazonaws.com/linux/latest/PINGPONG && chmod +x PINGPONG
```

then run the Pingpong

```bash
chmod +x ./PINGPONG && ./PINGPONG --key YOUR_DEVICE_ID
```

get YOUR_DEVICE_ID from [PingPong Device Page](https://app.pingpong.build/trading?invite_code=JMu26PTfcNTQ)

detach from screen by using Ctl + A + D

if your VPS has low resources its better to stp raptoreum minning

```bash
./PINGPONG stop --depins=raptoreum
```

## Blockmesh configuration

register for [Blockmesh](https://app.blockmesh.xyz/register?invite_code=iamshaho) and then set your email and password 

```bash
./PINGPONG config set --blockmesh.email=your_email --blockmesh.pwd=your_password
```

restart blockmesh minning

```bash
./PINGPONG stop --depins=blockmesh && ./PINGPONG start --depins=blockmesh
```

## Dawn

install [chrome extension](https://chromewebstore.google.com/detail/dawn-validator-chrome-ext/fpdkjdnhkakefebpekbdhillbhonfjjp?authuser=0&hl=en) and then register with my code if you like

```bash
410kck6w
```

then set your email and password and restart mining using below codes

```bash
./PINGPONG config set --dawn.email=your_email --dawn.pwd=your_password
./PINGPONG stop --depins=dawn && ./PINGPONG start --depins=dawn
```

## Gradient

register for [Gradient](https://app.gradient.network/signup?code=R32C3T) and use my code if you like

```bash
R32C3T
```

then set your email and password and restart mining using below codes

```bash
./PINGPONG config set --gradient.email=your_email --gradient.pwd=your_password
./PINGPONG stop --depins=gradient && ./PINGPONG start --depins=gradient
```

## Teneo

install extension [here](https://teneo.pro/community-node#install) and then code  if you like

```bash
0CH20
```

then set your email and password and restart mining using below codes

```bash
./PINGPONG config set --teneo.email=your_email --teneo.pwd=your_password
./PINGPONG stop --depins=teneo && ./PINGPONG start --depins=teneo
```

## Grass
[Grass](https://app.getgrass.io/register/?referralCode=HZNHg3zmPo9MePr)

## follow my X and TG channel for more 

[X](https://x.com/iamshaho)

[UbuntuForNodes TG channel](https://t.me/ubuntufornodes)

## Donations

If you would like to support the development of this project, you can make a donation using the following addresses:

- **Solana**: `EBbY1GskRSgwJcN3cuUCaZqk5zzpsr7A6ku7yg4TCGJa`
- **EVM**: `0x895b2c93976f72E6dB0Bf88265a74f34733abd3D`
- **BTC**: `tb1qfw8zztm67fjzgtru05udwtzq8f069fv8l7am2t`
