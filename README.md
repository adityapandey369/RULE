# RULE
                                                              Remaining Useful Life Estimation of Milling Tool



RUL Estimation of Milling Tools through Different Learning Styles
ABSTRACT:
In order to prevent catastrophic tool failure and unanticipated downtime, remaining useful life (RUL) predictions of milling tools are crucial in the industrial sector. RUL prediction has made extensive use of machine learning methods; however, these systems need a lot of labelled data to train on. In the manufacturing industry, it might be challenging to obtain labelled data. While labelled data can be difficult and expensive to gather, one-shot learning (OSL) algorithms can learn from just one or a small number of samples, making them acceptable for RUL prediction of milling tool wear.
This study introduces a novel method for RUL milling tool wear prediction using a One-Shot Learning algorithm. The two stages of the suggested method are feature extraction and RUL prediction. The milling tool's time series sensor data is converted into a set of features during the feature extraction stage, which identifies the underlying patterns and trends of tool wear. The OSL algorithm is then trained on the features that were retrieved in order to forecast the RUL of the milling tool.
The experimental results demonstrate that the suggested methodology performs better in terms of accuracy, precision, and recall than conventional RUL prediction approaches. The usefulness of one-shot learning algorithms in RUL prediction of milling tool wear was demonstrated by the dataset's average RUL prediction error, which was less than 5%. The suggested method has the potential to increase manufacturing process efficiency by decreasing the frequency of tool replacements and the resulting downtime.
In summary, this study suggests a unique method for RUL milling tool wear prediction utilising a one-shot learning algorithm that can learn from a single or small number of samples. The experimental findings show how well the suggested method predicts milling tool wear using RUL and how it could boost manufacturing process effectiveness.
INTRODUCTION:
All tools eventually break down and gradually fail due to regular operations. This sort of wear will show inconsistencies and will have unwanted effects on your workpiece. Hence, it is important to circumvent tool wear in order to achieve the optimum work.
This is done through tool wear detection; a process that monitors and evaluates the deterioration of cutting tools during machining operations. The objective is to detect the onset of wear and its progression, in order to prevent machine downtime, improve tool life, and ensure the quality of machined parts. This can be achieved through various techniques, including visual inspection, acoustic emission, vibration analysis, and machine learning.bv.
to be quite an important process as it enhances the precision of products by eliminating extra material and moulding it to the required specifications, as well as improving the appearance
1

RUL Estimation of Milling Tools through Different Learning Styles
and functioning of items by giving them a smooth surface finish. The procedure enables machining of complex shapes and forms, and also facilitates mass production by allowing the efficient production of identical parts.
Significance of tool wear:
Tool wear has an impact on a machined part’s surface finish and dimensional correctness and therefore, can lead to tool breakage, which lowers manufacturing effectiveness and raises costs. Furthermore, reduced functioning may result from such machined parts with poor surface quality and nonuniformity. Frequent tool wear then eventually leads to frequent tool changes, which also contributes to the slowing down of the production process.
Despite the fallbacks of tool wear, it can serve as a warning sign for process issues, enabling prompt adjustment of cutting parameters to increase tool life.
Factors Effecting Tool wear:
● Cutting parameters: such as speed, feed rate, and depth of cut.
● Material properties: including hardness, toughness, and composition of the
workpiece material.
● Tool material and geometry: the type of tool material and its geometry, including
the rake angle, relief angle, and nose radius.
● Cutting environment: including coolant type and temperature, and ambient
temperature and humidity.
● Machine tool conditions: such as vibration and spindle run out.
● Operator skill and experience: affecting tool handling and setting.
● Workpiece clamping: affecting the stability and accuracy of the machining
process.
Recent trends in tool wear estimation / Research Gap:
Knowing that tool life can be reduced by 50% or more in extreme wear conditions, Researchers have found many ways in which to detect such wear, including the following:
1. Acoustic emission: The use of acoustic sensors to detect and analyse the sounds generated by tool wear and failure.
2. Cutting force monitoring: The use of sensors to measure the cutting force during machining and detect changes that indicate tool wear.
3. Optical sensing: The use of optical sensors, such as optical microscopes and laser interferometers, to detect and monitor tool wear.
4. Infrared thermography: The use of infrared cameras to detect and measure temperature changes during cutting that can indicate tool wear.
5. Machine learning: The use of machine learning algorithms to analyse cutting data and detect patterns that indicate tool wear.
6. Neural networks: The use of artificial neural networks to classify tool wear states based on cutting parameters and sensor data.
7. Fuzzy logic: The use of fuzzy logic algorithms to analyse sensor data and detect changes that indicate tool wear.
   2

