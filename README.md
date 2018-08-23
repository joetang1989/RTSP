# RTSP
基于Vitamio做的实时监控视频画面demo

#BUG:
target api >=23时报:libffmpeg.so: text relocations
临时方案:降低target api值
正解:
mk中加入
LOCAL_LDFLAGS += -fPIC
参见：https://blog.csdn.net/ahence/article/details/68953878
