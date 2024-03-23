# AFK / Tracking Detection

Sends Trigger signals to <b>TrackingLost</b> and <b>TrackingFound</b> whenever face tracking is lost or found. Should work with webcam or ARKit tracking. Triggers after roughly 3 seconds.

You can use Trigger nodes in other graphs (exampled below) where you need to use these signals!

<b>TrackDetectTimer</b> - Timer between each check for blendshape values. Lowering this will make the detection trigger faster (though make it more noisy).
<b>Sensitivity</b> - Minimum variance for Tracking Lost to be triggered
<b>TrackingLostTimeout</b> - Time in ms after tracking is lost until tracking can be detected again.
