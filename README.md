# Long-Short-Term-Memory for Sentence Generation

In this project, a sentence generator is developed using LSTM modules. To optimize the final model, there are several aspects that can be optimized. Among those aspects, Hidden Dimension, Number of Layers, Embedding Dim, and Learning Rate was studied.

# Case Study
In case studies other parameters of the model was fixed to ensure accurate comparision.

<table>
  <tr>
    <td> Model name </td>
    <td> H10 </td>
    <td> H100 </td>
    <td> S1</td>
    <td> S5 </td>
    <td> E50 </td>
    <td> E200 </td>
    <td> LR0.1 </td>
    <td> LR0.01 </td>
  </tr>
  <tr>
    <td> Embedding Size </td>
    <td> 50 </td>
    <td> 50 </td>
    <td> 50</td>
    <td> 50 </td>
    <td> 50 </td>
    <td> 200 </td>
    <td> 50 </td>
    <td> 50 </td>
  </tr>
  <tr>
    <td> Hidden Layer Size </td>
    <td> 10 </td>
    <td> 100 </td>
    <td> 10</td>
    <td> 10 </td>
    <td> 10 </td>
    <td> 10 </td>
    <td> 10 </td>
    <td> 10 </td>
  </tr>
  <tr>
    <td> Number of Layers </td>
    <td> 2 </td>
    <td> 2 </td>
    <td> 1</td>
    <td> 5 </td>
    <td> 2 </td>
    <td> 2 </td>
    <td> 2 </td>
    <td> 2 </td>
  </tr>
  <tr>
    <td> Batch Size </td>
    <td> 256 </td>
    <td> 256 </td>
    <td> 256</td>
    <td> 256 </td>
    <td> 256 </td>
    <td> 256 </td>
    <td> 256 </td>
    <td> 256 </td>
  </tr>
   <tr>
    <td> Epochs </td>
    <td> 50 </td>
    <td> 50 </td>
    <td> 50</td>
    <td> 50 </td>
    <td> 50 </td>
    <td> 50 </td>
    <td> 50 </td>
    <td> 50 </td>
  </tr>
  <tr>
    <td> Learning Rate </td>
    <td> 0.10 </td>
    <td> 0.10 </td>
    <td> 0.10 </td>
    <td> 0.10 </td>
    <td> 0.10 </td>
    <td> 0.10 </td>
    <td> 0.10 </td>
    <td> 0.01 </td>
  </tr>
</table>

## Hidden Dimension
 - perplexity reduction speed is the same for both models
 - H10 converges sooner than H100
 - H100 has a better performance on the test split compared with H10
 - H100 generates more accurate sentences compared with H10
 
![Hidden Image](https://github.com/SajjadPSavoji/Language_Modelling_LSTM/blob/main/Asset/Screen%20Shot%202022-09-28%20at%203.04.51%20PM.jpeg)

## Number of Layers
 - perplexity reduction speed is NOT the same for both models
 - E50 has a better convergence properties compared with E200
 - E200 has a better performance on the test split compared with E50
 - E50 generates more accurate sentences compared with E200
 
![Hidden Image](https://github.com/SajjadPSavoji/Language_Modelling_LSTM/blob/main/Asset/Screen%20Shot%202022-09-28%20at%203.05.07%20PM.jpeg)

## Embedding Dimension

 - perplexity reduction speed is the same for both models
 - convergance speed is the same for both models
 - S1 has a better performance on the test split compared with S5
 - S1 generates more accurate sentences compared with S5

![Hidden Image](https://github.com/SajjadPSavoji/Language_Modelling_LSTM/blob/main/Asset/Screen%20Shot%202022-09-28%20at%203.05.22%20PM.jpeg)

## Learning Rate

 - perplexity reduction speed is more for LR0.1 compared with LR0.01
 - LR0.1 has a better convergence properties compared with LR0.01
 - LR0.1 has a better performance on the test split compared with LR0.01
 - LR0.1 generates more accurate sentences compared with LR0.01

![Hidden Image](https://github.com/SajjadPSavoji/Language_Modelling_LSTM/blob/main/Asset/Screen%20Shot%202022-09-28%20at%203.05.38%20PM.jpeg)

## Resources
* [Dataset Explained](https://www.reddit.com/r/MachineLearning/comments/ji7y06/p_dataset_of_196640_books_in_plain_text_for/)
* [Dataset(download)](https://the-eye.eu/public/AI/pile_preliminary_components/books1.tar.gz)
* [Intro to Pytorch for NLP](https://pytorch.org/tutorials/beginner/nlp/pytorch_tutorial.html#sphx-glr-beginner-nlp-pytorch-tutorial-py)
* [Intro to Pytorch for BOW](https://pytorch.org/tutorials/beginner/nlp/deep_learning_tutorial.html#sphx-glr-beginner-nlp-deep-learning-tutorial-py)
* [Intro to LSTM in Pytorch](https://pytorch.org/tutorials/beginner/nlp/deep_learning_tutorial.html#sphx-glr-beginner-nlp-deep-learning-tutorial-py)
* [Intro to Word Embedding in Pytorch](https://pytorch.org/docs/stable/generated/torch.nn.Embedding.html)
* [Intro to GRU in Pytorch](https://pytorch.org/docs/stable/generated/torch.nn.Embedding.html)
* [Intro to Glove module](https://pytorchnlp.readthedocs.io/en/latest/source/torchnlp.word_to_vector.html)
