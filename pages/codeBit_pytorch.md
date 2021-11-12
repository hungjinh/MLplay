# Code bits in Pytorch

## Device

```python
def try_gpu(i=0):
    """Return gpu(i) if exists, otherwise return cpu()."""
    if torch.cuda.device_count() >= i + 1:
        return torch.device(f'cuda:{i}')
    return torch.device('cpu')
```
Let code be compatible on machines with & without GPUs. <br> e.g. ``X = torch.ones(2, 3, device=try_gpu(0))``

<sub><sup>Reference : [Sec 5.6 D2L](http://d2l.ai/chapter_deep-learning-computation/use-gpu.html) </sup></sub>

