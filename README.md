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

