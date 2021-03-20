# ghost-on-web
Virtual weibo bot
data_clean: 数据清洗
dataset:爬下来的原始数据
paddleTest：paddle的ernie-gen模型测试



## 目标

**粉圈生成器**

输入主题（tag） 输出微博

同时做“虚拟用户”的效果测试：用微博小号，拿着生成的微博去回复一些明星关键词下的微博（包括粉丝，黑子，路人等等，不要有人工选择性 ) ，看看别人会回复什么



## 目前任务

**数据爬取**-已有若干xz粉的微博

**数据清洗**（待测试）-需要去掉@ 提取出#tag# 去掉url 分割转发内容，最终格式应该是[tag-相应微博].

如果原始数据包含多个tag，那么可以形成多条数据，不同tag对应通一条微博

**训练**-已初步测试ernie-gen，待验证清洗后效果

虚拟用户测试-需要可用的微博小号，不要绑我们自己的手机号，以免出意外

**部署模型**

**整理发布**