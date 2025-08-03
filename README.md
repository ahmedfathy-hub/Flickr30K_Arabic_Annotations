# Flickr30K_Arabic_Annotations

The Flickr30K dataset is a widely used benchmark in vision-language research, serving as a key resource for tasks like image captioning, and visual question answering (VQA). 

## Dataset Structure 
1. Size: 31,783 images collected from Flickr. 
2. Captions: 5 human-annotated English descriptions per image, 158,915 captions in total.
3. About images: everyday scenes, activities, objects, and people with no synthetic or artificial images.
4. License: images are publicly available under Flickr’s terms, but redistribution may require permission. 

## Data preprocessing Steps
1. Original Flickr30K dataset was separated into 6 chunks to speed up translating process and avoid Google Cloud Translation API down time because of long responses.
2. Each chunk was divided into 5 sub chuncks each one has 1000 images and each image has 5 captions, so each chunk includes 5000 English statement translated by Google Cloud Translation API.
3. The model used is Google Neural Machine Translation, with Arabic as target language. It provides high fluency and good statement translation
