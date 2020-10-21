- SurfaceView:继承于view，1.0就有，使用了双缓冲机制，即允许再子线程中更新画面，所以刷新会比View快，适合2D游戏开发
- GLSurfaceView:继承SurfaceView，1.5引入，在SurfaceView的基础上封装了openGl ES的api以及render线程，openGl专用的，适合3D游戏开发。
- TextureView：继承于view，4.0引入。因为surfaceView的原理是创建了一个在应用窗口上面的新窗口，脱离了android的普通窗口，因此无法对其做变化操作（比如平移缩放旋转），TextureView就解决了这个问题。
适用于视频播放器或者相机的开发。