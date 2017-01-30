1) firsly, we have extracted SIFT features,using BOW.cpp<br />
This code uses a Sliding Window(8x8) with overlap of 4 pixels. Using BOW1.cpp, we have almost 37k frames,which we have extracted vecors of 128 SIFT features.<br />
The fisrt has two outputs:1) frames with SIFT points on them. 2) "dictionary.yml"file which is used in the next stage. This file consists of CLuster's Centers. Here, we have used 9 clusters<br />
In stage two, the input of the code is each frame,separetly. This code firstly reads the "dictionary.yml",and investigate the nearest center to each frame. Using Bag of Words, the outputs are "descriptor.yml" and "video.csv" in which each frame has 9 features(membership to clusters).<br />