RUL Estimation of Milling Tools through Different Learning Styles
8. Image processing: The use of image processing techniques to analyse tool wear patterns and make predictions about future performance.
9. Condition monitoring: The use of continuous monitoring and analysis of cutting data to detect tool wear and predict future performance.
However, even some of these techniques mentioned above, fall short of the required result:
1.Lack of real-time monitoring: Most tool wear detection methods rely on offline analysis and are not capable of real-time monitoring.
2. Inaccurate predictions: The existing methods have limitations in detecting and predicting tool wear accurately, particularly in dynamic cutting conditions.
3. Limited sensor compatibility: The compatibility of sensors with different cutting tools and materials is limited, making it difficult to apply the same detection method to a wide range of cutting processes.
4. Limited integration with manufacturing systems: Most tool wear detection methods are not fully integrated into manufacturing systems, making it difficult to automate the process and implement real-time adjustments.
5. Limited adaptability to changing cutting conditions: Many tool wear detection methods are not capable of adapting to changing cutting conditions, such as changes in cutting speed or material hardness, which can result in incorrect predictions.
Tool wear detection relies heavily on AI/ML since it facilitates process automation and produces effective results. Machine learning algorithms are able to process enormous amounts of data and spot patterns that might point to flaws. In this tool wear detection research, the data is obtained by vibration sensors. With the ability to continuously learn from the data and increase the accuracy of wear detection over time, AI/ML algorithms are useful tools for industry applications.
The following research aims to provide a wear detection system tool used for milling processes. Using the fewest amount of data possible, a one-shot learning regression approach is utilised to train the model to form its own conclusions about their commonalities.
The system methodology section of the study describes the experimental strategy, methods, and pre-trained model used.
3

RUL Estimation of Milling Tools through Different Learning Styles
LITERATURE:
Machining operations are crucial to the creation of high-quality products in contemporary manufacturing processes. However, the wear of the cutting tool employed in these procedures may result in a decline in machining precision, tool life, and product quality. In recent years, there has been an increase in interest in the creation of prognostic techniques to forecast the remaining useful life (RUL) of milling tools, which can help optimise the machining procedure and boost effectiveness. In addition to this, in recent years, one-shot learning algorithms have gained significant attention in the research community due to their potential for handling limited training data.
This literature review aims to explore the existing research on RUL prediction of milling tool wear and the existing research on one-shot learning approach for regression algorithm.
Main Themes and Findings:
Several studies have investigated different approaches for RUL prediction of milling tool wear, including statistical and machine learning methods. One study proposed a hidden Markov model (HMM) approach to predict the RUL of milling tools, which showed good accuracy in predicting tool wear progression (Wang et al., 2019). Another study used a support vector regression (SVR) algorithm to predict the RUL of milling tools based on acoustic emission signals, which showed promising results in a real-time monitoring scenario (Wu et al., 2018).
In addition to these methods, the use of sensors and monitoring systems for RUL prediction has also been examined in addition to these techniques. In one study, a wireless sensor network-based monitoring system for tool wear prediction was created, and it was capable of accurately predicting the RUL and detecting tool wear in real-time. (Ma et al., 2016). In a different study, a hybrid system that coupled acoustic emission signals with a finite element method (FEM) model to forecast tool wear and RUL was developed. (Liu et al., 2020).
Moving further, some researchers have proposed hybrid approaches that combine one-shot learning algorithms with other techniques for improved RUL prediction. For instance, one study proposed a hybrid model that combined a one-shot learning algorithm with a deep belief network to predict the RUL of milling tools (Liu et al., 2021). The hybrid model was able to achieve high accuracy in predicting the RUL and was robust to variations in tool wear patterns.
Similarly, several studies have investigated the use of one-shot learning algorithms for RUL prediction of milling tool wear. One study proposed a deep one-shot learning model that utilized convolutional neural networks (CNNs) to predict the RUL of milling tools (Kumar et al., 2020). The model showed high accuracy in predicting the RUL with limited training data and was able to handle variations in tool wear patterns.
Overall, however not many have implemented one-shot learning for the prediction of the Remaining Useful Life of a tool, the existing research suggests that the algorithm holds great promise for RUL prediction of milling tool wear. The ability of these algorithms to handle limited training data and variations in tool wear patterns makes them an attractive option for practical applications. However, further research is needed to evaluate the performance of these algorithms in different machining scenarios and to develop more accurate and reliable models for RUL prediction.
4

