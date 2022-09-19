# WeRateDog-Tweet-Analysis

## Dataset

There were 3 data required for this investigation, an image prediction data called image_prediction_final which was in url format containing information about dog breed predictions, a tweeter_achieve in csv format containing dog ratings, dog age stage, and other useful information, the third file is an extracted tweeted json file called data_json containing tweeter retweet and favorite counts among other useful information.

* image_prediction_final: This file was extracted using the request python library and applying request.get method on the url link to programmatically access the information in the url, the tabs were separated by applying the sep = '\t' function.

* tweeter_achieve: This csv data was imported into the anaconda environment through upload and then imported into the python notebook using the pandas dataframe and applying the pd.read_csv method on the csv file.

* data_json: Due to authentification issues, I was unable to query the twitter API directly, however I have included the API query code that I would have used for the twitter API query if I had the right keys and token. To overcome this challenge, the twitter json data was provided by Udacity instructor. The provided data was a txt file, I read the files using readlines() method, opened an empty dataframe, then appended the contents of the txt file to the empty dataframe, I then converted the resulting data into a dataframe by applying pd.DataFrame method on it.
