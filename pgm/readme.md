For Classification I have used Linear Chain Conditional Random Fields. In this stage, extracted features(a file for each video, consists of vecots of 9 values for each frame) are the input of model. <br/ >
I have quantized labels in bins of 15 degree: -45to35--->1,2,3...,7<br/ >
I have used HCRF2.0 library.<br/ >
train data,train label.test data,test label are as follows,respectively: dataTrain.csv,labelTrain.csv,dataTest.csv,labelTest.csv<br/ >
for train and test I have used the following command:<br/ >
TestHCRF.exe [-t] [-T] [-d filename] [-l filename] [-D filename] [-L  filename] [-m filename] [-f filename]    [-r filename] [-o cg|bfgs|asa ]-a crf|ldcrf|hcrf|ghcrf] <br/ >
testHCRF.exe -t -T -d dataTrain.csv -l labelsTrain.csv -D dataTest.csv -L labelsTest.csv -m model.txt -f  fetures.txt -r results.txt -c stats.txt -o lbfgs -a crf <br/ >
for paremeter learning(weights of potential functions) I used LBFGS optimization.<br/ >
10 cross-fold validation is used. the results show the 62% precision for 7 class.
