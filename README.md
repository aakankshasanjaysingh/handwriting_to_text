# handwriting_to_text
This project is about recognising handwritten words with CNN and Bi-directional GRU, decoded with CTC.

## Dataset:
The IAM Handwriting dataset I have used contains 115,320 isolated and labeled images of words by 657 seperate writers.

<i>IAM words dataset can be downloaded from <a href=http://www.fki.inf.unibe.ch/databases/iam-handwriting-database>here</a>. There's also a labelled dataset available for images of lines.</br></i>

## Results:

Test image following the predicted text are shown below:

<ol>

<div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/g06-037k-01-02.png"/></a></a><p>all</p></div></li>

 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/d03-112-01-03.png"/></a></a><p>Kings</p></div></li>
 
  <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/g07-038-01-02.png"/></a><p>SGhigraphies</p></div></li>
  
 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/l04-098-00-06.png"/></a></a><p>and</p></div></li>

 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/b05-098-03-06.png"/></a></a><p>SI</p></div></li>
 
  <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/a01-122-05-06.png"/></a></a><p>SIt</p></div></li>
  
 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/a03-030-04-05.png"/></a></a><p>the</p></div></li>
 
 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/e04-004-04-01.png"/></a></a><p>show</p></div></li>
 
 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/k04-017-08-07.png"/></a></a><p>Gcertain</p></div></li>

</ol>

Yes, the results aren't very promising and only about 59% of the images in test set were identified correctly out of all images of words in the test/unseen set. I presume this is happening because of something improper in gates of GRU. 

Although such mistakes in spellings can be corrected using a language model. My colab session had crashed (12.72GB of RAM filling up completely) everytime I tried to import pre-trained language model(I was trying to use 'Google Billion words' dataset). And for this reason, I have uploaded the jupyter notebooks without having corrected the spellings. Yes, I do have plans to fix this in the future using Virtual Machines on cloud.


## Training:
Trained on GPU on Google Colab with <a href=https://www.tensorflow.org/api_docs/python/tf/keras>tensorflow.keras</a> and took around 9 hours to complete.


