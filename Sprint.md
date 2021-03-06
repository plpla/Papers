# Paper reading sprint


### November 7 2017

#### A simple representation of three-dimensional molecular structure

* Suggest that using 3D fingerprints allow to encode more relevant informations than 2D fingerprints in many applications

* We start with each atom a and give them a unique identifier (32 bit identifier). For each subsequent iterations i (a parameter), we look at a shell radius
of i around a and generate a new joint identifier.

* Merge by hashing each identifier over a large space --> almost no colision

* Gives better results compared to 2D on SEA (binding on 2000 protein targets)

* Encodes molecular information not available in 2D fingerprints (ex: steroisomere)


### October 23 2017

#### Feature selection method based on support vector machine and shape analysis for high-throughput medical data.

* How to select features, considering feature interaction, and how to define the measure that reveals multi-feature interaction are studied on high-throughput medical data

* New feature selection method based on SVM and Procrustes Analysis (PA) is proposed to solve the problem of feature extraction for high-throughput medical data

* Procrustes Analysis is a statistical shape analysis (https://en.wikipedia.org/wiki/Procrustes_analysis)

* To determine the importance of the feature subset, PA is employed to compare the low dimensional embedding structure of the feature subset with that of the original data.

* Data preprocessing (resampling, remove baseline dridt, correct m/z)

* The most separable components in the data are extracted then they use PA to compare the differences between a low dimensional embedding data
structure that removed a feature and the original one, to determine the
importance of the removed feature to maintain the original data structure.

* Advantages: (1) the number q of the mass spectrum
features to be selected is not required to be set in advance; and (2) from
the point of view of the influence of the mass spectrum points in the
direction of SVM extraction, SVM-PA also considers the interaction between
features and the relationship between features and class labels

* In simple: select an appropriate amount of features and keep the ones appropriate for classification.

* Increases the recognition rate (seems to use SVM)


### A lire

W.F.D. Rocha, M.M. Schantz, D.A. Sheen, P.M. Chu, K.A. Lippa, Unsupervised
classification of petroleum Certified Reference Materials and other fuels by
chemometric analysis of gas chromatography-mass spectrometry data, Fuel 197
(2017) 248–258.

http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0160919
