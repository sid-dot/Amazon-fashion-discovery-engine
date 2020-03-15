# Amazon-fashion-discovery-engine (Content based Recommendation System).

<b>Sumamry of the project:-</b>

Problem Statement: Given a product chosen by the customer, Recommended top 10 similar based products.
                                        <b>      Project Pipeline:-   </b>
1. <b>Data Acquisition. </b> --> Aquired a data using <b>Product Advertising API </b>
2. <b>Data Cleaning.</b>
                    a.) Missing Value finding and replacing
                    b.) Understanding Duplicate products and hence removing them. (Because training a model with duplicate products(same product with different colors, sizes, etc.) doesn't make sense.
                    c.) Balanced or imbalanced Data checking ---> Data is well balanced to start with.
3. <b>Text-Processing</b> 
                    a.) Tekenization and Stopword removal.
                    b.) Stemming --> We tried using stemming on our titles and it didnot work very well. 
4. <b>Text-based Product recommendations.</b>
         * Bow (Bag of words) based product similarity
         * TF.IDF(term frequency(Inverse Document Frequency)), based product similarity.
         * Word2Vec(word to vector), based product similarity.
5. <b>Image-based Product similarity.</b>
6. <b>A/B Testing.</b>

In Text Based Prodcut recommendation : using word2vec and tf.idf we got some good results as a recommendations.
In Image-Based Product recommendation : we get best results using deep learning based model.

Conclusion: we can further improve our model by using[Text Features, Brand Features(ONE HOT ENCODED), 
Color feature(ONE HOT ENCODED) and Image Feature(which we have extracted  using deep learning)
and we can assign weights on each of them and try to build (Euclidean distance-based similarity)

