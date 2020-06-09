方忆灵
31岁   |	男   |	硕士   |	1年编程工作经验  
135xxxxxx54

# 个人优势
1. 双一流大学、英语六级、普通话二乙、中共党员，责任心强，具有1年的编程工作经验和2年的英语工作经验；
2. 语言基础：掌握Python、Javascript、SQL、C等编程语言，掌握或熟悉75个Python标准库，理解面向对象编程，理解函数式编程，掌握生成器、闭包、装饰器、协程、鸭子类型、抽象基类等高级语法
3. 网络基础：掌握socket并发编程、selectors多路复用、asyncio异步编程，掌握redis缓存，掌握ZeroMQ消息队列，了解multiprocessing.managers分布式计算，了解IP、TCP、UDP、SSL、HTTP协议
4. 测试：掌握unittest、doctest等测试框架，掌握requests、selenium等测试工具，了解Django的测试驱动开发
5. 数据库：掌握MySQL和SQLite数据库，掌握Django ORM和SQLalchemy等ORM框架，成功优化过公司的MySQL慢查询代码
6. GUI编程：掌握Tkinter等GUI库，掌握cx_Freeze、PyInstaller等打包工具
7. Web开发：掌握Django和Flask等web框架，熟悉HTML、CSS、JavaScript等前端语言，开发过微信小程序
8. 部署：在Heroku云平台上成功部署过Django项目和Flask项目，了解Gunicorn、uWSGI、Nginx等服务器软件
9. 其他：熟悉Git常用命令，了解Linux shell，掌握正则表达式，掌握Excel的数据透视表

# 工作经历

  杭州学慧苑教育科技有限公司  
  网络程序员  2019.05-2020.03  
内容：
1. 工作内容：英语课本数据的采集、校对、转换，数据库结构设计（协助），python后端的慢查询代码优化（协助），编写微信小程序，编写excel函数和word宏，培训外包的英文编辑。
2. 上份工作的最大挑战：设计英语中考口语考试系统的excel结构及数据库结构。该excel表需要容纳一系列动态信息：比如区分口语试题中的发声文本和不发声文本，发声后的等待时间，播放题目要求还是短文，何时开启录音引擎等。为了实现“随机组卷”功能，每道题还需要进行模块化设计。
3. 上份工作的最大成就：优化了同事的django项目中的数据库慢查询代码，在不更改字段类型和数据的前提下，学生的3种学习数据统计图（单词学习量、单词掌握量、周/月/季度学习时间）的性能分别提升至原来的3倍、7倍、7倍，从而解决了统计图页面的502错误。  

  联合签证申请中心-杭州  
  签证柜员  2016.04—2017.11  
内容：
1. 工作内容：先后负责希腊、丹麦、芬兰、克罗地亚、立陶宛等5国的签证申请柜台受理；
2. 上份工作的最大挑战：17年3月希腊签证团队突然离职，我在1个月之内快速掌握了25页英文pdf+数份中文doc+4种英文软件，完成交接，并因此升职；
3. 上份工作的最大成就：带领签证中心的希腊团队，5~7月间以6.7%的员工占比消化掉中心12.2%的申请量，团队成员人均消化掉756份签证申请。


# 项目经历

## Flask-社交博客
独立开发	2019.01—2019.04  
描述：根据《Flask Web开发：基于Python的Web应用开发实战》第二版教材的指导，使用VS 2017构建python环境，创建了一个类似twitter的社交博客app，成功部署到heroku平台上。  
该app实现了以下功能：
- 邮件系统，用户注册帐户、更改密码时会收到app系统发送的认证邮件，需要点击邮件中的链接才能完成相应操作，且发送邮件使用了多线程，以防用户界面卡顿；
- 权限系统，注册用户分为普通用户、协管员、管理员3档，普通用户可以发帖、评论帖子、关注别人，协管员可以屏蔽或解除屏蔽任意评论，管理员具有所有权限；
- 限制访问，只允许登陆用户发帖，只允许登录用户修改自己的帖子，但是管理员可以修改任意用户的帖子；
- 头像系统，每位注册用户都能自动获得gravatar服务器分配的唯一头像，随机头像的样式仅与用户的注册邮箱有关；
- 统一的导航栏，上设有主页、个人主页、登陆、登出、更改密码等功能，协管员和管理员还享有评论管理功能；
- 个人主页，点击用户头像，可以进入该用户的个人主页，包含个人简介和自己的发帖记录，管理员有权编辑任何用户的个人简介；
- 社交系统，每位用户都可以关注或取消关注任意用户；
- 评论系统，用户可以对任意一个帖子进行评论，当评论数量过多时，app系统会自动进行分页；
- 帖子和评论均支持Markdown语法，且能够实时预览；
- 使用selenium进行单元测试。

项目成就：
1. 构建flask app的邮件系统时，由于国内无法使用gmail，因此我先后尝试了126和QQ邮件服务器，顺带学习并掌握了python的smtplib库；
2. 通过实现用户的关注系统，我对数据库中的“多对多关系”有了进一步的了解；
3. 在部署到heroku后，发现自己对代码的修改无法应用到heroku上，事后系统学习Git后，才发现当时的git仓库处于detached HEAD状态，于是通过创建新分支、提交、推送等操作，解决问题；
4. 访问部署的app失败，报错信息跟PostgreSQL，通过查询StackOverflow，得知自己使用的requirements.txt已过时，通过更新该文件，解决问题。

