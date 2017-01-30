1) firsly, we have extracted SIFT features,using BOW.cpp<br />
This code uses a Sliding Window(8x8) with overlap of 4 pixels. Using BOW1.cpp, we have almost 37k frames,which we have extracted vecors of 128 SIFT features.<br />
This stage has two outputs:1) frames with SIFT points on them. 2) "dictionary.yml"file which is used in the next stage. This file consists of CLuster's Centers. Here, we have used 9 clusters<br />
