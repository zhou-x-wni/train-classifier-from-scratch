# 路线划分问题

参考：
	端点检测(End-Point Detection,EPD)（常用于语音预处理）

参考链接
http://ibillxia.github.io/blog/2013/05/22/audio-signal-processing-time-domain-Voice-Activity-Detection/


## 端点检测

**4 端点检测（End-Point Detection，EPD）的目标是要决定信号的语音开始和结束的位置，所以又可以称为Speech Detection或Voice Activity Detection（VAD）。 端点检测在语音预处理中扮演着一个非常重要的角色。常见的端点检测方法大致可以分为如下两类:**
* 时域（Time Domain）的方法：计算量比较小，因此比较容易移植到计算能力较差的嵌入式平台
* acc:  accepted condition
* good: good condition
* vgood: very good condition

**Features:**
* buying: vhigh, high, med, low.
* maint: vhigh, high, med, low.
* doors: 2, 3, 4, 5more.
* persons: 2, 4, more.
* lug_boot: small, med, big.
* safety: low, med, high.

## Training
**Files:**
* [data_processing.py](/data_processing.py) : download data and process to an accepted format
* [model.py](/model.py) : training model and view result

![Training result](/result.png)


## Dependencies
* Python
* tensorflow
* pandas
* numpy
* matplotlib

You can view more tutorials on [this page](https://morvanzhou.github.io/) or know more about me on [here](https://morvanzhou.github.io/about/).