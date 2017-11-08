# a3c-tensorflow

This repo contains python code for replicating the asynchronous advantage actor-critic algorithm as described in https://arxiv.org/pdf/1602.01783.pdf

## Requirements

* tensorflow
* scipy
* gym (Atari)
* skimage

## Training

For training a3c algorithm in BreakoutDeterministic-v3 using 8 parallel actor learner threads execute the following command:
```
python a3c.py --game BreakoutDeterministic-v3 --num_concurrent 8
```

## Testing

For testing a trained a3c agent execute the folowing command
```
python a3c.py  --game BreakoutDeterministic-v3 --checkpoint_path path_to_checkpoint --testing True
```

## Resources

https://github.com/miyosuda/async_deep_reinforce

https://github.com/coreylynch/async-rl

https://github.com/muupan/async-rl
