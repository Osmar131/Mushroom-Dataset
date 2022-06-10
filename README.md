# Portfolio
# Musroom dataset project
The dataset provided by The Audobon Society Field Guide to North American Mushroom (1981) contains descriptions of hypothetical samples corresponding to 23 species of mushrooms of the Agaricus and Lepiota families. Each species is classified as edible or poisonous.

![image](https://user-images.githubusercontent.com/77253306/172767841-adb25971-b31e-42a4-9172-9c97ee399acb.png)

# Summary
Classifying each fungal sample in the dataset allows knowing if a mushroom with the provided characteristics is edible or poisonous.

For the classification problem, it is proposed to use the Random Forest ensemble algorithm.

# Training
Random Forest builds a set of trees with library sklearn and the prediction is the average of the results of each individual prediction of each tree.

![Arbol_8](https://user-images.githubusercontent.com/77253306/172770816-fec279fd-393d-4786-9980-a06848de917a.png)


# Results
The metrics obtained show good performance with the Random Forest trained model.

![tif43](https://user-images.githubusercontent.com/77253306/172771215-21c62ad0-adf5-4672-8b79-9e078fa4262f.png)

![tif44](https://user-images.githubusercontent.com/77253306/172771222-aa361a5b-55df-4de0-aa98-fd68bf008118.png)

Evolution of out-of-bag-error vs number of trees shows that the error decreases as different amounts of trees are tested, it also shows that the optimal number of trees is 21.

![tif45](https://user-images.githubusercontent.com/77253306/172986198-fd946694-dd0a-4757-ab66-7675653f191b.png)

Evolution of cv-error vs number of trees shows the error decrease as different amounts of trees are tested and with a kfold of 5, it also shows that the optimal number of trees is 11.

![tif46](https://user-images.githubusercontent.com/77253306/172986789-6897a43a-20dd-4746-87d5-d73747b5650b.png)

# Conclusiones
A decision tree tends to get over-trained, so one way to avoid this is through ensembles of prediction models. Random Forest builds several trees at once reducing this overtraining by averaging the results and also taking different samples from a training set.

It is also possible to reduce this over-training by adjusting various additional parameters such as the selection of certain attributes, type of gain measurement and the type of data, whether categorical or numeric.


<!---
Osmar131/Osmar131 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
