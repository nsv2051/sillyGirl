傻妞部分命令
empty ? #删除一个Bucket所有内容(已失效)
? empty ? #删除一个Bucket中包含?的所有数据

set sillyGirl adminUsername #傻妞web管理员用户名,不设置默认admin
set sillyGirl adminPassword #傻妞web管理员密码
set sillyGirl name 傻妞 #傻妞机器人名
set sillyGirl enable_http_server true #启动http服务，已失效,一定会打开
set sillyGirl port 8080 #傻妞http服务端口
set sillyGirl download_prefix https://ghproxy.com/ #傻妞更新代理
set sillyGirl duration 5 #傻妞消息撤回等待时间，单位秒
set sillyGirl update_notify false #傻妞自动升级是否通知
set sillyGirl auto_update true #是否开启傻妞自动更新
set sillyGirl enable_http_server true #是否启动http服务，对接微信公众号等需要，建议开启
set sillyGirl ignore_notify true # 傻妞忽略通知命令，默认忽略。
set sillyGirl http_addr http://xxx:port #失效ck无法禁用的，检查在青龙自动生成的傻妞地址GOTIFY_URL，特定网络环境手动

set qq spy_on ? # 返利间谍模式
set sillyGirl pushplus [token] # 管理员推送绑定pushplus指令
set sillyGirl recall 关键词1&关键词2... # 关键词撤回功能#关键词支持正则表达式。
#set sillyGirl recall [sS]*[^0-9a-zA-Z=][0-9a-zA-Z]{14}[^0-9a-zA-Z;][sS]* # 屏蔽京东口令小妙招
#set reply 打赏 [CQ:image,file=https://xxxxxxx] #傻妞内置赞赏码
#set reply ? ? # 关键词回复功能 第一个问号是支持正则的关键词，第二个问号是回复的内容。支持正则捕获分组

delete reply ? #删除用set的关键词回复

set qq masters q1&q2&q3... #qq管理员
set qq onGroups g1&g2&g3... #指定要监听的qq群
set qq ban_one2one true #qq屏蔽私聊,可收到消息,不会回复
set qq tempMessageGroupCode ? #qq临时消息默认群号
set qq auto_friend false #是否自动同意好友请求,已失效
set qq onself true #是否对监听自身消息,已失效
set qq default_bot 主机器人账号 #傻妞支持对接多个qq，主qq机器人
set qq notifier q1&q2&q3... #接受管理员通知的qq账号
set qq ignore q1&q2&q3... #忽略消息的qq账号
set qq spy_on q1&q2&q3... #spy群号

set tg token ? #telegram机器人token
set tg http_proxy ? #telegram机器人代理
set tg sock5 ? #telegram机器人ss5代理
set tg url ? #不知道干啥的
set tg masters t1&t2&t3... #telegram机器人管理员
set tg notifier t1&t2&t3... #接受通知的telegram账号

set wxmp app_id ? #微信公众平台app_id
set wxmp app_secret ? #微信公众平台app_secret
set wxmp token ? #微信公众平台token
set wxmp encoding_aes_key ? #微信公众平台encoding_aes_key
set wxmp masters w1&w2&w3 #微信公众平台管理员
set wxmp subscribe_reply ? #公众号关注事件回复
set wxmp default_reply #公众号默认回复

set wx masters ? #微信管理员
set wx notifier id&id&& #接受管理员通知消息账号
set wx onGroups onGroups g1&g2&g3... #指定要监听的群
set wx robot_wxid XXX #微信机器人id,好像是自动生成
set wx mode vlw #运行模式,一般能自动切换
set wx relay_port ? #微信回调时端口,反代用

set wx api_url ? #插件调用地址，确保傻妞可以访问可爱猫端口
set wx keaimao_dynamic_ip true #可爱猫是否动态网络地址，适用于可爱猫家庭宽带而傻妞在云服务器的情况下
set wx keaimao_port ? #可爱猫端口
set wx relay_mode true #图片转发模式，否则可能会出现此图片来自xx未经允许不得使用的提示
set wx relaier ? #指定转发地址，格式为 https://域名/relay?url=%s，不知道不用填
set wx sillyGirl_dynamic_ip true #傻妞是否动态网络地址，适用于傻妞家庭宽带而可爱猫在云服务器的情况下

set wx vlw_token XXX #对接vlw插件的token
set wx vlw_addr http://vlw插件ip:端口 #插件调用地址，对应之前插件配置的
set wx relay_mode true #图片转发模式，否则可能会出现此图片来自xx未经允许不得使用的提示。
set wx relaier ? #指定转发地址，格式为 https://域名/relay?url=%s，不知道干嘛的。

set qinglong enable_qinglong true #是否启用青龙管理
set qinglong QLS xxx #青龙配置,自动生成
set qinglong autoCronHideDuplicate false #关闭自动隐藏任务命令
set qinglong host http://xxx #青龙地址
set qinglong client_id xxx #青龙client_id
set qinglong client_secret xxx #青龙client_secret
set qinglong autoCronHideDuplicate false #关闭自动隐藏任务命令

set qinglong pins xxx #钉子
set qinglong chetou xxx #车头

set jd_cookie enable_jd_cookie true #是否启用芝士
set jd_cookie groupCode xxxxxxx #仅在指定群启用芝士
set jd_cookie http_proxy http://xxx或者sock5:// #代理
set jd_cookie asset_query_alias xxxxxxx #自定义查询口令，变相实现屏蔽查询口令。
set jd_cookie query_wait_time [限制秒数] #限制查询频率
set jd_cookie enable_auto_update true #自动检测ck有效性开关，关闭则为false。

set jd_cookie auto_migrate */7 * * * * #定时执行迁移

set jd_cookie ad ? #自定义广告，成功登录后发送
set jd_cookie pub_login_addr ? #出现无法自动验证的验证码时使用的地址

set jd_cookie adong_addr 阿东ip:端口 #阿东登录地址，已失效
set jd_cookie selfQid 机器人qq账号 #阿东qq机器人账号，仅支持阿东1.7及以下版本，已失效

set jd_cookie nolan_addr http://诺兰ip:端口 #诺兰登陆地址，需要http
set jd_cookie login_num ? #登录坑位,已失效

set jd_cookie xdd_url ? #短信登录接入xdd指令，格式http://IP地址:端口/api/login/smslogin
set jd_cookie xdd_token ? #对接xdd，额外参数

set jd_cookie enable_yad false #跳过云上阿东。已失效

set jd_cookie tip xxxx #登录服务不可用时提示
set jd_cookie login_tip xxx #发送短信前的提示
set jd_cookie login_tip_qq xxx #你可以单独某个客户端发送短信前的提示,其他客户端将qq改成别的,如wx
set jd_cookie phone_tip xxx #手机号获取成功后提示
set jd_cookie phone_tip_wx xxx #你可以单独某个客户端获取后期成功提示,其他客户端将wx改成别的,如qq
set jd_cookie sms_tip xxx #接收短信验证码提示
set jd_cookie nolan_timeout xxx #超时提示

set jd_cookie disable_notify true #关闭推送指令，不想收到请jd unbind
set jd_cookie asset_push 0 13 * * * #定时资产推送和cookie检查
set jd_cookie task_Notify 0 13 * * * #定时任务通知
set jd_cookie notify_mode group/private #任务通知群聊模式
set jd_cookie qqGroup ? #任务通知qq群聊ID
set jd_cookie wxGroup ? #任务通知微信群聊ID

set jd_cookie wsck_ua xxx #wskey转换时ua

set jdWSCK update 56 * * * * #wskey自动转cooke定时
