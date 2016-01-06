# stmn

Question Answering system from stmn.

## Requirements:
* Python 2.7
* Theano 0.7 (with floatX set to float64)
* recent [NumPy](http://www.numpy.org/) and [SciPy](http://www.scipy.org/)
* [scikit-learn](http://scikit-learn.org/stable/index.html)
* [gensim](https://radimrehurek.com/gensim/) 
* [Keras](https://github.com/fchollet/keras) 
* [NLTK 3](http://www.nltk.org/)

#
download data to corresponding directories in stmn folder:
```
cd (top_directory_of_folder)
mkdir data
cd data

curl -O http://www.cs.toronto.edu/~rkiros/models/dictionary.txt
curl -O http://www.cs.toronto.edu/~rkiros/models/utable.npy
curl -O http://www.cs.toronto.edu/~rkiros/models/btable.npy
curl -O http://www.cs.toronto.edu/~rkiros/models/uni_skip.npz
curl -O http://www.cs.toronto.edu/~rkiros/models/uni_skip.npz.pkl
curl -O http://www.cs.toronto.edu/~rkiros/models/bi_skip.npz
curl -O http://www.cs.toronto.edu/~rkiros/models/bi_skip.npz.pkl
```

```
cd (top_directory_of_folder)
mkdir en (or use existing /en directory)
cd en 

curl -O http://www.thespermwhale.com/jaseweston/babi/tasks_1-20_v1-2.tar.gz
tar -xvzf http://www.thespermwhale.com/jaseweston/babi/tasks_1-20_v1-2.tar.gz
```

##To Run:
```
python wmemnn.py ba/qa5_three-arg-relations_train.txt
```
if minimal computing resources are available:
```
python wmemnn.py en/qa5_short_train.txt
```

## Acknowledgements
based on Pararth Shah's [qa-memnn](https://github.com/pararthshah/qa-memnn) implementation and Ryan Kiros' [skip-thoughts](https://github.com/ryankiros/skip-thoughts) implementation.


## License

MIT