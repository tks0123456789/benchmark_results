
v2: v1 + cuDnn 5005
## benchmark_keras(s/epoch)
|file name                 |   v1   |   v2   |
|--------------------------|--------|--------|
|mnist_mlp.py              |     2s |        |
|mnist_cnn.py              |    26s |     10s|
|imdb_lstm.py              |    49s |     49s|
|imdb_cnn.py               |    15s |     10s|
|imdb_cnn_lstm.py          |    34s |     30s|
|imdb_bidirectional_lstm.py|    90s |     92s|
|cifar10_cnn.py            |    76s |     31s|

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

## Environment[v1]
* CPU: i7 4790k
* MEM: 32G
* GPU: GTX660
* OS : Ubuntu 14.04.4 LTS
* CUDA: 7.5
* Python 2.7.6
* Theano==0.8.2
* Keras==1.0.2
* scikit-learn==0.17.1
* scipy==0.17.1
* numpy==1.11.0