项目链接：https://github.com/nick-fang/flasky_twitter

## Django-学习笔记
独立开发	2018.05—2018.06  
描述：根据《Python编程：入门到实践》教材的指导，使用VS 2017构建python环境，创建了一个学习笔记app，成功部署到heroku平台上。  
该app实现了以下功能：
- 帐户系统，每位用户都可以创建自己的帐户，并在该帐户下新建自己的学习主题和条目；
- 限制访问，只允许登陆用户访问自己的学习笔记；
- 条目关联主题，每个条目必定属于某一个主题，类似于OneNote中的“页和分区”；
- 可修改，允许用户修改已经创建的主题和条目；
- 统一的导航栏，上设有主页、注册、登陆、登出等功能；
- 导航栏上的功能布局，能够随用户的登陆状态而作相应改变；
- 导航栏在窄屏幕的终端设备上会自动折叠，比如手机；
- 自定义的404和500错误页面，发生错误访问时，页面仍旧能够显示导航栏。

项目成就：
1. 教材中的部分模块和方法已过时（比如url函数、views.login函数），因此我自学django官方文档，并重现了书本上的功能；
2. 教材上的heroku部署方法已过时，因此我自学heroku网站给出的文档，成功将app部署上去；
3. 没有使用教材指定的IDE搭建python环境，而是使用了VS 2017，因此我熟悉了visual studio的那一套流程。

项目链接：https://github.com/nick-fang/django_learning_log

# 教育经历

  南京林业大学
  林木遗传育种 | 硕士	2010—2013
  

# 掌握技能汇总表

| 掌握的语法和技术 | 掌握的python标准库 | 掌握的第三方库 |
| - | - | - |
| 协程 | string | django及其插件 |
| 异步上下文管理器 | re | flask及其插件 |
| socket编程 | unicodedata | jinja2 |
| select I/O多路复用 | struct | werkzeug |
| asyncio事件循环编程 | datetime | bottle |
| concurrent.futures并发编程 | calendar | SQLAlchemy |
| multiprocessing.Manage分布式计算 | collection | gunicorn |
| GIL锁 | collection.abc | psycopg2 |
| 信号量 | heapq | httpbin |
| 生产者-消费者模式 | bisect | requests |
| 在线程池中运行事件循环 | array | selenium |
| tkinter GUI编程 | copy | beautifulsoup4 |
| cx_freeze打包可执行程序 | pprint | lxml |
| WSGI API | enum | aiohttp |
| 可hash对象 | numbers | aiofiles |
| 深/浅复制 | math | gevent |
| 强/弱引用 | random | memcache |
| 垃圾回收机制 | itertools | redis |
| 驻留 | functools | ZeroMQ |
| try-except-else-finally结构 | operator | yaml |
| raise from | os.path | pyperclip |
| 闭包函数 | glob | matplotlib |
| 参数化的装饰器 | shutil | pytest |
| 高阶数据结构（namedtuple、deque等） | pickle | ipython |
| 鸭子类型 | shelve | pylint |
| 抽象基类 | dbm | pep8 |
| 迭代器协议 | sqlite3 | mypy |
| 生成器协议 | csv | jupyter |
| 序列协议 | configparser | cx_freeze |
| 上下文管理器协议 | hashlib | PyInstaller |
| 类型注解 | os |  |
| 多重继承 | time |  |
| property/特性 | argparse |  |
| 高阶函数 | logging |  |
| 推导式 | getpass |  |
| 可调用对象 | threading |  |
| 递归函数 | multiprocessing |  |
| lambda函数 | multiprocessing.Manager |
| itertools和functools下的函数式编程 | concurrent.futures |  |
| 命名空间包 | subprocess |  |
| 相对导入 | queue |  |
| pip包管理 | asyncio |  |
| argparse编写脚本 | socket |  |
| 正则表达式 | ssl |  |
| struct处理二进制数据 | select |  |
| 单元测试 | selectors |  |
| selenium测试 | signal |  |
| 日志记录 | email |  |
| pep8代码风格 | json |  |
| requests爬虫 | base64 |  |
| Django web开发 | wsgiref |  |
| Flask web开发 | urllib.parse |  |
| Heroku网站部署 | urllib.request |  |
| 批处理脚本编写 | smtplib |  |
| Git管理代码 | uuid |  |
| MySQL | socketserver |  |
| 非关系型数据库 | http.server |  |
| redis缓存 | turtle |  |
| ZeroMQ消息队列 | doctest |  |
| html/css | unittest |  |
| JavaScript | timeit |  |
| 微信小程序 | venv |  |
| C语言 | sys |  |
| http协议 | contextlib |  |
| Linux shell | inspect |  |
| Excel函数 | decimal |  |
| Excel数据透视表 | fractions |  |
| Word正则表达式查找替换 | pip |  |
| Word录制宏 | difflib |  |
|  | filecmp |  |
|  | webbrowser |  |
|  | fileinput |  |
|  | tkinter |  |
|  | tkinter.ttk |  |
|  | weakref |  |
