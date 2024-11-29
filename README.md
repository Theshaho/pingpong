# pingpong

new [PingPong](https://app.pingpong.build/trading?invite_code=JMu26PTfcNTQ) version is ready to use now, and it will mine some new tokens like [Blockmesh](https://app.blockmesh.xyz/register?invite_code=iamshaho), Dawn(410kck6w), Gradient(R32C3T), [Grass](https://app.getgrass.io/register/?referralCode=HZNHg3zmPo9MePr) and Teneo(0CH20).

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

```bash
    sudo rm -rf PINGPONG && wget https://pingpong-build.s3.ap-southeast-1.amazonaws.com/linux/latest/PINGPONG && chmod +x PINGPONG
```

then run the Pingpong

```bash
chmod +x ./PINGPONG && ./PINGPONG --key YOUR_DEVICE_ID
```

get YOUR_DEVICE_ID from [PingPong Device Page](https://app.pingpong.build/trading?invite_code=JMu26PTfcNTQ)

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
