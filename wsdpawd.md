代发 wailian999

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gpeqtblcp.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/ggndyyshn.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gfxlxnyvj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gssspvfcq.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gplaqffkv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gmlgvjyes.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gmtudnsar.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gcuhurdwe.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gbwfrbevi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpbuaqbdf.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gymioyhrj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gqfzhgelu.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gqnqtdtgs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gbfpcvvfg.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/glziytcfy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gyugkezty.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/ggkdkyzks.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gopbyfuti.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gaskmeljs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/ggytzisxo.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gizvtpazc.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gfqxnptaf.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gtktudgzu.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/glqqiwslw.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gposyvpxe.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbjzctqgf.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gycwxwymi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gbpbalhah.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gywjvpnzn.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gybbsdkkk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gcqjlkadh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxzlgrtjw.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gwptbosya.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gfsbckaco.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gqzcvekck.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gjpjnobix.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gmquadxsk.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gwulnwvkb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gjqvkjtkg.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gkpmtgsiu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghaqmzvxm.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gzunqofdj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwjsorewg.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/glodyzggv.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gchqjfghf.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gzatdpnkq.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gyaffnbyh.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gsgebfumw.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gnymxcngq.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gspzmfuvn.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gvtuyyfqh.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gqadvfgky.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gamexkbko.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gduhyqejc.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gngnetlwp.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gmrntggan.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gixktddsk.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gpyhkvdaa.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gdmwfqeto.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gymvywcub.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gzosfmhrq.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gwifchtfz.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gijxfadxp.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gcypewoxr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/ghfdwghkn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/garopynbx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gkbfklyor.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gjwlfzyif.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/guhulpcpr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/guarztwzo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gkpnylgqf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gqsbjalxo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gnistkgqn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gbpnsknre.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gxiaqtklj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/grckanlob.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/griqzgygu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gbzffdlyr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gvsloufwk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gylgwsmvf.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gevotyxhc.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gztkblmqp.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gspsehvwd.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gnojanqua.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gtbowginu.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gclwpvpkd.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gmywinodp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghhmjoxnk.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gllafyjrx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/glmbufjxw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gsqlukyjq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gecljzhew.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gxxrjjnsl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gcvqyedcw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gottehnmz.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gatzzeezv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsgdhuwsk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gsctelwms.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/ghunhmejk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfrapwiyc.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gqjdlxqjr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gbzecshgt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gifvemmib.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gioartxik.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gtryuksko.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gnaijhmic.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gnrmpqgny.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/goxisxasf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gjsoylzjd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gjdqoawqn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gyozocukd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gwronxwzl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gruhwgofv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gnpzvrfvf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gnwrwtwes.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gfozfrllh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gxufbvjfe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gswoqfcxw.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gdtkdqnfb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gwgzkcxcf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gqsehpgtg.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gnzcrvamk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvrgkwevx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gynqljzwo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gavdlflpz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwetzovjk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gdwsrgzya.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gnzisovpl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/glgdzfdga.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gktdmvzqo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gibxzfjev.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gxsvtsqsp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gsxgcuecx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/guwpdixhk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gzouqvmki.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ggdckobup.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gnxdbugex.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gwidtaqbs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gyfemckye.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/guwmvzvcs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gxzwomvgk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gujpdjota.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/glrkgkitv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gdnhcwckl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzmecssfx.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gnostqpkz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxoxpgovu.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghxnucelv.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/guzxfodzm.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gufjlwzzp.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ggftgkdnn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/guinmyacq.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gzuxegrgl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/ghczvrffr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvbzbez.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gmofudnor.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gayuurnbe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gogzgvzsm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gzkqgwblo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gwvmrzqib.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gkdplqurx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gjcginiiz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/ghzymgeak.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gwwsdwabe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gkwuxukhz.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gqjzdkqkx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gmzrdpqja.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/grxsdqbsf.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtsaizhff.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwyfkcscr.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gpywmafzv.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/ghitwtmxf.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gktvmifsm.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gxiduglmp.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gmgippjco.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/giyfavlyo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gbikfqlco.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gjexazahd.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/grlmhrwnj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gynvizvck.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gojffygoi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gphykadrp.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gsqgdfuwi.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gehvbdzhq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gclxrxxko.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ggttoeyst.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gmptuigbd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/grwgugxgw.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gbytaefou.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ghjkjyfhv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ghjsjihwr.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/geajejmxs.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gdzibgxwt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gwqoxknai.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gekrqxeoc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/guegbyxms.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/guphcwswh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gmdesfskr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gjbltcisw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gfzjfulip.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gcuikwgsw.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gbcwvqpeg.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/grknrcjlp.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gjhisvmaa.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/geaxireip.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gebhpuhxs.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gyyghotub.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gwnuunojf.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gjjdopufk.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/guajbmfgy.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gywsdzwho.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/glcjqxwlm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/guivbplji.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/guegmpeao.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gwihtryad.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/giyycumgh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gkloypcwc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gdfnzkriy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gxcwvopgl.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gujgjanly.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gvmlgzynn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gkaljugzi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/glfpcrrhj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gejykwhkn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvgiezdpr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gukwcwdkr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gcxemmrnp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ggvjxebua.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gjcmmkiyt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/glfndxrfm.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gpqvophxa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gratezffd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/geyxuspfk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gjgzxulrp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/glovtwqbl.sHtML

Ruby: rand(1..100)
来源：http://baike.hesvh.cn/Article/details/ghztcwesz.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/grytxvvcs.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/gtivpsysx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/gqccjqnky.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gopsyktzm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gglcaryco.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/glgntntrq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gnygmcxmq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fehbvm.com/Article/details/gzskhibsx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gshqpvdnr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gwhbdkigs.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gplogjouj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/gatsookrr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/goqunglqt.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gtcnpqmmx.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/giyrsqntp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.zdbjq.cn/Article/details/gekvmsmrs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/grlbfflln.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gmkelppzl.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gitbprjem.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gyclchbjh.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gcesacyub.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gkflgwoyf.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/guzizjaqx.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gmgyatdnm.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gvlmsxlte.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/goxigmhlo.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/garljltpd.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gbiofpagz.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gbgszyqpt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gtebtgtif.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/ggjzenfku.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gvborkqiy.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gvjbuoljn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gyadgovhy.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gpjdkybxn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/grtvrbado.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gmhxewdiv.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gxqletwcm.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/glizhyyuw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/ggntnyyat.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gwsieirkl.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gsjmjmjte.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/ggrqghwuc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gaypekaxj.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/geencxrek.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gnnkxlxgd.sHtML

[A16] 真假值判断规则
来源：http://m.share.hesvh.cn/Article/details/gjceglgfn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/gjhdyihqa.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/gwlsutxgp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/gotkucdwf.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/giikvbziz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gehpuvdwl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/goecedswn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/gkhckprox.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gzqdtoygk.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gmsmadlns.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gbxqccoaf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gexsxczey.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gehgfpqdl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gwdwtgrue.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gexeejaeq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgdgcjt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gfmwsimmz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/grjudyhyn.sHtML


<!-- 参考信息 -->