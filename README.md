# Sleep stage classification from EEG data
**Sleep_physionet age Dataset _BCI project**

![image](https://user-images.githubusercontent.com/63863517/230394200-7b3fdf2a-28fa-43ea-99e6-ac2c14c93b3b.png)

1. Extract 30s events from annotations
2. Used Annotations descriptions :
  - 'Sleep stage 1'
  - 'Sleep stage 2'
  - 'Sleep stage 3'
  - 'Sleep stage 4'
  - 'Sleep stage R'
  - 'Sleep stage W'

![image](https://user-images.githubusercontent.com/63863517/230394481-d6212f72-bebe-433b-95e4-738a0fa4c178.png)

3. Create Epochs from the data based on the events found in the annotations

## Feature Engineering
### Good feature STD :
![image](https://user-images.githubusercontent.com/63863517/230391146-2f495747-c59f-49c9-a2b6-5aa766e1c307.png)

![image](https://user-images.githubusercontent.com/63863517/230391226-4d4c5967-0d04-4c94-b4ef-cb63e78a710a.png)

![image](https://user-images.githubusercontent.com/63863517/230391279-872f1b24-8266-4d7d-9842-9d49e2cf77b0.png)

### Good Feature as Peak-to-peak (PTP) amplitude

![image](https://user-images.githubusercontent.com/63863517/230391388-fbab6b74-6efa-4164-a177-b922be36ab23.png)

### Good Feature as Root-mean squared

![image](https://user-images.githubusercontent.com/63863517/230391500-f521e23d-631d-41fa-a175-4cbf7a04a7ee.png)

### Baaaad Feature as Kurtosis

![image](https://user-images.githubusercontent.com/63863517/230391611-094327a0-cddb-4c28-97da-e79970f400e8.png)

### baaad feature Skewness

![image](https://user-images.githubusercontent.com/63863517/230391713-da26c127-6ad8-410e-b650-d651e6165e61.png)


### Multiclass classification :
|Models|accuracy|
| --- | --- |
|SVM|% 72.03389830508475|
|K-Neighbors-Classifier| % 81.35593220338984|
|Decision-Tree-Classifier|% 87.28813559322035|
|Random-Forest-Classifier|% 87.28813559322035|