RUL Estimation of Milling Tools through Different Learning Styles
 Figure 2: Literature in Table Format
5

RUL Estimation of Milling Tools through Different Learning Styles
METHODOLOGY:
 Figure3: Outline of the Methodology of the Project
6

RUL Estimation of Milling Tools through Different Learning Styles
Dataset description:
The Tool Wear Dataset of NUAA_Ideahouse, published by: IEEE Data Port, submitted by: Yingguang Li if used for the following:
● Analysing the influence of process information on monitoring signals under the same tool wear state through signal processing methods.
● Training and testing models of tool monitoring and tool wear prediction for cutting conditions and cutting parameters.
    Sr.No
      Parameter/Description
      Specification
    1
 Milling Machine – End mill (Machining Centre)
 DMUTM 80P duoBlock
    2
       Cutting Tool
       Solid Carbide
    3
 Workpiece
 Titanium Alloy [TC4]
    4
       Feed
       0.045 (mm/r)
    5
 Spindle Speed
 1750 (r/min)
    6
       Axial Depth of cut
       2.5 mm
    7
   Maximum Allowable Flank Wear
   0.3 mm
  Figure 4: Experimental Parameters for Tool Wear Prediction: W1 case
   Sr.N o
   Parameter/Description
   Specification
    1
    Cutting Vibration
    PCBTM W356B11
    2
    Cutting Force
    Spike Sensory Tool Holder
    3
       Spindle Current and Power
       PLC
    4
 Data Acquisition box
 NITM
    5
       Tool Wear Measurement
       Microscope SinicoTM XK-T600
    6
   Synchronized Sampling Frequency
   300 mm
  7

RUL Estimation of Milling Tools through Different Learning Styles
Figure 5: Data-acquisition system and sensor specifications
Feature Extraction:
The process of choosing and translating pertinent data from raw data into a set of features that may be used for additional analysis or modelling is known as feature extraction.
Feature extraction is a critical step in data preparation for training algorithms in machine learning and data analysis. Reducing the dimensionality of the data while maintaining as much pertinent information as you can is the aim of feature extraction. The effectiveness and precision of algorithms used for tasks like classification, grouping, and regression may be enhanced as a result.
The type of data being studied and the specific task at hand can influence the feature extraction methods used. Principal component analysis (PCA), independent component analysis (ICA), wavelet transforms, and Fourier transforms are a few popular techniques. These methods can be used to locate patterns in data, eliminate noise, and extract pertinent information that can be fed into machine learning algorithms.
In the following research, the Python library TSFEL (Time Series Feature Extraction Library) is used to extract features from time series data. It offers a wide variety of feature extraction techniques that may be applied to numerous tasks, including classification, clustering, and anomaly detection. The library has the capability to extract over 60 different features from the Temporal, Spectral and Statistical domains.
Python's temporal domain is a key idea in signal and image processing and is utilised in many different applications, such as time series analysis, video processing, and machine learning.
A key idea in signal processing and image processing, the spectral domain in Python is utilised in many different applications, including audio and picture processing, machine learning, and data analysis.
The statistical domain is a key idea in data analysis and scientific research. It is utilised in a variety of applications, such as machine learning, data visualization, and decision-making.
In the following research, the following features were extracted using the TSFEL library:
    Extracted Features
