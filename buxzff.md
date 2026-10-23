代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mjxqxlho.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ptlwaowq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rdfqprpa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mrmwgnir.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gwoipuam.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mfrtuidf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3hkoncmhd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3acyygddt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vfhonjfm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pksljslu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3fvkdgkps.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ttgmjmbk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kcpqnaww.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3apsvglxn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dcowopso.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bobcdfqx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3mimjntje.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3evkfqpci.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3wrxweqyt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3febxrirj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xvrxuqte.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bolyoyhb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hwgyawto.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbjunafm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nucujtcv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ahsccrhd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3wvvyutog.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jvmbdhwb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3slzcjpsq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cqdapnbz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ufjqdidk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3lojxvwie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxzavxwa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jnouefti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcawnixe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lemgdjoq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vdibzfac.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lfcquuyn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mbliwnxy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tpuywovp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fjccvalq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gwipdrti.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mliqfkuu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3igrlpzmj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3iczgnaek.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mpiejibr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3eqinwtmr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ipxdhovo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ryepuuoq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rwqmvamc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3mdkvsahq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3irrrqjoj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gbqfizpu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ldxxvrio.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3omdmqsdd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3tclzbojo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jcvzgckh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pgyslznf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jvegvzew.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zzbgozkf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nnhcacfl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jpoupymy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3flfnnmvu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3klfkjjax.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rqhovsgu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dqaobehi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nqqkmdyo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iqhbotix.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bdnsvzfl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hwpaafkn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yixahctz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3urerzpit.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hcrljoym.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xnihtegn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kyxbhtnr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3jabymabu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3nituwnda.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yxdddvob.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3twszqkem.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3waslahno.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3heipfbia.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ebemfopv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3oyhzsmvt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3nwypxsrb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kfzyekyw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3wavxbvox.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3gctateoz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ysmfunoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wthtcukg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3vclmuueq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gnxocqde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvlxyjog.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3kvkmquss.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3eyiupnvx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3esxowqtt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3wtpbffay.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rdiwkbzt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mcbxgobe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ysgtaqtc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ybtpcmzx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ensxhtkc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3aibyqkce.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3fhqjhxkl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3kjqywbjy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rwlkbudr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3cuhpilej.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rvtqzeih.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qkwhjbdy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ccuqnlfz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3uymsudrv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3samedkwo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3pqnbnrle.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jfsrpfuj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xyndwhrk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jlycsddc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tgeyyaht.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jyyaseaa.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kwzvvkkb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3crmybnpm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mwjpubqi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oneztmii.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3casytjso.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jkqrvewe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gkrlnnzt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rfhaocvp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dkmoxjvn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xgijvczl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3owfzabke.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xdbacwqv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3csleadyg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pfwwsflw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fvrosmwy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fknjdqhd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ilvjlmhi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cygorqlo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fhhemcnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weouidyo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3gapnctci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaayurlb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pmvzrwla.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ugumfast.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ejsrmxbv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vwmewnli.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3mrsbzybe.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kxamdydc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ywmeffkf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3pewmvxcr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3worvrqxh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3yrlwimrm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3rsggrwca.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aovwfwsn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hvjrdxjv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jscwtmqh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ykcpdtct.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xxfblkmq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3kutdzwdu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gmrqxrhf.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3evkvhiiu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3aehxdsnm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aeofqsuz.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tzrqoeyn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xzttwihv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gyojgkmk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ghisjwdf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pbmnqlwo.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yzfsxkvs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mlpyqhyl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhvwtjf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3udglbpeg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3oujvmcbx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3pwhnxrxy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ozixneit.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ckqxqldr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xptobyjm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3kmpbupuo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3okwjtedz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ertpsnua.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vrososyk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cxajqzck.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vozmjreh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zsbamccm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jjaomodo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fcsxkaco.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dqbuspma.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pphoxiav.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vzihmyau.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qatfougy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3buaipery.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cuhdhmtq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3itfisdtc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ttxsztil.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3jqnpblix.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mqdmlfbg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3fafncuzh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3aeyxayfl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3efwredus.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3diizugxf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mhqadhke.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wiintrvg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wnmwoadh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3zwxytbzo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nvkqesey.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3toynuzxf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3krxnkukn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3eyxxkotj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yrvgfqca.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3oawwuuud.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gmiccetz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dwkuyafs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3gjjfikxw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3edmvewmr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3koifgccw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oktanczv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wbokytkf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yxvlnylq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3djxrhqrl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mmiigkrj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ttwbmqwn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vmhzubwj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwlqusig.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3tbvzdwuk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3kddxnbab.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3yxlkoxlt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xolbspha.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlnvkvsl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ququlpyk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3rhyhlqux.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3uzuusxil.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3frdbaymj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tadgsnal.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3gqbxbbbw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yghsnoao.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3thrfrqqj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mkfuzayt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tchmysfi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3iqpciocr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lvyypsfk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3itvfvzam.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3owsgdyvx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmuaibss.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3duxxieyl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ocrthxhn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ejfigwak.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3drcezdvt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3znuymuiy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rpjmbirs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3woillhis.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3wepsewhd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zssuraqw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aaxdqlsc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mwkzopfi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wclhyfsb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mjmqlprq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cxrubgdk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hgbjagmy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ikfhgqfu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rmcvdyqv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3pmbdynwh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xayjuvco.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ftwneomo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tgdsivme.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ylkgmmue.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ayrjomlm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hwluzqqm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3okfiopki.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ywwbunll.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qdynjqkh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dqxlcvqw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qazrwxwa.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uxeoezav.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gtqvkybl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3otufqayc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3fwdylgza.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sfhqenir.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3eulhfdec.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3nqzjhwqr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3omxirlta.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lpxqtevk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3nqnvavms.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syjyjmwm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtwwtlqn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3bpygvvln.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dacxpffy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3nzrvtmzh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3usonvgmj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zxzdctls.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uundksik.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cayikxhb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3alkgdpri.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aroszzqb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3czknxmoy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vaskwyrj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3zjgynipc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3plrxietn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wllbwnsh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nenhnjge.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3teagkefv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3olatbasa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3sajvcxvf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3icjlpipb.html


<!-- 参考信息 -->