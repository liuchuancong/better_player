# better_player

A new Flutter project.

## Add playback

```
<service
            android:name=".PlaybackService"
            android:foregroundServiceType="mediaPlayback"
            android:exported="true">
            <intent-filter>
                <action android:name="androidx.media3.session.MediaSessionService"/>
            </intent-filter>
        </service>
```


If you call setData again,the nolification and playback will be disappear,you should and the code. i don't konw why
```
 @override
  void didChangeAppLifecycleState(AppLifecycleState state) {
    super.didChangeAppLifecycleState(state);
    if (state == AppLifecycleState.paused) {
      mobileController?.startPlay();
    }
  }
```

SurfaceView will be blackscreen, when enter fullscreen or toggle screen.would you please help me ?