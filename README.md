# ResNet Implementation for CIFAR10 in PyTorch

The experiment is carried out on the data set CIFAR10. The network selected in the experiment is ResNet32, and we do the hyper-parameters tuning and analyzing.

## Start to train

ResNet32, lerning_rate=0.1
```bash
python -u trainer.py --epochs=100 --lr=0.1 --weight-decay=1e-4
```
<div align="center">
  <img src="assets/fig_1.jpg"  width="500px" />
</div>

ResNet32, lerning_rate=0.3
```bash
python -u trainer.py --epochs=100 --lr=0.3 --weight-decay=1e-4
```
<div align="center">
  <img src="assets/fig_2.jpg"  width="500px" />
</div>

ResNet32, lerning_rate=0.5
```bash
python -u trainer.py --epochs=100 --lr=0.5 --weight-decay=1e-4
```
<div align="center">
  <img src="assets/fig_3.jpg"  width="500px" />
</div>

We can compare the train loss and precision between different learning rates of the model, and we can find that when the learning rate is 0.1, the ResNet model show the better effect.

<div align="center">
  <img src="assets/fig_4.jpg"  width="500px" />
</div>

<div align="center">
  <img src="assets/fig_5.jpg"  width="500px" />
</div>
