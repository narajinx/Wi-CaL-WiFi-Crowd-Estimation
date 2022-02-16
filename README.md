# Wi-CaL: WiFi-based Crowd Estimation
Wi-CaL is a simultaneous crowd estimation system including crowd counting and crowd localization through WiFi sensing and machine learning. We distribute our datasets, codes for conventional machine learning and deep learning, to enable the people interested in wireless sensing to practically test the system.

## Components

### Datasets
(1) small-sized / medium-sized room: We conducted WiFi CSI collection in small-sized meeting room (5.5m X 5.5m) with up to 5 people, and medium-sized seminar room (11m X 5.5m) with up to 10 people, in a campus building.


(2) sess1, 2, 3: We conducted the same data collection for 3 different days. These are for leave-one-session-out cross-validation in machine learning. Day N data is corresponding to sess N.

(3) P=X, S=Y data files: 'P' means the number of people, i.e., 'P=X' file is the feature data obtained from X people case (counting data). 'S' means the section number, i.e., 'S=Y' file is the feature data obtained from the case when people were gathered within a particular section Y in the experiment area. 'S=0' is a case of when all participants were walking around all over the area.

### Learning codes (written in Jupyter notebook)

First, you select which estimation you want to check out (crowd-counting or crowd-localization). You will find regression code for counting, and classification code for localization.
For each estimation, two kinds of validation methods are included (k-fold_cross-validation or leave-one-session-out_cross-validation).
Then again, two kinds of learning codes are included (ML or DNN).

(1) k-fold / leave-one-session-out cross-validation: For k-fold cross-validation, we implemented stratified k-fold method in our code. You can select which session data you will use for learning models at the 5th cell of the codes. On the other hand, for leave-one-session-out cross-validation, all sessions data will be used at the same time, 2 sessions for training and 1 session for testing.

(2) learning models: In ML codes, you will find 4 different conventional ML models are used for system evaluation. Indeed, you can change the models or parameters as you wish. In DNN codes as well, you can adjust the DNN architecture, activation function, early stopping patience, etc.
