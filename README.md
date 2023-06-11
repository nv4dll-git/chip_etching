# chip_etching

## 程序用途
微流控湿法刻蚀的工艺中，流道的宽度等于设计宽度+2*刻蚀深度，因此存在设计稿与实物具有差别的问题，为实验设计带来较多不变。
chip_etching软件包用为基于图像处理的微流控芯片刻蚀模拟程序，用于模拟湿法刻蚀过程，辅助微流控芯片设计。

## 原理
首先获取芯片的轮廓，然后每一个轮廓上的像素以刻蚀深度为半径向外扩展，模拟刻蚀过程。

## 流程
- 首先将微流控芯片的CAD设计稿导出为无压缩的PNG格式，分辨率越高越好，大约需要3000*2000。
- 采用Photoshop或其他软件将设计稿二值化，并储存为无压缩的tif格式。
- 使用etching_simulation.ipynb进行刻蚀模拟。

## 案例
- 二值化处理后的微流控芯片：
![微流控芯片设计稿（二值化处理后）](https://github.com/nv4dll-git/chip_etching/blob/main/data/model.tif)
- 刻蚀模拟结果：
![微流控芯片设计稿（二值化处理后）](https://github.com/nv4dll-git/chip_etching/blob/main/data/output.png)
- 微流控芯片的实物照片：
![微流控芯片设计稿（二值化处理后）](https://github.com/nv4dll-git/chip_etching/blob/main/data/real.png)
可以看出，刻蚀模拟结果与实物十分接近。

## 软件环境需求
- Python
- scipy
- matplotlib

## Author/作者
Haowei Jia, China University of Petroleum, nv4dll@outlook.com.
贾昊卫，中国石油大学（北京），nv4dll@outlook.com。
## License 
MIT
