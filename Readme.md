# Parkinson Disease Detection



# Introduction 

Parkinson's is a neurodegenarative progressive disorder disease. It affects the nervous system and the part of the body controlled by it. It appears in the part of the brain called substantia nigra. Normally these brain cells produce dopamine and these dopamine operates in a delicate balance with other neurotransmitters to help cordinate the millions of nerve and muscle cell involved in the movement. When these nerve cells die or become impaired, they lose the ability to produce the dopamine. When 60-80% of these cells are lost then enough dopamine are not produced and Parkinson's motor symptoms appear. Without enough dopamine, this balance is disrupted resulting tremor, rigidity, slowness of movement and impaired balance. So Parkinson's disease is caused by the disruption of the brain cells that produce the dopamine which allows the brain to communicate each other and control the fluency of the movement. It is thought that the disease begins many years before the motor symptoms appears and therefore, researchers are looking for ways to recognize the non-motor symptoms that appear early in the disease as early as possible, thereby halting the progression of the disease. A person suffering from the Parkinson's can have following symptoms:

*Tremor*

*Slowed movement*

*Rigid muscle*

*Impaired posture*

*Loss of automatic movement*

*Speech change*

*Writing change*

*Impaired posture*

Also, Parkinson's disease can have other symptoms that include:

*Depression*

*Anxiety*

*Sleeping and memory-related issues*

*Loss of sense of smell along with balance problems*

The symptoms of Parkinson's disease can be different from patient to patient. Early sign of the disease can be mild and can go unnoticed. Symptoms often begin on one side of your body and usually remain worse on that side. Sometimes it is difficult to detect whether there is Parkinson's disease present in the patient's body. Parkinson's disease if detected in the early stage will be curable, and will be time and cost effective, but there is no effective treatment in the advanced stage.



# Dataset 

The dataset used in this project is from UCI machine learning data bank. The dataset has 24 columns, thus we need to reduce the dimension before we train the data. The target or independent variable is "status" with binary values of 0 and 1. Status values for healthy person and PD person are 0 and 1 respectively.m The goal of this project is to develope the best machine learning model to predict the Parkinson's disease so that we can treat the patient in the timely manner. The following are the columns in the dataset.

**name**: This column represents the name of the patient. It serves as an identifier and is not directly related to the voice measurements.

**mdvp:fo(hz)**: This column represents the fundamental frequency of the voice measured in hertz (Hz). It indicates the rate at which the vocal folds vibrate, which is a key parameter for voice production.

**mdvp:fhi(hz)**: This column represents the highest frequency component in the voice measured in hertz (Hz). It provides information about the upper limit of the vocal range.

**mdvp:flo(hz)**: This column represents the lowest frequency component in the voice measured in hertz (Hz). It provides information about the lower limit of the vocal range.

**mdvp:jitter(%)**: This column represents the percentage of local frequency variation in the voice signal. It reflects the irregularity of vocal fold vibrations.

**mdvp:jitter(abs)**: This column represents the absolute value of the jitter measurement. It provides a quantification of the absolute frequency variation in the voice signal.

**mdvp:rap**: This column represents the relative amplitude perturbation in the voice signal. It measures the difference between consecutive peak amplitudes.

**mdvp:ppq**: This column represents the five-point period perturbation quotient. It measures the variations in the voice signal's cycle lengths.

**jitter:ddp**: This column represents the average absolute difference of differences between consecutive periods. It provides a measure of irregularities in the voice signal's cycle lengths.

**mdvp:shimmer**: This column represents the variation in amplitude of the voice signal. It reflects the presence of fluctuations or shimmer in the voice.

**mdvp:shimmer(db)**: This column represents the shimmer measurement in decibels (dB). It provides a quantification of the amplitude variation in the voice signal.

**shimmer:apq3**: This column represents the amplitude perturbation quotient for the first three harmonics. It measures the irregularities in the amplitude of specific frequency components.

**shimmer:apq5**: This column represents the amplitude perturbation quotient for the first five harmonics. It provides a measure of the irregularities in the amplitude of specific frequency components.

**mdvp:apq**: This column represents the amplitude perturbation quotient, which is the average absolute difference between consecutive amplitude periods. It quantifies the variations in the amplitude of the voice signal.

**shimmer:dda**: This column represents the average absolute differences of adjacent differences between consecutive amplitude periods. It provides a measure of the presence of shimmer in the voice signal.

**nhr**: This column represents the ratio of noise to harmonic components in the voice signal. It indicates the level of background noise in the voice.

**hnr**: This column represents the ratio of the energy in the harmonics to the energy in the noise. It provides an estimate of the clarity of the voice signal.

**status**: This column represents the binary target variable indicating the presence (1) or absence (0) of Parkinson's disease in the patient.

**rpde**: This column represents the nonlinear dynamical complexity measure of the voice signal. It quantifies the degree of determinism and predictability in the voice.

**dfa**: This column represents the detrended fluctuation analysis measure of the voice signal. It provides information about the presence of long-term correlations in the voice signal.

**spread1**: This column represents a nonlinear measure of the fundamental frequency variation. It quantifies the nonlinear dynamic behavior of the voice.

**spread2**: This column represents a nonlinear measure of the amplitude variation in the voice signal. It provides additional information about the nonlinear dynamics of the voice.

**d2**: This column represents the correlation dimension of the voice signal. It quantifies the complexity and structure in the voice signal.

**ppe**: This column represents the pitch period entropy of the voice signal. It provides information about the unpredictability of pitch periods.

**Citation - 'Exploiting Nonlinear Recurrence and Fractal Scaling Properties for Voice Disorder Detection', Little MA, McSharry PE, Roberts SJ, Costello DAE, Moroz IM. BioMedical Engineering OnLine 2007, 6:23 (26 June 2007)**


# Steps Taken in Notebook (There are two notebooks: 1 for the EDA and the other for the modelling)

Exploratory Data Analysis

Feature Engineering

Train Test Split

Scaling the Data

Balancing the Dataset

Model Evaluation Function using Accuracy score, Confusion Matrix and Kappa score

Logistic Regression

Decision Tree

Random Forest

Gradient Boosting

XG boosting


# Conclusion 

The evaluation of the models was done using the evaluate_classification_model function, which provided a confusion matrix, accuracy score, and kappa score. 


The results showed that both Gradient Boosting and XG Boost achieved high accuracy and kappa scores, with over 88% accuracy and a kappa score of over 80%.

The slides can be found in the slides folder.



