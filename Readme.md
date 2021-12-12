## Transfer Learning ##

Transfer learning is a technique that focuses on storing knowledge gained while solving one problem and applying it to a different but related problem.   
For example, knowledge gained while learning to recognize fruits could apply when trying to recognize fruit vendors/vegetables/baskets etc.  
Effective in :  
- Image Classification,  
- Object Detection,  
- Instance segmentation,  
- NLP.  
  
One common approach is using a model pre-trained on millions of data poins and then fine-tuning it on a small subset of new problem's data points. It also used for fixed feature-extraction scenarios.  
  
Example: VGG - 16   
<img width="727" alt="Screenshot 2021-11-21 at 4 48 53 PM" src="https://user-images.githubusercontent.com/61674750/142759738-39b17d53-99aa-4e05-bf7f-0de287fc5459.png">  
  
Fixed Feature Extractor Architecture:  
Type 1:  
<img width="729" alt="Screenshot 2021-11-21 at 8 03 11 PM" src="https://user-images.githubusercontent.com/61674750/142766127-49b27d09-d7fa-4914-b6a3-70fabb762f3d.png">  
  
 Type 2:   
 <img width="727" alt="Screenshot 2021-11-21 at 8 03 50 PM" src="https://user-images.githubusercontent.com/61674750/142766148-68be10fd-ee1b-4a12-8def-bbf7b25b493d.png">
  
Pytroch's Autograd :   
<img width="738" alt="Screenshot 2021-11-21 at 8 13 57 PM" src="https://user-images.githubusercontent.com/61674750/142766571-904e62c8-fc46-4f52-8d2a-21c375f5c774.png">  
Itself calculates the loss in forward pass and it's gradients wrt weights, in the backward pass.



Learning Rates :  
- Adam optimiser : experimental values suggest 3e-4 being a good guesstimate for fine-tuning.
