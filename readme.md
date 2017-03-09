### Second project in Deep Learning Nanodegree

Assignment to classify images.


## Running with jupyter:

```bash
conda create --name tflow python=3
source activate dlnd
# or activate dlnd on windows
conda install numpy matplotlib pandas tqdm jupyter notebook scikit-learn bokeh scipy h5py -y
pip install tensorflow
jupyter notebook dlnd_image_classification.ipynb
```

## Running with docker 

```bash
docker build -t xavero/deeplearn .
docker run -p 8888:8888 -v /$(pwd):/opt/notebooks xavero/deeplearn
# the last command output will contain the link for access jupyter, including the token. 
# if you are using Docker Toolbox, replace the host with the docker machine ip or hostname.
```