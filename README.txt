NOTE: To run this example, you need to download the Yelp dataset:

https://www.yelp.com/dataset/download

After you download the file from Yelp, you'll need to unextract it:

cd ~/Desktop/project_code/14_training_a_text_classifier/
tar -xvf ~/Downloads/yelp_dataset.tar

Then you can run the format_dataset.py script. After that, the model can be trained using fasttext:

fasttext supervised -input fasttext_dataset_training.txt -output reviews_model_ngrams -wordNgrams 2

Then, you'll be able to run the final use_model.py script.