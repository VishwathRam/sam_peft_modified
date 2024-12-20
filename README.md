- Implements PEFT (Parameter Efficient Fine Tuning) for SAM.
- Reduces no. of trainable parameters to 0.203%.

```bash
~/Desktop/workspace/peft-sam/src main peft-sam ❯ python models.py 
* Normal SAM model (with all weights unfrozen):
  * trainable params: 93735472 || all params: 93735472 || trainable%: 100.000%
* Normal SAM model (with encoder weights unfrozen):
  * trainable params: 4058340 || all params: 93735472 || trainable%: 4.330%
* Normal peft SAM model (frozen encoders):
  * trainable params: 190720 || all params: 93923888 || trainable%: 0.203%
* Normal peft SAM model (un-frozen encoders):
  * trainable params: 190720 || all params: 93923888 || trainable%: 0.203%
```
