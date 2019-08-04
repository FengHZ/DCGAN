# DCGAN
A demo of DCGAN in CelebA

## Requirements

```python
python >=3.5
Pytorch >=1.1.0
torchvision >= 0.2.1
pillow 
numpy
scikit-learn
tensorboard
```
## Dataset
In this project, we use the [face recognition dataset `Celeba`](https://zhuanlan.zhihu.com/p/35975956), and download the `img_align_celeba.zip` file. The user should specify the `basepath` and put the unzipped data into folder

```
os.path.join(basepath,"dataset","celeba")
```

## Run

```
python main.py -dp -bp basepath --gpu gpu_id(e.g. "0,1")
```

## Result Check

The train results as well as the generated images will be stored in 

```
os.path.join(basepath,"DCGAN")
```

Then to view the whole process of training, jump into the folder and use command

```
tensorboard --logdir runs
```

to view the training log in web browser.

