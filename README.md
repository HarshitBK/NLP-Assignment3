# NLP-Assignment3

# Answer 1 

We have selected the **Llama3.2-1B** model

# Answer 2

For Llama3.2-1B

Total Parameters: 1,235,814,400

Trainable Parameters: 1,235,814,400

# Answer 3 

a. The fine tuned code of classification SST-2 can be found in the fine-tuningsst2.ipynb

b. The fine tuned code of Question- Answering SQuAD can be found in .ipynb       

# Answer 4
Scores for the metrics on the test split are-

a. 
**Zero-shot Model Metrics:**

Accuracy: 0.5458054936896808

Precision: 0.5554336754681501

Recall: 0.9410593389088012

F1: 0.6985612928655893

**Fine-tuned Model Metrics:**

Accuracy: 0.9510764662212323

Precision: 0.9566834972096732

Recall: 0.955794504181601

F1: 0.9562387940766319

b.
**Zero-shot Model Metrics:**


**Fine-tuned Model Metrics:**


# Answer 5
Number of parameters in pre-trained model: **1,235,814,400**

Number of parameters in fine tuned model of classification SST-2: **1,235,814,400**

Number of parameters in fine tuned model of classification SQuAD: 

The number of parameters in pre-trained model and fine-tuning model are not same.

# Answer 6

**Hugging Face link** - https://huggingface.co/HarshitBK/FineTuneModel-Llama/tree/main

# Answer 7
b. **Understanding from the Number of Parameters Between Pretraining and Fine-Tuning**

Number of parameters remains the same. The model architecture does not change during fine-tuning. 
The same parameters are adjusted to optimize task-specific objectives. Thus, the total number of trainable parameters remains consistent between the pre-trained and fine-tuned versions.
During fine-tuning, only a subset of the model's pre-trained knowledge is specialized for the target task. 
This demonstrates how pre-training captures general knowledge, while fine-tuning adapts this knowledge for specific tasks without requiring additional parameters.

c. 

# Contributions
1. Harshi - Slected the model and calculated the number of parameters of the selected model.
2. Rushi - Fine tuned the pre-trained model for SST-2 classification task and calculated the scores of classification metrics.
3. Hirva - Fine tuned the pre-trained model for SQuAD and calculated the score of its metrics.
4. Harshit and Khushal - Calculated the parameters after fine tuning, uploaded it on the hugging face and also answered Q7. 
        Further, created and updated the github repository.

