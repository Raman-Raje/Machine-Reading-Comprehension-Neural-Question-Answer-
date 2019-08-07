# About Dataset:
Data Stanford Question Answering Dataset (SQuAD) is a reading comprehension dataset, consisting of questions posed by crowdworkers on a set of Wikipedia articles, where the answer to every question is a segment of text, or span, from the corresponding reading passage, or the question might be unanswerable. You can download this dataset here https://rajpurkar.github.io/SQuAD-explorer/

**SQuAD 1.1:** The previous version of the SQuAD dataset, contains 100,000+ question-answer pairs on 500+ articles.

# Standford Attentive Reader
Implemented standford attentive reader model using keras.

# Problem Statement
Predicting the right answer for the given question and context.

# Blog:
I have written a detailed post regarding this on medium. You can read it here https://medium.com/@raman.shinde15/neural-question-and-answering-using-sqad-dataset-and-attention-983d3a1dd42c


# Observations:
1. Obtained micro f1_score of **40.33%** on test data.
2. **Algined question embedding and f_exact match** found to be the moset effective as mentioned in paper
3. f1_score can be further improoved by adding Algined question embedding feature to context.
4. Algined question embedding was omitted due to computational power limits
5. Algined question embedding was omittited because, training on 1 epoch was taking more than 5 hours.
6. Performance can be improoved further by considering:
    1. All the data points 
    2. Taking 128 units and 3 Layer of Bi_LSTM as mentioned in paper.
    3. Considering Algined question embedding + f_exact together.
   

# Summary:
 
 |                   Features                  | Accuracy | micro f1 score | macro f1 score |
 
 | question + context + POS + TF + Exact_lemma |  0.308   |     0.403      |     0.306      |
 