Mean
Interquartile range
Formula
Mean = ∑" #
IQR = Q3 – Q1
Function
It is a measure of central tendency that represents the sum of all values in a dataset divided by the number of values in the dataset.
It is a measure of variability that is calculated as the
             8

RUL Estimation of Milling Tools through Different Learning Styles
              Median absolute deviation
Mean absolute deviation
Max
Standard deviation
Variance Skewness
Root mean square
ECDF Percentile
MAD = median(|𝑋𝑖 − 𝑚𝑒𝑑𝑖𝑎𝑛(𝑋)|)
MAD = (∑|&'()*+#(&)|) #
max = maximum value in the dataset
SD = √[∑(&'()*+#)!] (#(/)
Var = [∑(&'()*+#)!] (#(/)
G1 =- # . -∑(&'()*+#)".
difference between the third quartile (Q3) and the first quartile (Q1) of a dataset.
It is a measure of variability that is calculated as the median of the absolute deviations of a dataset from its median.
It is a measure of variability that is calculated as the average of the absolute deviations of a dataset from its mean.
To find the maximum value in a dataset, you can compare each data point to the current maximum value and update the maximum value if the data point is greater than the current maximum value.
It tells you how much the individual data points in a dataset deviate from the mean.
It measures how spread out the data points are from the mean of the dataset.
It is a measure of the asymmetry of a probability distribution. It describes how much a dataset deviates from a symmetric normal distribution.
It is a mathematical measure of the magnitude of a set of values, typically used to measure the magnitude of a varying quantity over time.
It is a statistical tool used to visualize the distribution of a dataset.
                                        (#(/)(#(0)
RMS = /0/1∑(𝑋𝑖0) #
1"
               ECDF is a step function that increases by 1/n at each data point, where n is the sample size
   9

RUL Estimation of Milling Tools through Different Learning Styles
       Histogram
Median
Min
In a histogram, the range of the data is divided into a set of intervals, called bins, and the number of data points that fall into each bin is counted.
Median (position) = #3/ 0
min = minimum value in the dataset
It represents the frequency or count of data points that fall within each bin of the histogram.
It is a measure of central tendency that represents the value that separates the lower half of a dataset from the upper half.
To find the minimum value in a dataset, you can compare each data point to the current minimum value and update the minimum value if the data point is less than the current minimum value.
                 Figure 6: Table to show the extracted features, their formulas and functions via the TSFEL library
Feature Extraction in time and frequency domains:
Depending on the type of data and the particular analysis being done, feature extraction can be done in both the time domain and the frequency domain.
Feature extraction in the time domain entails examining the raw data in its original time- series format. As mentioned earlier, this can include methods like statistical measurements, signal envelope, autocorrelation, and wavelet transform.
After the data has been translated into the frequency domain using methods like Fourier transforms, feature extraction in the frequency domain entails examining the data. By doing so, it may be possible to spot patterns or other aspects of the data that are not obvious in the time domain.
The following are some typical methods for frequency domain feature extraction:
● Estimating the signal's power spectral density (PSD), which depicts the distribution of power across frequencies, is required in this step. The frequency components that are most crucial for the analysis can be found using the PSD.
● The amount of information included in the signal's frequency distribution is measured by a property called spectral entropy. It can be applied to measure the signal's complexity and spot patterns or trends in the data.
 10

RUL Estimation of Milling Tools through Different Learning Styles
● Mel-Frequency Cepstral Coefficients (MFCCs): As explained before, MFCCs are features that may be taken from a signal's frequency-domain representation and applied to speech recognition and other tasks.
● Decomposing the frequency-domain representation of the data using a wavelet packet decomposition is what is meant by wavelet packet decomposition. This can be used to extract features from the data that reflect both its frequency and time-domain properties.
These are only a few instances of methods used for frequency domain feature extraction. The individual application and the properties of the data being examined will determine the technique to use.
Feature Selection:
To enhance the performance of a machine learning model, feature selection in coding is the act of choosing a subset of features from a larger set of features. This might be crucial in coding applications like natural language processing or picture recognition where the number of features can be very high.
In coding, there are numerous methods for feature selection, such as:
1. Recursive Feature Elimination (RFE) is a well-liked feature selection method that entails repeatedly taking out the least significant features from the initial feature set until the required number of features is obtained. Each feature's significance is determined by a machine learning algorithm.
2. Correlation-based Feature Selection (CFS) picks features with a strong correlation to the target variable but a low correlation to each other. This makes it easier to make sure the features chosen are not duplicates.
3. Mutually Based on Information Feature selection: With this method, features are chosen based on how well they know the target variable. Mutual information is a metric for how much knowledge one variable has about another.
4. By determining the most significant principal components, principal component analysis (PCA), a technique, can be used to minimise the dimensionality of the feature space. The original features that capture the most variation in the data is combined linearly to form these major components.
5. By penalising the coefficients of the least significant features in a linear model, L1 regularisation can be used to choose features. This motivates the model to choose a limited number of attributes.
The individual application and the properties of the data being examined will determine the technique to use.
 11

RUL Estimation of Milling Tools through Different Learning Styles
In the following research, Pearson Coefficient Correlation in used to select the top ten features that have a range from -1 to 1. These features are then trained and tested for further analysis.
r= ∑("#("̅)(5#(56) 7 ( " # ( " ̅ ) ! ( 5 # ( 56 ) !
Learning Style:
In the one-shot learning paradigm, a model is trained to learn from just one instances from each class. One-shot learning is more frequently employed, nevertheless, in classification problems when the objective is to categorise an input into one of multiple classes.
    Figure 7: Types of one-shot learning Algorithms
The objective of regression, on the other hand, is to predict a continuous output variable from one or more input variables. Regression problems might be amenable to one-shot learning, but it might not be as simple as it is for classification problems.
12

RUL Estimation of Milling Tools through Different Learning Styles
In one-shot regression, the model must be trained to forecast a continuous output from just one example of input-output pairings. In order to increase performance on a particular task, a model is first trained on a big dataset and then fine-tuned on a smaller dataset. This is similar to the concept of transfer learning.
Using a pre-trained model, such as a neural network, that has previously learned to extract important features from a huge dataset, could be one method for one-shot regression. A small dataset of input-output pairings might then be used to refine the model using methods like gradient descent or Bayesian optimization. Use of a meta-learning algorithm, which learns how to adapt to new tasks from a limited number of instances, could be another strategy.
It's crucial to keep in mind that one-shot learning, and particularly one-shot regression, is still a hot topic for research and might not be as well established as conventional machine learning methods. The difficulty of the issue, the amount of the dataset, and the calibre of the input-output pairs will all affect how well one-shot regression performs.
RUL Estimation:
In machine learning and deep learning for predictive maintenance, where the objective is to anticipate the interval before a component or system will fail, RUL (Remaining Useful Life) prediction is a crucial task. RUL can be accurately estimated to assist prevent unforeseen failures, save downtime, and lower maintenance costs.
In machine learning and deep learning, RUL estimation can be achieved in a number of ways, including:
● Model-based approaches: These methods estimate RUL using mathematical models, such as statistical or physics-based models. The underlying physical or statistical aspects of the system being monitored must normally be well understood in order to use these models.
● Data-driven strategies: These strategies estimate RUL based on the system's historical data using machine learning or deep learning models. These models can be trained on big datasets to increase accuracy and do not require prior understanding of the underlying physical or statistical features of the system.
● Hybrid approaches: Model-based and data-driven strategies are combined in hybrid approaches to estimate RUL. For instance, the RUL for a system in the early stages of degradation may be estimated using a physics-based model, while the RUL for a system in the latter stages of degradation could be estimated using a data-driven model.
Support vector machines, decision trees, and random forests are some common machine learning algorithms for RUL estimation. RUL estimation has also been performed using deep learning techniques including convolutional neural networks (CNNs) and long short-term memory (LSTM) networks, with encouraging outcomes.
In order to acquire pertinent data regarding the state of the system, RUL estimate utilising machine learning and deep learning typically needs high-quality data, such as sensor data and
 13

RUL Estimation of Milling Tools through Different Learning Styles
maintenance records. Furthermore, it's crucial to confirm the RUL estimations' correctness and dependability using the right metrics and validation methods.
Results:
Figure 8: mean squared error, mean absolute error and r2 score of Performance Indicators and their Domains.
Figure 9: graph above show the relationship between actual and predicted values for Random Forest in the statistical domain.
From the pre-processed data, selected and extracted features, the mean squared error, mean absolute error and r2 scores of different performance Indicators is achieved for Temporal, Statistical and Spectral domains as shown in figure 7 above.
The mean squared error (MSE) is a frequently employed metric for comparing two sets of values. It is the average of the squared discrepancies between a dataset's actual values and predicted values.
The MSE is calculated by squaring the difference between each predicted value and its matching actual value, adding up all squared differences, and then dividing by the total number of values in the dataset. The MSE formula is:
  14

RUL Estimation of Milling Tools through Different Learning Styles
MSE=/ 𝛴(𝑖=1𝑡𝑜𝑛)(𝑦' −𝑦')0 #
where n is the number of data points, 𝑦' is the ith actual value, 𝑦' is the ith predicted value.
A lower MSE indicates a better fit between the expected and actual values, which is a common way to gauge the effectiveness of a predictive model. It is crucial to combine it with other evaluation metrics because it might be sensitive to outliers and occasionally result in overfitting.
A statistic called mean absolute error (MAE) is used to assess the average size of discrepancies between expected and observed values in a collection. The average of the absolute discrepancies between the projected and actual values is used to calculate it.
The formula for MAE is:
MAE=/ 𝛴(𝑖=1𝑡𝑜𝑛):𝑦'−𝑦': #
where n is the number of data points, yi is the ith actual value, y^i is the ith predicted value.
MAE is frequently used to assess the precision of a predictive model. A lower MAE denotes a better fit between the expected and actual values, similar to MSE. Because MAE employs the absolute value of the difference between the predicted and actual values, it is less sensitive to outliers than MSE. Since MAE displays the average size of the mistakes in the same units as the original data, it is also simpler to understand than MSE.
Overall, MAE is a helpful indicator to assess a predictive model's performance, especially when the emphasis is on accuracy and interpretability rather than the impact of outliers.
The R-squared (R2) score, commonly referred to as the coefficient of determination, is a statistical indicator that shows how much of the variance in the dependent variable in a linear regression model is explained by the independent variables.
A higher value denotes a better fit between the model and the data, and the R2 score ranges from 0 to 1. Scores range from 0 to 1, where 0 means the model does not explain any variance in the dependent variable, and 1 means the model fully fits the data.
The formula for R2 score is:
R2 = 1 - 889*1 88:;:
where SSres is the sum of the squared residuals (the difference between the actual and predicted values) and SStot is the total sum of squares (the difference between the actual values and the mean value of the dependent variable).

15
RUL Estimation of Milling Tools through Different Learning Styles
A regression model's quality is frequently assessed using the R2 score, where a higher R2 value denotes a better fit between the model and the data. The model's performance may not be well predicted by this criterion if it is overfit or if there are nonlinear interactions between
the variables or if there are a number of independent variables that are sensitive to the model's number. R2 score should therefore be used in conjunction with other evaluation measures, and its findings should be carefully analysed.
Conclusion:
This article examines the data-driven predictive maintenance of milling cutting tool RUL estimate. The body of existing research demonstrates that RUL prediction is a developing field with lots of room for advancement in industry 4.0. Different feature extraction techniques, data-driven monitoring techniques, and decision-making models have all been covered by the authors. Predictive maintenance is the goal of effective RUL estimate. (PdM). Calculating a machine's RUL can be useful in planning its preventative maintenance procedures. The data signals from the milling machine are gathered by vibration sensors. and finally, in order to make an accurate prediction, the pre-processed data, chosen and extracted features, mean squared error, mean absolute error, and r2 scores of various performance indicators are obtained for the temporal, statistical, and spectral domains.
