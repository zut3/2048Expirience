# 2048Expirience
This repo contains dataset of 2048 game. File encoded in hdf5 format.

## Usage
```python
  import h5py
  f = h5py.File('games_0.h5', 'r')
  f['states'][:] #numpy array of game states
  f['actions'][:] #0, 1, 2, or 3, what means up, down, left, or right actions
  f['rewards'][:] #1 if this move leads to win and -1 if leads to lose
  f.close()
```
