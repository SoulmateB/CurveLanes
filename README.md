## CurveLanes Dataset



### Introduction

CurveLanes is a new benchmark lane detection dataset with 150K lanes images for difficult scenarios such as curves and multi-lanes in traffic lane detection. It is collected in real urban and highway scenarios in multiple cities in China. We separate the whole dataset 150K into three parts: train:100K, val: 20K and testing: 30K. The original image resolution is 2650×1440.

 ![CurveLanes](CurveLanes.png)



For each image, we manually annotate all lanes in image with cubic splines. Most of the annotated images in this CurveLanes dataset have more than one curve line with a large curvature. More difficult scenarios such as S-curves, Y-lanes, night and multi-lanes (the number of lane lines is more than 4) can be found in this dataset. 

![proportion](proportion.png)

More introduction of the dataset can be found in our paper.

### Annotations

The dataset should include three parts: 

1. train: images, labels and train.txt
2. valid: images, labels and valid.txt
3. test:  images and test.txt

For each image, there would be a .lines.json label file, in which each line gives the x, y coordinates for key points of the lane marking.

```python 
{
  "Lines":[
    # A lane marking
    [
      # The x, y coordinates for key points of a lane marking that has at least two key points.
      {
        "y":"1439.0",
        "x":"2079.41"
      },
      {
        "y":"1438.08",
        "x":"2078.19"
      },
      ...
    ]
    ...
  ]
}
```



### Downloads



### Tools



### Concact

 For any questions regarding this dataset, please contact Hang Xu (chromexbjxh@gmail.com).

### License

Any academic and non-academic entities can use this dataset freely for non-commercial purposes such as academic research, teaching, or scientific publications. Permission is granted to use the data given that you agree：

1. That you include a reference to the CurveLanes Dataset in any work you do with the dataset.

2. That you do not distribute this dataset or modified versions. It is permissible to distribute derivative works in as far as they are abstract representations of this dataset (such as models trained on it or additional annotations that do not directly include any of our data).

3. That you may not use the data set or any derivative works for commercial purposes, such as selling data or using it for commercial gain.

4. That the data set is provided "as is". Although we ( Huawei Technologies Co., Ltd. ) have made every effort to ensure accuracy, we cannot accept responsibility for errors or omissions.

5. We ( Huawei Technologies Co., Ltd. )  reserve all rights not expressly granted to you.

   

### Citation



### Acknowledgments

 
