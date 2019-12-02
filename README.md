Facerecognition-Hisense-cup

Hisense cup the first Jilin College Students artificial intelligence innovation competition

times:2019/11/22

完整源代码
实现一边截取人脸一边删除人脸
上诉功能改进，修复部分bug

时间：2019年11月20日

功能实现：实现全人脸识别画框，从图片中找出所有的人脸然后画上方框
剩下功能：存储处理好的照片
完成附加项


人脸新想法

libfacedetection for python dlls只能做到任意角度的人脸识别，但是不能做到68个点个人脸计算
尝试用libfacedetection与face_recognition进行结合
做到快速计算的同时，也能对比出人脸


优点：图像录入的速度很满意，能达到目的

缺点：图像的计算速度很慢，6个人需要7/8秒

待完善点：1.图像处理完毕以后应该结束全部过程  2.人脸对比，从采集到的图像中找到目标人  3.描述人物

新想法：用于仕琪老师python接口，裁剪出人脸，然后交给face_recognition进行计算（2019/11/20）



时间：2019/11/22
完成目标人脸比对
优点：不能有效比对，效率较低。大概率的情况下会认错人

问题思考：
1.摄像头分辨率过低，因为目标人如果用高清的图像会大概率识别出（此时阈值需要手动更改） 

2.计算时间非常长，大概需要20s左右（六张脸），因为做了大量的重复计算
