# CIL_Project
## What to do before running CIL-Notebook.ipynb
* [Tutorial](https://github.com/kpe/bert-for-tf2)
* Download Twitter Dataset from Kaggle Competition Page and put in a folder named twitter-datasets in the folder CIL.
* Download from https://github.com/google-research/bert either the bert_base Model or the bert_large_wwm Model (Whole Word Masking) and put it in the folder CIL/bert/checkpoints/bert_base or CIL/bert/checkpoints/bert_large_wwm.
* To run everything now on Google Colab, upload everthing to your Google Drive and then run the Notebook on TPUs if available.
## Other resources/papers
* [Trainig data set](https://www.kaggle.com/kazanova/sentiment140)
* [Google's T5](https://arxiv.org/pdf/1910.10683.pdf) instead of BERT?
  * [Announcement with Colab Link](https://ai.googleblog.com/2020/02/exploring-transfer-learning-with-t5.html)
  * [Huggingface implementation](https://huggingface.co/transformers/model_doc/t5.html)
* [Albert](https://ai.googleblog.com/2019/12/albert-lite-bert-for-self-supervised.html) instead of BERT
* [GPT-3](https://arxiv.org/abs/2005.14165) is not much different to GPT-2 for much training and not available to public.
* [Preprocessing](https://trec.nist.gov/pubs/trec28/papers/DICE_UPB.IS.pdf)
  * Stop-words, URLs, usernames and unicode-characters are removed
  * Extra white-spaces, repeated full stops, question marks and exclamation marks are removed.
  * Emojis were converted to text using the python libraryemoji4
  * Lemmatization,  restoring  language  vocabulary  to  general  form  (can  express  completesemantics) by WordNetLemmatizer5.
  * Finally all tweet tokens are converted to lower-case.
* [Sample project on COVID](https://arxiv.org/pdf/2005.07503.pdf)
* MoNoise [Model](https://www.aclweb.org/anthology/P19-3032.pdf) [Rules](https://arxiv.org/pdf/1710.03476.pdf)
 * For  each  word  we  find  the  top  40  closest  candidates  in  thevector space based on the cosine distance
 * We use the [Aspell](http://aspell.net/) spell checker to repair typographical errors
 * We generate a list of all replacement pairs occurring in the training data. 
 * We include a generation module thatsimply searches for all words in the Aspell dictionary which start with the character sequence of ouroriginal word.  To avoid large candidate lists.
 * We generate word splits by splitting a word on every possible position and checking if bothresulting words are canonical according to the Aspell dictionary.
* [MoNoise alternative](https://arxiv.org/pdf/1904.06100.pdf)
* [Lexical Normalization with BERT](https://www.aclweb.org/anthology/D19-5539.pdf)
* [Twitter Fine-Tuning BERT](https://arxiv.org/pdf/1905.05583.pdf)
* [Adverserial NLP Overview](https://www.aclweb.org/anthology/N19-5001/)
* [Adverserial with RNNs](https://www.aclweb.org/anthology/L18-1584.pdf)
  
