# NLP-Assignment3

# Answer 1 

We have selected the **Llama3.2-1B** model

# Answer 2

For Llama3.2-1B

Total Parameters: 1,235,814,400

Trainable Parameters: 1,235,814,400

# Answer 3 

a. The fine tuned code of classification SST-2 can be found in the fine-tuningsst2-1922ee.ipynb

b. The fine tuned code of Question- Answering SQuAD can be found in finetuning-Squad.ipynb    

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


# Answer 5
Number of parameters in pre-trained model: **1,235,814,400**

Number of parameters in fine tuned model of classification SST-2: **1,235,815,600**

Number of parameters in fine tuned model of classification SQuAD: **1,235,815,900**

The number of parameters in pre-trained model and fine-tuning model are almost same
with negligible difference. 

# Answer 6

**Hugging Face link** - https://huggingface.co/HarshitBK/FineTuneModel-Llama/tree/main

# Answer 7

a. **Lower or Higher Scores in the Metrics**

**1. Zero-Shot Model Metrics**

The zero-shot scenario indicates the performance of the model without any task-specific training on the SST2 dataset.

Accuracy (54.58%): The model's overall correctness is relatively low, close to a random guess for binary classification, as it lacks domain-specific adaptation.
Precision (55.54%): The model identifies positive instances with moderate precision, indicating many false positives in its predictions.
Recall (94.11%): The high recall shows that the model captures almost all positive instances but at the expense of precision. This suggests it labels many instances as positive, resulting in fewer false negatives.
F1 Score (69.86%): A weighted harmonic mean of precision and recall indicates that the high recall boosts the F1 score but is limited by moderate precision.
Reason for Lower Scores:

The model is relying on its generalized pre-trained knowledge, which may not align well with the SST2 dataset’s sentiment classification task.
Lack of exposure to SST2-specific nuances leads to suboptimal classification decisions.

**2. Fine-Tuned Model Metrics**

The fine-tuned scenario indicates the performance after adapting the model specifically to the SST2 dataset.

Accuracy (95.11%): Significant improvement demonstrates that the model has learned task-specific patterns and sentiment-related features.
Precision (95.67%): High precision indicates the model is much better at avoiding false positives, assigning positive labels more correctly.
Recall (95.58%): Recall remains high, meaning the model still identifies most positive instances.
F1 Score (95.62%): A high F1 score indicates a strong balance between precision and recall, showcasing the model’s reliability in handling the task.
Reason for Higher Scores:

Fine-tuning exposes the model to SST2-specific training data, allowing it to align its weights and representations with the task.
The model better understands the dataset's context and nuances, leading to a significant reduction in false positives and false negatives.

b. **Understanding from the Number of Parameters Between Pretraining and Fine-Tuning**

Number of parameters almost the same with negligible difference. The model architecture does not change during fine-tuning. 
The same parameters are adjusted to optimize task-specific objectives. Thus, the total number of trainable parameters remains consistent between the pre-trained and fine-tuned versions.
During fine-tuning, only a subset of the model's pre-trained knowledge is specialized for the target task. 
This demonstrates how pre-training captures general knowledge, while fine-tuning adapts this knowledge for specific tasks without requiring additional parameters.

c.  **Performance Difference for Zero-Shot and Fine-Tuned Models**

The performance of the Llama model in zero-shot and fine-tuned settings has distinct capabilities and limitations. 

In the zero-shot setting, the pre-trained model benefits from its training on diverse datasets, enabling it to handle a wide range of tasks with decent general-purpose knowledge. However, it may struggle with task-specific nuances, such as detecting subtle sentiment shifts in SST-2 or understanding precise contexts in SQuAD questions, leading to errors. 

Fine-tuning the model on task-specific data significantly improves its performance by aligning predictions with the requirements of the task, such as achieving higher accuracy in sentiment analysis or better exact-match scores in question-answering. This specialization allows the model to recognize patterns and linguistic nuances tailored to the task. However, fine-tuning also introduces challenges, such as reduced generalization to out-of-distribution data and the potential for overfitting, which can degrade test performance. 

# Contributions
1. Harshi - Slected the model and calculated the number of parameters of the selected model.
2. Rushi - Fine tuned the pre-trained model for SST-2 classification task and calculated the scores of classification metrics.
3. Hirva - Fine tuned the pre-trained model for SQuAD and calculated the score of its metrics.
4. Harshit and Khushal - Calculated the parameters after fine tuning, uploaded it on the hugging face and also answered Q7. 
        Further, created and updated the github repository.

