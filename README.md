# chip_etching

## 程序用途
微流控湿法刻蚀的工艺中，流道的宽度等于设计宽度+2*刻蚀深度，因此存在设计稿与实物具有差别的问题，为实验设计带来较多不变。
chip_etching软件包用为基于图像处理的微流控芯片刻蚀模拟程序，用于模拟湿法刻蚀过程。

## 原理
首先获取芯片的轮廓，然后每一个轮廓上的像素以刻蚀深度为半径向外扩展，模拟刻蚀过程。

## 流程
- 首先将微流控芯片的CAD设计稿导出为无压缩的PNG格式。
- 采用Photoshop或其他软件将设计稿二值化。
- 使用etching_simulation.ipynb进行刻蚀模拟。

## 案例

![微流控芯片设计稿（二值化处理后）](https://github.com/nv4dll-git/chip_etching/blob/main/data/model.tif)

## Requirement
- Python
- scipy
- matplotlib

## Author
Haowei Jia, China University of Petroleum, nv4dll@outlook.com.
## TODO
- Fully translation of files.
## License 
MIT
