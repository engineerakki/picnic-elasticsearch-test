# Take-Home-Test

## Pre-Requisites:
i)  K8s(min 2 nodes, v1.14+) \
ii) kubectl \
iii) Helm (v3+) 

## Usage Details:

### Step1:
Clone this repository and create a namespace:

    git clone https://github.com/engineerakki/picnic-elasticsearch-test.git
    cd elasticsearch
    kubectl create ns es

### Step2:
Install the chart:

    helm install demo -n es .

### Step3:
Test the chart:

     helm test -n es demo

### Step4:
Access the cluster health:

    curl -XGET '164.90.242.19:9200/_cluster/health?pretty'
    
## More detailed README with screenshots:
[Full README File](https://drive.google.com/file/d/1bgzMmqBQBByLEGfxo7MBZYzVviJJjS1c/view?usp=sharing)
