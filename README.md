- š Hi, Iām @flowerQiang
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
flowerQiang/flowerQiang is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
0.0.5 The time of creating alarm clock on IOS side is written dead

Adding an alarm clock can be modified to

// ę·»å é¹éē»åļ¼å¼å§åå¤å°ē§ļ¼č„äøŗę­£åęÆå¼å§åå¤å°ē§ć
    NSArray *arrAlert = dic[@"alert"];
    for (int i = 0;i<arrAlert.count;i++) {
        EKAlarm *elarm = [EKAlarm alarmWithRelativeOffset:-[arrAlert[i] intValue]*60];
        [event addAlarm:elarm];
    }
