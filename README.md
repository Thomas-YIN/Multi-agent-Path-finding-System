# Multi-agent Path-finding System


https://user-images.githubusercontent.com/90048984/209107354-c0a526d5-6900-4545-a8c7-4a0bb8a58af0.mp4

This repository is for the course project of COMP3211: Artificial Intelligence, HKUST. This is a team project developed by me and [ZHOU Siyuan](https://github.com/szhoubd).

### Project description
Imagine in a warehouse, a fleet of robots are designed to pick up packages from certain
locations and deliver them to certain ports. They should deliver the packages as eﬀiciently
as possible, and at the same time, must not bump into each other or obstacles (no collision). For more details, please refer to [this document](./description.pdf).

### Dependencies:

```
pip install -r requirements.txt
```

### Usage:

```
usage: run.py [-h] [--agents AGENTS [AGENTS ...]] [--map MAP] [--goals GOALS [GOALS ...]] [--vis]
              [--save SAVE]

Multi-Agent Path Finding Term Project.

optional arguments:
  -h, --help            show this help message and exit
  --agents AGENTS [AGENTS ...]
                        Specify a list of agent names
  --map MAP             Specify a map
  --goals GOALS [GOALS ...]
                        Specify the goals for each agent,e.g. 2_0 0_2
  --vis                 Visulize the process
  --save SAVE           Specify the path to save the animation vedio
```

Example:

```
python run.py --agents p1 p2 --map empty --goals 5_5 1_5 --vis --save empty.mp4
```

You may need to install `ffmpeg` to support `.mp4` extension,

```
conda install -c conda-forge ffmpeg
```
