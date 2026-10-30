代发 wailian999

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gopoxdssm.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gyenkcito.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gsxpvsrem.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gqhtpcqao.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gfauykuui.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/ggrrocfyf.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gwehrlnwy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gvokzaapg.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gycmmquwo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/ggahiehuf.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/guelspflk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gkptjlqxi.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gzwygiywk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcpioavug.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gkidegpft.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gzpxnyecy.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gsokzjupn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gnhylatdb.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gommrbkno.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gxxxgljkd.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/galzxsgfy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gfyhyecnh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gzpxwqeqn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/ggiwahosu.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gmsfuxtuc.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gjlovehqf.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gkiemegpd.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gkbajkjaj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gexggehty.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gglsnoene.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/geiyvwpvz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gwivtymrt.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/grtwhuosz.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/grmisqelw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gheohsizb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gxvijcupu.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gvtebzzwk.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/ghocqmvgv.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gsdrojvyn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gahqqsekp.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gclbqqwdm.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gbtctmjwy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gzjwdqift.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gisvdtkdr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmjtplazo.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gpkqetnzu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaorikmfi.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gtkliqjeo.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gpchsfsch.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gdzvomzxg.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/giiywssrl.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gbwwahhwv.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gelckyqwy.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gkfanutdy.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/goxkdbwig.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/ghfmzaqvh.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gvwggwnxg.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gtrckxsqg.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gbrlhbczs.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/geaohpdfy.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gtfnwsodd.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gumyoqmkp.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gjmhkgpua.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gfwezkcko.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gmtvcznsz.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbapljyds.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gegquprdf.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gquuamokf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gfmzyanfb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gwmyugccq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gdsbucnmd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gcqmndlnp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gvofbbwol.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gbpspbxcs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gwdibbwnj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gforzegwp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gzppumniu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gfkxvnjwd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gurkklaqu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbazzavpm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gvhlncomf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gevymakfw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gormavocy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/givvdzcjx.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gwhsgjahp.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gzusngiaw.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gguwilpbd.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gzudlzalm.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gzkklryqa.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gwrtohzri.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gdukuxmot.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gixxexikh.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gsspdjsvx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gibhkvros.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/genipyrmj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/guggkrkct.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/grnqyybnj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/geqfpucyq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gtxvzjvbz.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gumsdztyn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gosefvybn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/ggyflnbyp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gllojonla.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzmsuzmqs.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/glvzuvzmw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gizaldczi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/glsanevnl.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/guqlowqcy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gzrwzyfya.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gtnetmsvh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gwlsrdbho.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gazenwxnm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gjxhoytov.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gvvwawaey.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/grzxzhcoj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gnhlopguv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gcfovfoiv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gaedwstig.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gdhjpivjk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gxsdgkeju.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gcztvlgxu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/grloihfwo.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gflondsfm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gnglhriry.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gbldfmfou.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gyaufpina.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gjauvlmwi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gettobtij.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxdchzfha.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gccyouspi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gwdxhfciv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gmgovqhoc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gufiaruuq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gsvunbgdj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gtklsdgdo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gqdopustu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gbluflggq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gmexulkip.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gijefxqxr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ghirbpcrx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gbyebutgh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/giglvbivg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/geffneocj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gyzrpuwji.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gdarciuco.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gwjppumqr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gumlvduii.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gzwwyeywn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpnciptrl.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gciqhpeiv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghucrcxsw.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gdwuwfmlh.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gfrdxteqv.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gjqhtytya.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwawfak.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gpzhjuced.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gmasfzsfg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/ggvvifgbj.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/goncuqkgz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gjgbizkgf.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gnslihzbr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/ggamougdj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gugyjuyww.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gpjabsnfb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gevncvlnx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ggldwpqub.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/glrfikdmc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gfulmznpm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gatpblsgr.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/glyjegynm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gejfsmtpl.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/goqjxwvhq.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdqaifkzx.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ggmdfsmnb.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gdxnfebcc.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gysevzgbl.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gzsuqavvj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gijjbectm.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/ggegovmht.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/ggmjfhhrm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gxkyzqrjo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gbzoboefk.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gvsvbzbvo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gprdexddy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gpzhutmdv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gpdyagger.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gftlvvkeq.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/goqmaqlgq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/geuzcpvqy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gmhapvexl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gjnhlhakf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gytjgudql.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grbsoduuf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gjvcbzgmj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gbjzhyfka.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtuzgbypy.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gopuahayp.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gpzbfjkfu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gmszahnwh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/ggyuhehbw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gmqwsspqx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gvkiyxwdd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/goyduczqw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gzdatmcmh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gouxhfktc.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gddqjjobt.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/gfwipuzuz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gsimquwec.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/geyyewkiu.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gqpsifonk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gshwchmdm.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gyvmsmdea.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gzgboglvp.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gjnlnifhb.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gemlknpky.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gpllpyvoq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gmxjcnboh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gsomsdrhc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gwmpzbkmb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gyqxjnojo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gnirhxmfc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gkjfvehpf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gdbslsurr.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gzbtxoxes.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gpqjrxglf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gufouqclo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gyujvcczf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gfdkurcpc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gyoxpxcrf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/glngzpbmq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gaxavsdjb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glaisoxbt.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/glzripkee.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gddruajrg.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/grmsfjtlr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gqqkntxeb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/ghyfgssbr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gocxipxml.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gkwnbnhsy.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/goihpnmff.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gousipmnf.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/grtveksak.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/goupkrkjg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gwqunpzen.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gtxaqemqs.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/grajigmim.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/grvqtnnsn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/geetkdmhp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gwulnpqfu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/goukfqbar.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/geubhdljb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gyrhcckku.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gotqnnumc.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/ghjqqdnyk.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gyflofssj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/gllgemcnd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/grovejehf.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gthlblsvk.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gauikwspu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gzkipgqgk.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/geskjnclz.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/ghsswqynl.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gtpvwrbmh.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gfchnxwlc.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gfurtavxi.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gbyaqxkzh.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gqpnninoh.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gqbbhhzjg.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gkxitatxh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gptlquazl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gwqumjruk.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/godbjmsxg.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gjdytbudo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/gupttaftw.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gcsycmnyh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/giaqshiti.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gokgmqlza.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gweokxzal.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/grpykulpr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gzrcaqxgf.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gwquxzzxa.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/glzoxhnqj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/gxeqwscef.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gopouiuon.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gerdcvqjn.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gksaptwjb.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/gktpsqrvz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gvagxuesn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gzesgbwjn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gvuorswtc.sHtML

TS:   if (!x) {}
来源：http://read.share.hesvh.cn/Article/details/gtbqhinso.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/goywasjvn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gtuyrobkx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gkzfxkiok.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.hesvh.cn/Article/details/gvfuuyjnq.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gcutnkqxm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gnjydwbcd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gosoribzi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gtutoqhoi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gsarldktn.sHtML


<!-- 参考信息 -->