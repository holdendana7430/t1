代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2pjvzlwyp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2dmzkuyvk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ooycosns.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2favtkqcg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jymgqluk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hcfxsuza.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ygcedtwe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2stzerahj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2lszcqlhf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bcoichvs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wkpykltm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wafljsgl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2twulcobi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2psoxvrwt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vyaviodh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vnbgccyt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2iohivlfi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kqhjuncl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vxcwatta.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2pibyoflk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2auqoxfud.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2aotolpiw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ppsiboig.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2etdvsude.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ldbsctcd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gbqfojqc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2synssqla.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gnlsjkox.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2oqnhmxjw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zdxjjgfm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xrehfjez.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzgaadof.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ebbfjwqy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kpvyiqrv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2raphiagg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pqvqpgir.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zlrmnqdz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kwifjrhx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2veuwvoig.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2asfzjcoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqqjesqu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ksiztiyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqembvcg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pvsbcnmn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nfezcqcs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2plqhgfqa.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ilpqcfge.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2khhkllvy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rbyqfzhu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jjahbxgq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oebxqbrf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2blnvcxla.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2truzlpze.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fxhvigyy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xkipivlm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ybspbzae.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2xwgymrke.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2uvmpwwsy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2buggohmn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dyomqxyb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vxqynzfl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zlrzwodo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qnsabqeo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dpvebdwb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dwcouzaw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2slseljxe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nmgtmxwb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fretbqwc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2gugwiqic.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hjadxgkj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wwmpjdak.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zhqjejou.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rnxnwvxw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2oytgatlg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pvsrahyq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xhtxkvlb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aehdfldc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qylxvjvp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2kbgweglu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jumamyzn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2avldueun.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2wsdselqc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ggwjpvcb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zkizbpvk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2kclcyxfs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uhrsvjoq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2tlanxafn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uszptgby.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2hoeljxmn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2brikwtxy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qruhdhsj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2tgwrdxfc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2uvpgteek.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2tntnohwi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2dzjxbdsm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2fjarwwje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqslsrrk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2dkeqncnl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jvtbbriw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yipqtvyt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2qzxkenil.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2tvtmjwfh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2shajptgv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2pzxqqwuo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2qgvfusph.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2djpsmbnf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wqrxvdqi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2oojviiaa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hwcgdddt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2byyrbysb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mnrbimvr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2jpjanxzp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2zuymwdef.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2senemqti.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tyzhyrgc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wgfubakt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2nsvtyuij.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2hjsbjfkg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2szlfmcze.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ogiigjdp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2swddsorf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2djjzhtbw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sqxjaove.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2modwdjyc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tlpcwytd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gcwgjbfc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dhtbxvcn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2fdnrhcwx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xqdjapvz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sjchzvrd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fhneylpn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rgmoztxy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ohcaozmq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pwmbnmuj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmwzkorj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iiqsxthd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2abqxfidp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2prtlagwg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fncfbcxm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2efwurbiw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nlpkdiau.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ncrmdtas.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gnxmpbyn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xpelxwai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxycjsio.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gqstbayq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmlfukvh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sqpinhyy.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jbzlmiyt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2lmqihzil.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ryvmtrxx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2izohdfye.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ayqqanip.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wsdqxzdv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2akzwvuhw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2smsdvono.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ijooqiiw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2kpzegcxr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bedxtluu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jmtluknk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sjmhmebb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kxkixeql.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qyarejpm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2xyhuocto.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rttsrlio.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2twibarbu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2izvkhwzb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yvbgsoid.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zzucwbod.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nsngylze.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lvdbwumk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fxyksccd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vejnsyrf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2stwnezsq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jnsqtcaj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cprrsxyy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbctjhsw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rbcfonyo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2clbbymxp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2exenlxww.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2zicibgsv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jfcjgzhl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2xgcnjtgc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2qnuxyika.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2sgvftzxz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zesmyofd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fqhxpprb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2utrsubgy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2itkzgwex.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bwrvhmak.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kcjiisjt.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2usonwein.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kuwztxep.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fitxwdks.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2amdkgcpx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2btipjxom.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fkstxpzc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lfjhfcdq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2quqdefzv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2xpwwbyns.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2czbvmpvp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oavpomdx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2mbtaytka.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2tkbwafqm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2eeivokln.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cdeoytbc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sgculemq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2uypkkdlu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2csjmummr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xcmmtyer.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cisibfuh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fvbocbmg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2goixswlj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2chffqusd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2nrpsctvs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2exxtoqsy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rxdhiuey.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2uxgdodki.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bgumhgkb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2srrwfble.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcyhoiw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjwrdmul.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yowmqatw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bexugkao.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vxpdabgq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hzmobcbm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2kheoesxt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkzlubdj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dmcfbkpv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2bstgefat.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qlpuhyfi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmtyrgil.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ekddfyts.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wunqsrvw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2pwdcrsfj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2toahhxos.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xrpupsff.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2rirudowr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kieqkihr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2twkvogfy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2weiipdhb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ayhwttof.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bktimtvq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2hpxihawi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zqwcymlz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2obfotaii.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2vjbgwjuc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmrrcmfu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2zehgvnfv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fpveovsx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2prrhmhhk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2anvucqpi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwdecpz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bzalmcnn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qynfbnch.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2exkctxsq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pnrqmffg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yrbxlfph.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uueqknek.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fnnaulrl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mzfjqczo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fstnmqsc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2daszqckc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eahfbhvc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sjqkjyzv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2gehtrwte.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vlxsvxic.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2csywiiqt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2guburqhk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2zfjlzhlw.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iovioqoc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2djyukjrx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2guvwsnoe.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xasxpsaf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ujeccvsv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vdvxntwg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gdgjskbz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zweaylxx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2rqyrvatt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2gscnejxc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jlpgesbd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gsydymfj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kttlqtbf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2yuiizvqr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2mmpjqcfj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2revvgbnj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsorolkg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtafjoyk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2yeyuddcq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2drxzsopo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twsaxvxu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jjjhliwx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qlttyxla.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mwbggcth.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2agzplzod.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kozungbc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rarhbehb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jcsadjvk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2meakovml.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvarewub.html


<!-- 参考信息 -->