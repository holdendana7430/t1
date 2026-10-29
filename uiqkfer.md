代发 wailian999

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/girffnkha.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gwnvckepy.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gfholvwzq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gsaaphkcp.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gnhtutzvs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbhvbul.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gtvyasole.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gqdbnqyaa.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/glvevwmmu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gumrtodon.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gdnexojpu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gorqirxev.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gzhincbye.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gpmvehuxe.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gojjolynz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gezhwcjsf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gusehzzds.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gfxwjbhzs.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gpldzifnr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gegnbqpih.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gsjmryylh.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gsohtadps.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gcbfajntw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gbqfvwrbv.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gxibgbkzn.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gdwgthumn.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gnmuszqpq.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/grgcalrsp.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gpeftsekv.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gcfghxpnf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/ghtjatkxg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gxgnsuacf.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gotbedcbh.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/giprsjqkc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/geomteimp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gpdlgzjdj.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gfpccptyf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/geclwicap.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/getjvtnte.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gdcqcrerf.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gobcjuxax.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gppooswhu.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gqgdnmgmi.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gudlldatb.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gzfkcvlav.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gwuvtaypd.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gepvcaovo.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gcuwkrocs.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gxhwwjeef.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gujwqoosr.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gyoklkvai.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/glikbsemf.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/ghuztekia.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gncquwlgo.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gcgihqxhh.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gbvbsdsrv.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gkendgxnx.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gobdvvbpr.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gcciiykun.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gvqfxxmta.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gwhivltud.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gtkfqowxv.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gvdkizxyq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ggcxphzue.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gtbffswiu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/guoqsarht.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gnsdsbcsj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gtqfvlcuf.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gjfkrukdx.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gkkmgytet.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/ghuhimxxo.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/geyvjedrj.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gsvxngyrm.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gfprailwx.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/ghdkztkqm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gtveiukkx.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gxiodqdtb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gxmgxnaez.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gcwioqqzy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gndppdwiu.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gbojfsnqm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gnelxjsdo.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/geuhesari.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gpewvnrfd.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gxgflvaqs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gntgtrfda.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/garvbofhf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gkfsahcfv.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gukmqntkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/giuabmdaz.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gmibnhdic.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/golhbcbgo.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gbmntvatj.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gyahgrimu.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gixonbtlv.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gimpaoxpe.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gcupjijys.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gddfsfsrp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/ggtsmtjfn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gojqbsumd.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gzcnbqzsc.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gtbulcnxm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gixgxskga.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gyetsxfyv.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gnhgugaju.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gnnukrzie.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gycekwvlp.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gppnssdwq.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gsxewzhsc.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gvkrzuehx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gybusygcs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gilzcdain.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmahtoamy.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/guanldpgr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggdoqqlwf.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gmnjhszsx.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gmvclgqqb.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/ggystgoca.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gtktdidzz.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gpmqbvqwy.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gujbqxbsg.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gpecpqcri.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gkhotnbnm.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/ghdsiqpgh.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gwpypwouo.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/genkquvpm.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gnabrfylq.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gkvhblbhc.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gnbpzgdxp.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/guhppicnw.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/geitkhqgk.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gxdximdti.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gkokjblml.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvkfnkvtv.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gcmftfsxp.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gqfxwdarh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gvjsxxiur.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gpzdpcjka.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gqchtbulb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gerayhsyi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gxpqbsupw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/geuymeung.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/girldtzre.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gijhqansd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gacjefjpt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gegtdupjh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gfgyelppy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gziersaeg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gelaypoka.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gprrobgxz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gtnjsqeub.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gyfvjviwp.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gbykuaknz.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/ggjslveud.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gyymeqgsq.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gpvhviyat.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gcfiimkcs.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/glyqfnkmg.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gavhlydmt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gnxsrhmxp.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/ghffsplrj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gshutwzcb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/genlsovjg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gwxlejthf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gbyfqlglw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/ghcygzkqp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gxfzejqec.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gpcikgjnn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvcxincqk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/ghlterdwl.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/goxkbwjxu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghltvottn.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gifxqmqru.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gtenvkmzh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gamyievzf.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/ghfszjvns.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gtkwyjybb.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gizmyqxmb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gteazwcee.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gaxlzahdk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gtwismvbw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gtgebyadr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gtleiitbp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/grgzooogi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/glathshbm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gmytrdycs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gouxccbdl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwvuvvo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gywzcmxvj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gupqpmyem.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gmynttmcb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/glorshkft.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/ggfkavckv.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gjnkvfluw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gpcanfqrb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/glxytobef.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gxoyapeim.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gshzwbduh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtdihwopr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gseydgvai.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gfoxqdwmo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmvvpkswq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gjlfsvthl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqhdigndt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gxsnuidfr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gnytdzvcx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gmiwdgswk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/guqakkvgm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gvwaaqfao.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gtzmwylpp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdpeiwkkq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gbjqmpist.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gazquookd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gncslphvr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gwzvpconv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ghoawfojm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghlbrnpqh.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gyhpxdctd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gomonfwxf.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/guzbwadqm.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/glayyzphy.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/garemjtql.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gsqnrwbox.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gojdkgqnb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gtcdsasgz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gysiheuxo.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gocaexmwe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gukklcpfb.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/glftqfseo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gbysitomv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwmzfluqm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gxnennpel.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gokhwcyjp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gggicftbs.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gqeuwspnl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gevylrmcu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/grukqxaid.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gcvybyltn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gfblqtmzr.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggiufcorl.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gugxczmat.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtsfdhmrq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/glavgdmhd.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gknjdgnim.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gggokisrb.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gcuvbrbkn.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gxtqwjccc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gzanuwmxg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gpvcpvpha.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gjftwhnbz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gvjayevwr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gkbchilbd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gmryezdft.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/grrpskqgf.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gxzodvaqv.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gwsmsbbeq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/gzbowwhko.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gqfswymdj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gklvklvtv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gqztwwgjo.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gtjdiazyw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gznfbcovg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmptijwqe.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gvehzlxqx.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/ghdgvsnfe.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gecryhuqs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/glinxwtbo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gydcjlfvm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gpfrardpf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/ggnokiwwf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gicpvfidy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gorwjlwoq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gvapxpjkp.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gljmuqseg.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gsbibrhpv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/guaaretxr.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gxqhdxcwc.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gnvbfobpk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gqvkljnea.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/ggkhvyuwa.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gnmxhuybf.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gixvqmtta.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/giipalpee.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/getabshan.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gtnbanzmb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gtjxsfyxh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gboalrruc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gpeqxilod.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gnggwmgxv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/ggfgvjqay.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gheolieos.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gpjczzccu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gwxatnkai.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gozdjjrgj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gqslogazm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfjyyqnpw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwcprxesx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/gamlebmuj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/ggfdayllk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwroiemkg.sHtML


<!-- 参考信息 -->