# Wi-CaL: WiFi-based Crowd Estimation
Wi-CaL is a simultaneous crowd estimation system including crowd counting and crowd localization through WiFi sensing and machine learning. We distribute our datasets, codes for conventional machine learning and deep learning, to enable the people interested in wireless sensing to practically test the system.

## Components

### Datasets
(1) small-sized / medium-sized room: We conducted WiFi CSI collection in small-sized meeting room (5.5m X 5.5m) with up to 5 people, and medium-sized seminar room (11m X 5.5m) with up to 10 people, in a campus building.


(2) sess1, 2, 3: We conducted the same data collection for 3 different days. These are for leave-one-session-out cross-validation in machine learning. Day N data is corresponding to sess N.

(3) P=X, S=Y data files: 'P' means the number of people, i.e., 'P=X' file is the feature data obtained from X people case (counting data). 'S' means the section number, i.e., 'S=Y' file is the feature data obtained from the case when people were gathered within a particular section Y in the experiment area.
