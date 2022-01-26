# PersonRE-ID-Project-
This Repository contains a project for the exam of Deep Learning at University of Trento.

The project consists in 2 main tasks:
<li> Attribute Prediction </li>
<li> Person Re-Identification </li>

Given various images of different persons taken from different cameras (a version of Market-1501 Dataset), the model should try to predict a series of attributes associated with each image and produce similar embeddings for different images of the same person. 
The approach proposed in the code is composed by a Pretrained ResNet as a common backbone to extract the common features from the images in order to create the embeddings; as a next step, the embeddings are fed into 12 different Convolutional heads for the attribute recognition task (one for each attribute of our list) and an additional head for the prediction of the Person ID associated with the input image. The possible attributes of an image are:
<table>
  <tr>
   <th>Attributes</th>
   <th>Possible values</th>
  </tr>
  <tr>
   <th>Age</th>
   <th>Young, Teenager, Adult, Old</th>
  </tr>
  <tr>
   <th>Backpack</th>
   <th>Yes, No</th>
  </tr>
  <tr>
   <th>Bag</th>
   <th>Yes, No</th>
  </tr>
  <tr>
   <th>Hand Bag</th>
   <th>Yes, No</th>
  </tr>
  <tr>
   <th>Clothes</th>
   <th>Dress, Pants</th>
  </tr>
  <tr>
   <th>Down</th>
   <th>Long, Short</th>
  </tr>
  <tr>
   <th>Up</th>
   <th>Long, Short</th>
  </tr>
  <tr>
   <th>Hair</th>
   <th>Short, Long</th>
  </tr>
  <tr>
   <th>Hat</th>
   <th>Yes, No</th>
  </tr>
  <tr>
   <th>Gender</th>
   <th>Male, Female</th>
  </tr>
  <tr>
   <th>Up Color</th>
   <th>Black, White, Red, Purple, Yellow, Gray, Blue, Green, Multicolor</th>
  </tr>
  <tr>
   <th>Down Color</th>
   <th>Black, White, Pink, Purple, Yellow, Gray, Blue, Green, Brown, Multicolor</th>
  </tr>
</table>
