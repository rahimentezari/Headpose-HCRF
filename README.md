# Headpose-HCRF
 1)This project is to estimate human head pose in video.<br />
 2)The dataset used here is HPEG(A Natural Head Pose abd Eye Gaze Dataset).This dataset consists of 2 sessions. I have used session a. Session b also includes Gaze data.<br />
 3)In Session a,each video last for almost 6 seconds. There is also a "data"file for each video,which consists of head angle(Yaw).<br />
 4) I have used Probabilistic Graphical Model for classification. In more datails,I have used Conditional Random Fields in terms of HCRF Library. <br />
 Feature Extraction:<br />
 For this phase I have used the following paper:"Head Pose Estimation Using Histogram of SIFT Descriptors ". So I have used SIFT Features too.
