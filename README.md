# EfficientCube+: DNN-based Rubik's Cube Solver

## TODO

- [x] Accelerate cube operations
  - [x] Enable TF32 mode for faster training/inference (TensorCore)
  - [x] Remove redundant sticker replacement plan generation
  - [x] Move cube creation to GPU
  - [x] Implement in-GPU cube operations (PyTorch)
  - [x] Implement in-GPU cube operations (Triton)
- [x] Optimize model training
  - [x] Implement in-GPU training data generation
  - [x] Fix performance degradation in mixed-precision FP16 mode
- [x] Accelerate inference
  - [x] Minimize data transfer between CPU and GPU
  - [x] Use log probability to reduce floating point error
  - [x] Parallelize the inference process
- [ ] Adjust model structure
  - [ ] Change activation-norm to norm-activation
  - [ ] Adjust layer sizes
  - [ ] Add layer norm or activation after ResidualBlock
  - [ ] Use dropout
  - [ ] Use weight initialization
  - [ ] Test layer norm
- [ ] Reinforcement learning
  - [ ] Apply reinforcement learning after supervised learning
  - [ ] Evaluate the result