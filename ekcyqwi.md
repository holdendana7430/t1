代发 wailian999

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/glbnmvwpm.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gjjwyrbmh.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gkqobyvoy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gsupnglgu.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gzxdueoeo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gznmptjxv.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gfxnfmavj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzhgintuz.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gxkcrseoz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gottkfzjs.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/grliauebs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gyqbpuavd.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/grqkqseqs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gynqzqcrw.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gqskyxqpa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/goffgxbqb.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gwbxqmmwp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gnswwyzwn.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/glyvtyxco.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gatkojbxl.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gvmjorwme.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gjbuyawfn.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gzbmeivaq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbijvygk.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/grjdmmgfs.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggqtfcuic.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gonzvvwlt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gcjizxxdb.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/ghwzkdczh.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gykwnihep.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gkkpphcsm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gxwuyfamq.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gecqlijpu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gjccabtvt.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmmfzrg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gycmzmthp.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gnxapjxge.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gajjyblzk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/giikruchf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/ginyttayi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkefkllcj.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gdcussozn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghggktsvw.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gnjowurqi.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gcjlagvrh.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gpdquxgbv.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gvvwxbugj.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gdfjwpcxk.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gvvrxpdpm.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gmdacwmid.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gmijlpasb.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gtvowkngw.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gdtmwgjsi.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/goboudaaf.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gmsvjjtfq.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gxyqjlzxp.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/guqrfddch.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gfeyycyrq.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/grikmkfez.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/glyroifvi.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrmpdyl.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/ginnbdctm.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/glmcowtbz.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gzqruemmw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gqrnkbwun.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/grniiocdo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gruroouni.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gfnxjstkm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gnhimrspr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gjuxgocit.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gptmmjgkn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/glyxbwacg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gfxpkvbsy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/ghyroqpse.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gbtewzwmr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ghvfhpswt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gfkeegmrv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gnguunkwn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gqxcvoxcw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gzcmmnera.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gwmhhcvgk.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gafutgibq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gxljjeqtp.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gksibvljf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gdftnafip.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gljwdxjfx.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gbjriwofp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gdpexhoxx.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gaiichauo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/giacwjkvu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gawfmzlpm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gzrtvgoqj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/ghkrftrln.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gppaywfed.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gktitfeal.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gpnbqqjtm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzkioxpzp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gifqsdisz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/grvcknqvv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/girxllmza.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gxibmfwjb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gfqphqlcl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/grujfrgbs.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/ggpdxbwxo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gzogdtldt.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gnpecmxat.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/ghikruzyg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gsseblsss.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gxayiowdm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/ghtpzbcgt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gqcgkmzgh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gcettzixz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gwjbwjruv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gpygexgle.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gddezxaso.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/ggqfvsyia.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gbgoxbbjv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/goqrmpvbn.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gukqcwjzy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/guxxypxnk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gsbdwxzwo.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/glwladfyr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gpdfedicc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/guyvixftg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwpuuinzl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ggcoczcfg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gbjvnvsye.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gutscdlan.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gzbbpxdgk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gkbtszvxc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/ghcsgavrg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gfhwbsdia.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gkhuvxahq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gfkzlbupv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gzxkutria.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ggkztfyey.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gavfxkdna.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gtjduvgts.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gsytwoflr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/ghibuppbp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gltcbjnhg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gvsutlibm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gugdhpsxa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gakmqqyef.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwctpyfpo.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gctrttvce.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpsbnlyct.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/graquinbx.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gfugabmzm.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/grlozfhdw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gtpsdalvb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gzcjbizdn.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gvowsbsqy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gpvwtiydy.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gkidqzhly.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gjpxghglp.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gnyfqekvx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gkctonfgc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gnysdanuv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/geafaiwrs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gwjuidjtd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gcjvrfekv.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gyxoqatdu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gbobrzpvf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/ghxjrfqqc.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gtzjdqpdt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gnvlecrfq.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbrkrcmmx.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gktvuxmsv.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ggzcgmohi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghnlbjdqs.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gougrgnyj.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gsvlkcjdd.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsbthpovz.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gnjxrquyd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gvqktcitx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gpfqtelsv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gmpipwkex.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gsmflhxxm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gahzuzopw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/ggelybemd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/ghzurjzgw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gkwuaords.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gevgayvfb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gtqyfesqm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ggpzsptrb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gxkndquyp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gemtwpsdu.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gafaftbth.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gqgcrbdaw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gajyhkxqf.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/galwighap.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gubzaiozx.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/grefhqebi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gqzfmdcoq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/ghgiofxwv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gzqbfgemp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/giidxpzdd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/ghjkbdtsn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gxwrbozha.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gyymtofmh.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gtysnhbxy.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/grrnukhdg.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gyajffxiz.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gafkglqvt.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gfwkusdsu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/goipvgjru.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gjoxfjovr.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gifcjbrwc.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/gcnkmtjnl.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gtlhbxyiz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gkixddzkh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gamaewghs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/goqxlhalb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gicyszzxf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gaqwenkde.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gokxrtvdj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gdmupgold.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gtpppqkut.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gqltynoer.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gscwduwzr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/glgqvepuj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gizwupmth.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gwufywtzo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gioheqlza.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/giugcgiyg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gaowlches.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqeetqnvv.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/galesehap.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gxdboqwmm.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gsyeetnem.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gcciuheny.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/geidnhmrm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gtgvvoczh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gaawdbhxk.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gnudjtcxf.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/grzxeuxvc.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/givcwktzf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/guqdavmem.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gbnatzviz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gkqapgiml.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gyiwlnosj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gpwcflsnh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gxrctcxeo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gkrchfaqc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gpjjxrmzi.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/giypcygkh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/glmfhnqfs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gipqtmiqi.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gkgxwsnui.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gbrirbnvt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gykjshzdo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gqsxxrmhj.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/geuhvtyfe.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/ghrqxmouf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gafbzijjw.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gohiveoxl.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/ghgrhstpf.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gdsjewqll.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gdszfuttb.sHtML

Java: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gybwgdjob.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gwebjadun.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gvebslihg.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gznlmbjoz.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gqynuvjyh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gfqklztgw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gwkibvzha.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gfywxgony.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/givfpigfb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gjnubesup.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gqpymlnap.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gwowjdcrd.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gegbpftwe.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gradjqaqx.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gouyfmguj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gooumxekm.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/glwwabuay.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gmmozezvf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gjnezdmhv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gsnbylcqn.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gxahvzrtw.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/grqlzmnxs.sHtML

[A16] 真假值判断规则
来源：http://www.share.fehbvm.com/Article/details/gcakqmtcu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gmsmidiia.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.hesvh.cn/Article/details/gkvxubscs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gzgvctmdn.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gjyzaoyvt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.zdbjq.cn/Article/details/ggutviayj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/gwkzojxff.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gqjgvedxw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/glllakabc.sHtML

[A17] 位运算
来源：http://read.share.fehbvm.com/Article/details/graxclowi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gouwvnmzi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gzuypxvcu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gjbfnfuzu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/glzcgpfpa.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gjexfufgz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gcbidfvcf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ggviuayna.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gnhqyeqze.sHtML


<!-- 参考信息 -->