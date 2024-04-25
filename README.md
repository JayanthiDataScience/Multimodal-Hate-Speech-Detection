# Multimodal Hate Speech Detection
# INTRODUCTION
In the evolving social media landscape, hate speech detection presents a multifaceted barrier, demanding a complex understanding of textual and visual content. This project addresses the challenge of detecting hate speech in multimedia content by developing an advanced fusion model that integrates image and text data. Identifying the limitations of existing unimodal approaches, that predominantly focus on either text or images, this project proposes a novel multimodal framework that enhances the detection of hate speech by leveraging the contexts between visual and textual cues. 
# OBJECTIVE
To develop a system with good capability of hate speech detection by including visual content analysis and textual analysis,
improve the model’s ability to understand the context in which hate speech occurs, specifically in visual content, and to create a safer online environment.
# DATA OVERVIEW
The dataset consists of 1,50,000 tweets annotated by 3 annotators using the platform of Amazon Mechanical Truck. It consists of tweet text, image text, and images. It has 5 fields namely img_url, labels, tweet_url, tweet_text and labels_str.
The labels are an array of length 3 denoting classes 0 to 5.The labels_str is the array with three labels string consisting of label definitions for each class.
# METHODLOGY
1) For texts preprocessing is done using methods like tokenization, padding, removal of stop words, stemming, and lemmatization.
2) For images preprocessing is done to scale them to the size of 500 pixel.
3) After preprocessing majority voting was done among three labels to get a single label for each class.
4) After labelling the entire dataset is divided into training, test and validation based on their tweet ids.
5) The labelled data is given as input to feature extraction where relevant features from the data are extracted.
6) The extracted feature data is trained using machine learning models and deep learning models. The output of the model is either classified or binarized based on the output function.
# RESULTS
For Unimodal Text model BERT performed the best. For Unimodal Image Multilayer Perceptron had better ROC. For Multimodal model the combination of Images, Image Text, Tweet Text achieved an higher ROC.
# CONCLUSION & FUTURE WORK
The project employed sophisticated machine learning and neural networks to integrate and analyze both textual and visual data, aiming to identify and categorize hate speech more effectively than using text or image data in isolation. As hate speech can also be present in audio, future work could integrate audio analysis with images and text for comprehensive content analysis. Investigate the use of transformer models like VisualBERT, ViLBERT, or CLIP that have been pre-trained on a large corpus of image-text pairs.
# CONTRIBUTORS
1) Jayanthi Jayakumaran
2) Venkata Sai Tarun Munduri





