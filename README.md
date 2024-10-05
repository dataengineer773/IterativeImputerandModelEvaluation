We evaluate machine learning models on a dataset using k-fold cross_validation. To correctly apply iterative missing data imputation and avoid data lekage, it is reqired that models for each column arecalculated on the
training datset only, only then applied to the train and tests for each fold in th edataset, This can be achived by creating  a modeling pipeline where the first step is th eiterative imputation, then the second step is
the model, This can be achived using the Pipeline class.
