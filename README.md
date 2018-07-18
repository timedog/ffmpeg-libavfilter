FFMPEG-LIBAVFILTER README
=========================
## vf_histogram.c
修改**FFmpeg histogram filter** : 添加了`display_mode` : `video`，该`display_mode`可以使直方图和原始图像一起输出，形如：
```
      直方图             图像
    +---------+--------------------------+
    |    Y    |                          |
    |         |                          |
    +---------+                          |
    |    U    |        video             |
    |         |                          |
    +---------+                          |
    |    V    |                          |
    |         |                          |
    +---------+--------------------------+
```
#### 注意事项
* `display_mode`选择`video`时，`level_height`、`scale_height`将由filter自动计算，手动设置无效
 
