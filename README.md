
##
|            |    v1    |    v2    |    v3    |
|------------|----------|----------|----------|
|CPU         |i7 4790k  |  <<==    |  <<==    |
|MEM         |     32G  |  <<==    |  <<==    |
|GPU         |GTX 660   |  <<==    |GTX 1070  |
|Ubuntu      |14.04.4LTS|  <<==    |  <<==    |
|VGA driver  |361.42    |  <<==    |367.35    |
|CUDA        |7.5       |  <<==    |8.0RC     |
|cuDNN       |NA        |5005      |  <<==    |
|Python      |2.7.6     |  <<==    |  <<==    |
|Theano      |0.8.2     |  <<==    |  <<==    |
|Keras       |1.0.2     |  <<==    |1.0.4     |
|scikit-learn|0.17.1    |  <<==    |  <<==    |
|scipy       |0.17.1    |  <<==    |  <<==    |
|numpy       |1.11.0    |  <<==    |  <<==    |


## benchmark_keras(s/epoch)
|file name                 |   v1   |   v2   |   v3   |
|--------------------------|--------|--------|--------|
|mnist_mlp.py              |     2s |        |      1s|
|mnist_cnn.py              |    26s |     10s|      3s|
|imdb_lstm.py              |    49s |     49s|     35s|
|imdb_cnn.py               |    15s |     10s|      3s|
|imdb_cnn_lstm.py          |    34s |     30s|     20s|
|imdb_bidirectional_lstm.py|    90s |     92s|     61s|
|cifar10_cnn.py            |    76s |     31s|     16s|

## benchmark_sklearn_v1.txt
bench_covertype.py

|Classifier  |train-time|test-time|error-rate|n-jobs|
|------------|----------|---------|----------|------|
|CART        |  6.8731s | 0.0116s |   0.0424 |     1|
|liblinear   |  4.3188s | 0.0072s |   0.2305 |     1| 
|SGD         |  0.2960s | 0.0244s |   0.2315 |     1|
|GaussianNB  |  0.3585s | 0.0419s |   0.4841 |     1|
|ExtraTrees  | 22.0710s | 0.3468s |   0.0372 |     1|
|ExtraTrees  | 12.4086s | 0.3312s |   0.0372 |     2|
|ExtraTrees  |  9.1098s | 0.2537s |   0.0372 |     4|
|ExtraTrees  |  7.8867s | 0.2251s |   0.0372 |     8|
|RandomForest| 19.9885s | 0.2347s |   0.0330 |     1|
|RandomForest| 15.5255s | 0.2145s |   0.0330 |     2|
|RandomForest|  9.4432s | 0.1105s |   0.0330 |     4|
|RandomForest|  8.2592s | 0.1364s |   0.0330 |     8|


