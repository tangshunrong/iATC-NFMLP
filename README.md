# iATC-NFMLP

## Introduce

  A novel multi-label classifier, iATC-NFMLP, is proposed to identify classes in the first level of Anatomical Therapeutic Chemicals (ATC) classification system for given drugs. It adopts features derived from seven drug networks and fingerprints to encode drugs and multilayer perceptron as the prediction engine.                                                                                                            

  Through 10-fold cross-validation, the absolute true and accuracy are 78.35% and 82.34% respectively. Through jackknife test, the absolute true and accuracy are 79.27% and 82.76% respectively, higher than previous classifiers.                                                                
                                                            

                                                     
                                 
<div align=center><img src="https://github.com/tangshunrong/iATC-NFMLP/blob/main/iATC-NFMLP.jpg" width="1100" height="650" />
</div>


## Requirements
#### Tensorflow Version 1.15   
#### Keras Version 2.2.4
#### Python Version 3.6
#### Jupiter Notebook Version 6.3.0

## Running Method
### 10-fold cross-validation                                                                                        
Run “0.10Cross-training”, “1.10Cross validation”, “2.Result calculation” in order respectively. The instructions can be found in a file “Readme.txt” in the fold “10Cross”.                                                                                                     

### Jackknife test
Unzip the “0.run.zip” file, and run “1.run.bat”, the program will run for 3-4 days(using RTX2070). After that, you will get a result file containing 3883 prediction results. Then use the results for validation. The validation code is in “1.val” folder. The instructions can be found in a file “Readme.txt” in the fold “jackknife”.                                                                                                     

## Other Information
Network embedding dataset and Mashup algorithm are from: https://github.com/zhou256/iATC-NRAKEL

