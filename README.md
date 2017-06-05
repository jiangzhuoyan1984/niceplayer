# niceplayer
NicePlayer: 学习NiceVideoPlayer后自己实现的demo，采用MediaPlayer+TextureView实现，项目实现了全屏播放和小窗口播放等功能。

1. MediaPlayer的操作封装在IMediaPlayer接口中;
2. MediaController的操作封装在AbstractMediaController中;
3. MediaPlayerManager采用单例来管理一个界面上可能出现的多个MediaPlayer，比如ListView, RecyclerView等;
4. niceplayercore module中提供了AbstractMediaController的默认实现--DefaultMediaController，用户可以选择使用它也可以自定义Controller继承AbstractMediaController即可;
5. NiceMediaPlayer是关键类，它封装了MediaPlayer。其中的Container包含TextureView和MediaController。