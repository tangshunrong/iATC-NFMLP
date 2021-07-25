# iATC-NFMLP

## Introduce

  A novel multi-label classifier, based on molecule similarity, structure and multilayer perceptron, is for the drug ATC label prediction in first layer. Use molecule fingerprint and network embedding as feature, MLP as classification method.                                                       
  
  Used drug-related information in STITCH and KEGG, which consists of seven drug networks. Mashup, a powerful network embedding algorithm, is used to extract information-rich drug features. ECFP fingerprint extraction method is for structure vectors.                                                          
  
  The obtained feature is feed into a MLP classifier. The classifier is modified in activation function to adapt the multi-label classification. The network structure is in the figure.                                                                           
  
  Through 10-cross validation, the absolute true and accuracy are 78.35% and 82.34% respectively. Through jackknife validation, the absolute true and accuracy are 79.27% and 82.76% respectively.                                                                

                                                     
                                    


<div align=center><img src="https://github.com/tangshunrong/iATC-NFMLP/blob/main/iATC-NFMLP.jpg" width="1100" height="650" />
</div>


## Requirements
#### Tensorflow Version 1.15   
#### Keras Version 2.2.4
#### Python Version 3.6

#### Mashup runtime: 
Matlab2016a                                         
Reference: https://github.com/zhou256/iATC-NRAKEL


## Running Method
### 10-cross                                                                                        
Run “0.10Cross-training”, “1.10Cross validation”, “2.Result calculation” in order respectively. The instructions are in the code comments. 
### Jackknife
Unzip the “0.run.zip” file, and run “1.run.bat”, the program will run for 3-4 days. After that, you will get a result file containing 3883 prediction results. Then use the results for validation. The validation code is in “1.val” folder. 

## Other Info
Network embedding dataset and Mashup algorithm are from: https://github.com/zhou256/iATC-NRAKEL

