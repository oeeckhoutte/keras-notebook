# conda keras tensorflow jupyter notebook

## Get Started

Build the Docker image

```sh
docker build -t oeeckhoutte/keras-notebook
```

With port forwarding:

```sh
docker run -d -p 8888:8888 oeeckhoutte/keras-notebook
```

With [Tensorflow]: (See [this][Keras Backend] for more information)

```sh
docker run -d -p 8888:8888 -e KERAS_BACKEND=tensorflow oeeckhoutte/keras-notebook
```

For persistent storage:

```sh
docker run -d -p 8888:8888 -v /notebook:/notebook oeeckhoutte/keras-notebook
```

Just browse localhost:8888 and have fun...

[Keras]: http://keras.io/
[Jupyter]: https://jupyter.org/
[TensorFlow]: https://www.tensorflow.org/
[Keras Backend]: http://keras.io/backend/
