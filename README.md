# Primate-Splice-Junction-Gene-Sequences-DNA-With-Associated-Imperfect-Domain-Theory
LSTM deep learning model to detect DNA sequence types (EI or IE) using python with accuracy 95%


Learn how to manipulate data in a .txt file and convert it to .xlsx or .csv .
Overview of deep learning.
What is LSTM and why is used?
Long Short-Term Memory (LSTM) networks are a type of recurrent neural network (RNN) capable of learning order dependence in sequence prediction problems. This is a behavior required in complex problem domains like machine translation, speech recognition, and more. LSTMs are a complex area of deep learning.

Text data was downloaded from UCI.com .
Text data was converted to excel sheet.
Excel sheet data was processed.
LSTM model application.
Python programming language used.
Google Colab Cloud Used for the need of GPU.

Title of Database: 
Primate splice-junction gene sequences (DNA)  with associated imperfect domain theory.

Video Clarification:
Introns and Exons Difference.
Link: https://www.youtube.com/watch?v=YtKoTOCJGt4

Problem Description: 
Splice junctions are points on a DNA sequence at which `superfluous' DNA is  removed during the process of protein creation in higher organisms.
 The problem posed in this dataset is to recognize, given a sequence of DNA, the  boundaries between exons (the parts of the DNA sequence retained after  splicing) and introns (the parts of the DNA sequence that are spliced  out). 
This problem consists of two subtasks: recognizing exon/intron  boundaries (referred to as EI sites), and recognizing intron/exon boundaries  (IE sites). (In the biological community, IE borders are referred to a ``acceptors'' while EI borders are referred to as ``donors''.)

About The Dataset:
Number of Instances: 1535. 
Number of Attributes: 61   -- class (one of EI, IE)   -- instance name   -- 60 sequential DNA nucleotide positions
1)One of {EI ,IE}, indicating the class.             
2)The instance name.          
3-62)The remaining 60 fields are the sequence, starting at position 30 and ending at position +30. 
Each of these fields is almost always filled by one of  {A, G, T, C}. 

Other characters indicate ambiguity among the standard characters according to the following table:			
character	    meaning			

D		          A or G or T	

N             A or G or C or T			

S             C or G	

R		         A or G

Missing Attribute Values: none.

Class Distribution: 	
EI:       767  (49.9%)     ---   IE:       768  (50.1%)

Shape of Dataset Text File :
![image](https://user-images.githubusercontent.com/112272836/193588561-8bfbda9e-d9f8-4029-9363-e9588b94a432.png)

How Data was Processed?
Prediction Column:
Each EI was converted to a 0 --
Each IE was converted to a 1 --
Attributes:
Our data set has constant DNA sequences of length 60 --
So 60 attributes were created having its indices  --
Each A was converted to 0 --
Each C was converted to 1 --
Each G was converted to 2 --
Each  T was converted to 3 --

What about Garbage?
It was mentioned in the data description that there is no garbage, instead there are some inaccurate values, for example:
character	    meaning			

D		          A or G or T	

N             A or G or C or T			

S             C or G	

R		         A or G

Problem solved by creating an array for each of these four letters including their expected values and a random one was chosen each time from each array at run time .


After Conversion to Excel File and Processing it: 
![image](https://user-images.githubusercontent.com/112272836/193588848-ab37e5dc-5219-46ac-b347-b77aafaefcee.png)

Applying LSTM model:

Train data was 70% and test was 30% --
Sigmoid activation function used --
Epochs =100 and batch size=20 --
Optimizer Adam used --
Loss function binary crossentropy used --
Accuracy was 94.58% --


![image](https://user-images.githubusercontent.com/112272836/193588948-0090eed9-2252-46c6-9544-547aedd695bc.png)



![image](https://user-images.githubusercontent.com/112272836/193588967-79b66800-30be-46a7-ae0a-558668a1e7d8.png)




