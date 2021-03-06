# First Order Motion Model for Image Animation

This repository contains the source code for the paper [First Order Motion Model for Image Animation](https://papers.nips.cc/paper/8935-first-order-motion-model-for-image-animation) by Aliaksandr Siarohin, [Stéphane Lathuilière](http://stelat.eu), [Sergey Tulyakov](http://stulyakov.com), [Elisa Ricci](http://elisaricci.eu/) and [Nicu Sebe](http://disi.unitn.it/~sebe/). 

### Installation
Хэрэв NVIDIA GPU байгаа бол CUDA enabled PyTorch-ыг татаж суулгана уу.
Үүний тулд Conda evniroment үүсгэн дараах алхмуудыг хийнэ үү.
```console
conda create -name new_env python=3.6
activate new_env
pip install -r requirements_gpu.txt
conda install pytorch torchvision cudatoolkit=9.2 -c pytorch
conda install numpy
conda install ffmpeg -c conda-forge
```

jupyter kernel-ийг install хийж өгнө. Үүний тулд conda env-аа activate хийсэн байх ёстойг анхаарна уу!
```
python -m ipykernel install --user --name new_env --display-name "Python (new_env)"
```

Эцэст нь Demo.ipynb дотороо kernel-ийг нь өөрсдийн үүсгэсэн kernel-д шилжүүлнэ!

Хэрэв NVIDIA GPU байхгүй бол шууд requirements.txt дотор байгаа сангуудыг доорх коммандаар татна уу.

(Энэ нь дан CPU дээр ажиллах тул хувиргалтын үед удаан ажиллана.)
```
pip install -r requirements_cpu.txt
pip install torch==1.5.0+cpu torchvision==0.6.0+cpu -f https://download.pytorch.org/whl/torch_stable.html
```


### Pre-trained checkpoint
Checkpoints can be found under following link: [google-drive](https://drive.google.com/open?id=1PyQJmkdCsAkOYwUyaj_l-l0as-iLDgeH) or [yandex-disk](https://yadi.sk/d/lEw8uRm140L_eQ).

Citation:

```
@InProceedings{Siarohin_2019_NeurIPS,
  author={Siarohin, Aliaksandr and Lathuilière, Stéphane and Tulyakov, Sergey and Ricci, Elisa and Sebe, Nicu},
  title={First Order Motion Model for Image Animation},
  booktitle = {Conference on Neural Information Processing Systems (NeurIPS)},
  month = {December},
  year = {2019}
}
```
