# Instructions

Install warp-ctc first using cmake

- `mkdir build`
- `cd build`
- `cmake ..`
- `make`

Now, go to the python directory and run `sudo python setup.py install`

# Usage

Once installed, you should be able to `import ctc`.

`ctc.cpu_ctc_np`, `ctc.cpu_ctc_th` are Numpy and Python bindings respectively.

Inputs: 
  - acts: 3-d float array, same as c++ bindings
  - act_lens: 1-d int array of input length of each example
  - labels: list of 1-d int array for each example in minibatch
  - label_lens: 1-d int array of label length of each example
Outputs:
  - cost: 1-d float array for cost of each minibatch example
  - grads: 3-d float array for pre-activation gradients

# Credits

https://github.com/baidu-research/warp-ctc
