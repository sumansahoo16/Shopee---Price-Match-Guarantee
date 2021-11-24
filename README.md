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

![image](https://storage.googleapis.com/wandb-production.appspot.com/andrada/images/projects/239376/5f470291.png?Expires=1637777196&GoogleAccessId=wandb-production%40appspot.gserviceaccount.com&Signature=FYX4CHpO8mzZ2z9eWlMsieU%2B5kdYQVCrtE8Qrem0OLtuaQhHloxSYNOButHOfxghim2QTww9qDxM1fiqWpJZTV%2BbqtdqLD%2BN9K9N03XKb%2B7Q1Gdn4AUVN%2FQYu5gYpHaYoJOhNSNGZZbhfclVQVxOZ%2B3YgudpEDaDabBaujK%2BIprWVoQhi9sehtKGTnX%2BgIn%2FDbhlU2hJtmttSDTtQqAWR3pYMf1p1WCnK%2BXc%2BcbqJeAeo3wzUXrsGF1yFAPxhMjIW6bYEnlPtrs0LS3bNduDD4BWOitA0C3K87%2Fm%2FvQFgGBZZQ6ifsr%2BPv2Cz5mf8plXbWf2tXozy2rMf1xl12rHJQ%3D%3D)


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
