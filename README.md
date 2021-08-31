- 👋 Hi, I’m @flowerQiang
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
flowerQiang/flowerQiang is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
0.0.5 The time of creating alarm clock on IOS side is written dead

Adding an alarm clock can be modified to

// 添加闹钟结合（开始前多少秒）若为正则是开始后多少秒。
    NSArray *arrAlert = dic[@"alert"];
    for (int i = 0;i<arrAlert.count;i++) {
        EKAlarm *elarm = [EKAlarm alarmWithRelativeOffset:-[arrAlert[i] intValue]*60];
        [event addAlarm:elarm];
    }
