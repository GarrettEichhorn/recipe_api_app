## API Documentation  

Access the API here: [Reciperfect API](https://reciperfect.herokuapp.com/)  

-----

The API references a pre-built dataset that scrapes recipes from a few of my favorite online sources. You can review the methodology and sites in the main repository [here](https://github.com/GarrettEichhorn/recipe_generator).  

To search the recipe dataset, enter your query "/api/search/**query**". The API will return all recipes that contain the **query**, ranked by relevance and returned in JSON format.  This is achieved using the [TF-IDF vectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html) and [cosine similarity](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html).

#### Example: search for recipes containing "chicken"...

[https://reciperfect.herokuapp.com/api/search/chicken](https://reciperfect.herokuapp.com/api/search/chicken)
