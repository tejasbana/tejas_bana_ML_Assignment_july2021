
Problem Statement:
 Fashion category and attribute extractoin from an image.

Case considered:
1. Public, studio and extracted cloth images are considered.
2. 50 category and 1000 attributes considered.
3. Front and back of the cloths are taken into consideration.
4. Image transformation, like rotation for recognizing cloths from every angle.
5. Only Single person images.

Cons:
1. No bounding box
2. Multiple cloths items in a sigle image.
3. Multiple persons in the images.
4. Cloths from side angle.


<table style="width:100%">
  <!-- <tr>
    <th>Day-Date</th>
    <th>Work</th> 
    <th>Time</th>
  </tr> -->
  <tr>
    <td>Day 1: 11/07/2021</td>
    <td>Day 2: 12/07/2021</td>
    <td>Day 3: 13/07/2021</td>
    <td>Day 4: 14/07/2021</td>
    <td>Day 5: 18/07/2021</td>
    <td>Day 6: 19/07/2021</td>
  </tr>
  <tr>
    <td>1. Read the paper regarding the simple approach. CNN-Classification
		<br>2. Cloths extraction followed by classification.</td>
    <td>1. Read state-of-the-art Research Paper:
		<br>2. Attentive Fashion Grammar Network for
  		Fashion Landmark Detection and Clothing Category Classification</td>
    <td>1. Dataset finalization: DeepFashion</td>
    <td>1. Work on basic implementation: Vision Transformer classification
		<br>2. Exploring the dataset with pandas
		<br>3. Creating category head and attribute head for classification
		<br>4. Further Implovement </td>
    <td>1. <strong>Working on the Code</strong></td>
    <td>1. <strong>Experiment with Resnet-18 and ResNext_52_4d</strong></td>
  </tr>
  <tr>
    <td>(1-2hrs)</td>
    <td>(2hrs)</td>
    <td>(1-2hrs)</td>
    <td>(3-4hrs)</td>
    <td>(8 hrs)</td>
    <td>(4 hrs)</td>
  </tr>
</table>


<h1>Experiments:</h1>

1. ResNet-18 from scratch --> X

<table style="width:100%">
  <!-- <tr>
    <th>Day-Date</th>
    <th>Work</th> 
    <th>Time</th>
  </tr> -->
  <tr>
    <td>2. PreTrained ResNet-18</td>
    <td>30 epochs</td>
    <td>category  val_acc: 99.62%</td>
    <td>attribute val_acc: 03.93%</td>
    <td>binary_cross_entropy_with_logits</td>
    <td>Should use a different loss function</td>
  </tr>
  <tr>
    <td>3. PreTrained ResNext_32_4d</td>
    <td>25 epochs</td>
    <td>category  val_acc: 93.09%</td>
    <td>attribute val_acc: 02.00%</td>
    <td>binary_cross_entropy_with_logits</td>
    <td><strong>No improvement using big models.</strong></td>
  </tr>
  <tr>
    <td>4. PreTrained ResNet-18</td>
    <td></td>
    <td></td>
    <td></td>
    <td>MultiLabelSoftMarginLoss</td>
    <td></td>
  </tr>
</table>


Important Links: 

1. DeepFashion: http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html
2. Vision Transformer: https://github.com/lucidrains/vit-pytorch
3. BRCNN approach: https://github.com/zuoxiang95/BCRNN
4. Other info: https://github.com/PlabanM1/FashionNet/blob/master/FashionNet.ipynb


<h1>Day 1: 11/07/2021</h1>

1. Read the paper regarding the simple approach. CNN-Classification

2. Cloths extraction followed by classification.

<h1>Day 2: 12/07/2021</h1>

1. Read state-of-the-art Research Paper:

2. Attentive Fashion Grammar Network for
  Fashion Landmark Detection and Clothing Category Classification

<h1>Day 3: 13/07/2021</h1>

1. Dataset finalization: DeepFashion 

<ul>
    <li>289,222 number of clothes images;</li>

   <li>
    50 number of clothing categories, and 1,000 number of clothing attributes; 
   </ll>li>

   <li>Each image is annotated by bounding box and clothing type.<li>
</ul>

<h1>Day 4: 14/07/2021</h1>

1. Work on basic implementation: Vision Transformer classification

2. Exploring the dataset with pandas

3. Creating category head and attribute head for classification

4. Further Implovement 