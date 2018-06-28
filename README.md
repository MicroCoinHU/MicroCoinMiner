# MicroCoin Miner

Use this program to mine MicroCoins

## How to build

1. Clone from github
```
git clone https://github.com/MicroCoinHU/MicroCoinMiner.git
```
2. Build with lazarus
```
cd MicroCoinMiner
lazbuild MicroCoinMiner.lpi
```
3. Copy [microcoinsha.cl](src/microcoinsha.cl) to output folder
4. Copy libeay32.dll to output folder
5. Run
```
MicroCoinMiner
```

## Command line parameters:
```
-s wallet/pool server:port, leave empty to default
-n your pool username, optional
-c CPU core count for CPU mining
-d X GPU device for GPU mining
-p X GPU platform for GPU mining
```

Example for cpu mining (with 4 cores):
```
MicroCoinMiner -s -n -c 4
```

Example for GPU mining:
```
MicroCoinMiner -p 0 -d -s -n
```
