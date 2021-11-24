# Shopee---Price-Match-Guarantee

### Problem Statement

The Shopee - Price Match Guarantee Kaggle competition had the purpose of identifying if two products are the same by looking at their images and descriptions.

Two different images of similar wares may represent the same product or two completely different items. Retailers want to avoid misrepresentations and other issues that could come from conflating two dissimilar products.  - Shopee

Goal: To build a model that can identify which images contain the same product/s.

Challenges:
- Finding near-duplicates of the product (and NOT the image)
- Erasing the impact of the background (the area surrounding the product) 
- Using the description of the image (or the title )

Dataset Example : 

![image](https://api.wandb.ai/files/andrada/images/projects/239376/5f470291.png)


### Solution 

Models : nfnet_l0, nfnet_l1, sbert, distilbert, w2v, phash, tfidf

with :
- CurricularFace
- SAM optimizer
- concatenating image_embeddings and text_embeddings
- tfidf
- TTA(Resize+CenterCrop)

Summary : 

![image](https://user-images.githubusercontent.com/66665933/117750943-3e298100-b24f-11eb-990e-07c7e2c57026.png)
