# everything-recognition
Упражнение на чтение кода. Распознавание образов


Simple script for recognizing a number of preset objects from video input using OpenCV python library. Recognized objects
are highlighted with a frame.


### __Requirements__

Apart from python3 the script needs `opencv-python`version 3.4.17.61 installed on your system. Install it by running
```
pip install -r requirements.txt
```
in the terminal after cloning the code.

### __Installing and running__

run

```
git clone https://github.com/devmanorg/everything-recognition.git [path-to-copy-to]
```
command to clone the program. Go to the folder and run
```
python3 run.py
```
to run the program. Hit 'q' to stop & exit.

### Available options

The program can recognize and highlight following objects: face front, face profile and eyes (all enabled by default);
smile, full body and cat face front (all disabled by default). To change the recognized types open `config.py`
in any text editor and set `'draw': True` to enable recognizing this object type or `'draw': False` to disable it.

### Content description

`run.py` has main code. When the program is started, it loads enabled in 'config.py' (see `Available options`
part above) objects' cascades from `haarcascades` folder and starts video input from your camera until exit button is
hit. Whenever an object is recognized, it gets highlighted with a frame.
