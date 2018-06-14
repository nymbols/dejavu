# Installation of Hym

So far Hym has only been tested on Mac OS X.

* [`pyaudio`](http://people.csail.mit.edu/hubert/pyaudio/) for grabbing audio from microphone
* [`ffmpeg`](https://github.com/FFmpeg/FFmpeg) for converting audio files to .wav format
* [`pydub`](http://pydub.com/), a Python `ffmpeg` wrapper
* [`numpy`](http://www.numpy.org/) for taking the FFT of audio signals
* [`scipy`](http://www.scipy.org/), used in peak finding algorithms
* [`matplotlib`](http://matplotlib.org/), used for spectrograms and plotting
* [`mysql-connector-python`](https://dev.mysql.com/doc/connector-python/en/) for interfacing with MySQL databases

For installing `ffmpeg` on Mac OS X, I highly recommend [this post](http://jungels.net/articles/ffmpeg-howto.html).
## Max OS X

### Dependency installation for Mac OS X

Tested on OS X Mavericks. An option is to install [Homebrew](http://brew.sh) and do the following:

```
brew install portaudio
brew install ffmpeg

sudo easy_install pyaudio
sudo easy_install pydub
sudo easy_install numpy
sudo easy_install scipy
sudo easy_install matplotlib
sudo easy_install pip

sudo pip install mysql-connector-python
```

However installing `portaudio` and/or `ffmpeg` from source is also doable. 
