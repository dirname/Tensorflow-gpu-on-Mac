# Tensorflow gpu on Mac
<div align="center">
  <img src="https://www.tensorflow.org/images/tf_logo_social.png">
</div>

---
__Environment__
+ Python 3.6.8
+ CUDA 10.0
+ cuDNN 7.5
---
## Installation

Download `tensorflow-1.12.2-cp36-cp36m-macosx_10_7_x86_64.whl`

Open Terminal and run :

```bash
pip install tensorflow-1.12.2-cp36-cp36m-macosx_10_7_x86_64.whl
```

## Test

Well, After installation, you can check whether GPU computing is used or not.

Run this code in Python
```bash
import tensorflow as tf
sess = tf.Session(config=tf.ConfigProto(log_device_placement=True))
```

If you see information about GPU, it means success.

## About Build

Python Version                                                                       | Status                                                                                                                                                                                        | Branch
--------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------
**3.6.8**                                                                     | ![Build Status](https://github.com/dirname/dirname.github.io/blob/master/2019/04/29/1556506356/success.png?raw=true)                                                            | r1.12
**3.6.8**                                                                     | ![Build Status](https://github.com/dirname/dirname.github.io/blob/master/2019/04/29/1556506356/success.png?raw=true)                                                            | r1.12.2
**3.6.8**                                                                     | ![Build Status](https://github.com/dirname/dirname.github.io/blob/master/2019/04/29/1556506356/failed.png?raw=true)                                                            | r1.13
**3.6.8**                                                                     | ![Build Status](https://github.com/dirname/dirname.github.io/blob/master/2019/04/29/1556506356/failed.png?raw=true)                                                            | r1.14
**3.7 +**                                                                     | ![Build Status](https://github.com/dirname/dirname.github.io/blob/master/2019/04/29/1556506356/failed.png?raw=true)                                                            | All

If you are interested in compiling, you can refer to [Mac build tensorflow + cuda](https://blog.forgiveher.cn/2019/04/29/1556506356/#more).
