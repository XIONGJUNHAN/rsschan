# RSS Chan

> RSS update&notification(Bark、DingTalk、FeiShu、go-cqhttp、gotify、iGot、server chan、push+、qmsg chan、WeChat work、telegram). - RSS更新与通知(Bark、钉钉群机器人、飞书群机器人、go-cqhttp、gotify、iGot、server chan、push+、qmsg chan、WeChat work、telegram)。

# 功能
RSS酱 运行在github action上的rss自动更新通知项目
- 支持多rss订阅源
- 支持多种推送通知
- 支持Github Action
- 过滤重复消息
- ~~精准定时(云函数实现)待实现~~

# 目录文件
- main.py        主程序
- notify.py      通知库
- oldrss         rss记录
- rss_sub        rss订阅

# 使用方法
1. Fork本项目
2. 项目添加必须变量 Settings -> Secrets -> Actions -> New repository secret
    - USERNAME           Github用户名
    - USEREMAIL          Github邮箱
    - 其他push token变量名请看notify.py下的push_config名字
3. 添加订阅至 rss_sub
4. 在action里启动或者 右上角 Star 启动并查看log