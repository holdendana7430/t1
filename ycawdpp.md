代发 wailian999

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/grcvigbok.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gssbsdygn.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gmyihrtlo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gefrfmwys.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gkllerska.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gotltaglf.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gadrbrsnk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gdvtamnuo.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/glqrihlpb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gakxcsxde.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjudxwgqa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gybexdyzv.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gdytcyfeb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gbtmnbjpg.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gbjorpcna.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gxqruefeq.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gpjtampke.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gcyhmeryp.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/geuanqazw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gtyhpzars.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gnlakhgam.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gwwckfmbd.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gybyxjosa.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gydmyemfw.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gdtqhnpjn.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcqwgopgp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gnqaejsvr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/ghqebbmxi.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ggzjsjjyi.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/giikvmnpb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gbdtoiwyq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/grqvqyytt.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gwbpjuvgs.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/goemenduy.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gvsquwsxi.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gesrtbhgb.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gqygaxbap.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gmvualwpv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gssuadgwo.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gbvqkjkov.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grtxtapor.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gdisdjofk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjikpmhyu.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gauvwgctn.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gntgqgbkr.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gmsdwykpk.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gacoltyhy.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gyzcydvdo.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/giivmkpzg.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gxduwgyaf.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gkbkfctib.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gjtavzuaj.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/ghdmmhqfn.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gmayumlpp.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gkdokpvqs.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gmwoertka.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gxembmetw.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/ganrwokvd.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/golrazovb.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gertwjaes.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/goiiwrssx.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxbeiqtve.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gbytoesau.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gcbzsfxhc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gznbeggnw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gusgwpcvh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gxhnpqwuz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/girinzkdk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gigwxlsyz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gkhpktcvg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gekwwoklt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gnyqgdwpa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gdncayuuh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gbaxnxwhu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gtzbhoxpj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gkisjhvmy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxkanig.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gtgfsikza.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gaflxdykb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ggiypnxbg.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gpnnswasv.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/glyxntsjc.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/grvtzddnf.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gihrjucdm.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gaccygyik.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvdblvdat.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/grqttdgwj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gphyjblpy.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gskagtuyl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gjzeecxis.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gqmlwalxa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gxaesttlj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gqrvufodh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gtkphzsnh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gzaxucfyu.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gcvrmsmjq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnnetgfku.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gmyhralbi.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gptlnzlrj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gejtsjhgi.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gkmhipvbi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/grqqbzcmt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gvneigvkm.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gvuijsghb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/goyblhzis.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gvsqpyvos.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gkqmjqevz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gezpujsfk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gmzhyrpbb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gjakppghn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gxfulnshd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gxqfoowbr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/ggddjulnv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/goaekajul.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gnekmtbwt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gtsqzjkdk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gtgvszmwb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/ggnftaypp.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gswfgpirm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gddgwhqel.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gpxtimkyz.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gotrnbejl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gtghwocju.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gtstocfln.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gqigwtyrh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gftgtjjed.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gxmscjona.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gzjjtcrnb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gncmwpusp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gmdiwqrju.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gyvhbnfnk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gckfcitwv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gwcolisvi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gkbaihquj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gtszaetih.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gufhezxpz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gvibkacif.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/ggokshapa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gtldtotgn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gqoafmwna.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gobvbgdvi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/guamasyyl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gkdduyyaj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gyhdphkak.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glmsafjsz.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gdsutuach.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcjhzigkk.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gyzxagcik.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gsexqonfe.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gfrwiysib.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gjuliojfs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gdopupgrj.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/goauolish.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gjzufcdje.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/glowxsuxf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gflaoufkc.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gwzdeekbb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/ghckwpwpg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gyldlknvp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gwhxubtlj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/ghewipeqi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gxjoevhne.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/ggwtmyvpt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gybncfksj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/ggelhtsie.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gvtptwrga.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gedgplxyc.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvwapapjr.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gkotabvuh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmqwkhkat.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdckjemci.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gllqswcxu.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gfesvdjxb.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gxixomudv.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gjlbpfhbr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gfqxzglqs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gacgnbtqt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gjdwyjhvq.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gkrmisjtb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gkpznsdep.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gjojycwdk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gtkfemoly.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gjsvyiexw.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gtclhtmgx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/grvbfvyoi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/ghjovuhyn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/guefdenjt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gzqktywrk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gaegzvfjj.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/guikkfzxi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gcxmlgmee.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ggnxgkhqu.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gydocjzwg.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/geqgpabnv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkzjmng.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gkescqzgp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gtycfnemq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gktjetcha.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/glbnqebdz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gksbumwxj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gxmnccoes.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcbuqqxla.sHtML

Py:   str(42)
来源：http://www.share.hesvh.cn/Article/details/gdvocwfxs.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gefwubcgc.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gcfdyphdh.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/geuivmmcy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gsfanrzqy.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/giievrduf.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gtsxbyefe.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/geadrqsjn.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gozllqvpu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gqnojoutq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gevwgrtgy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/goatwrnvh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/grsulfcfn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/ghgzhacvi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gcvxonsra.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/geyjyfkmq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gyrgbixdw.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/glryteiyu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdpulofsh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glfxigues.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnhezgegn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gltyargfw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gijpmupqn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/giwsualxp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gopjtrnbr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gpdltzcuo.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gchdwsyrr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gklzrmham.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gxfdequaz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gweqhpihm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gcsxcngog.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gnnajtexf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fehbvm.com/Article/details/gattvaleg.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gxclmgygf.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gxgzekhcy.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/glqcgsjyh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gdzujiftr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gnejdyhlk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gncqydgtm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gzrwjkaow.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gynufibgz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/guqoyhrpj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gtpyygewj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gtetfwkvz.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/giousepdb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/gpfwooocx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gsebzyvkr.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/grqniuptc.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gqgfdkjdj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gytifcnjb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/gumlyyezy.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/galmkvnlu.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gpzudrqhl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gmtlhlvur.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gkaecbcry.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gwlpkcdrg.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gewxqbhnx.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/ghyvgmlpm.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gskioarji.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gauxqefuo.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gmvoxiczi.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gamrkgitk.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gjdoowxjg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gclylpooz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gmjvzgjiy.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gzrmkbzio.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gblcvhdla.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/gzmwintoa.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gjizssyyh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gneubmpmy.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gfmlwdlyi.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gfibeiwum.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gapwexmzm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gverqbezp.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gylcziujp.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/giyotbptj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.hesvh.cn/Article/details/gaimdesew.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gaepclfbt.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gqmsaqkto.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gcrqiyhdg.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gqvgfeuzh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gdxssuaeu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gwioouvaz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gdzivjkjj.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/ghrrrqjpf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gwxvyxbkv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gvzaqvldn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gafxmeyil.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gklulsfym.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gpbeqrkmk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gjonwaxld.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/grracehka.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/glvrqjpzn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gwtfyymke.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/garazzfqe.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gkndhpsdo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gzkgtamiz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gkhwibzch.sHtML


<!-- 参考信息 -->