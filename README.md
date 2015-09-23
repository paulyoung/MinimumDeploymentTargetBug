# Minimum Deployment Target Bug

Run `script/build` to see intermittent build failures of the nature `error: module file's minimum deployment target is ios9.0 v9.0` for `ImgFlo` despite its minimum deployment target being set to 8.0

This is assuming that a failure due to [rdar://20490378](http://www.openradar.me/20490378) is not encountered instead. If so, retry until the expected failure occurs.

The issue can been seen in [this Travis build failure](https://travis-ci.org/paulyoung/MinimumDeploymentTargetBug/builds/81733277#L444).
