代发 wailian999

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/glugcnleq.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gohklbpdw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gaagrakgx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/ghutrkpdz.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gcngsdxgi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/glhlusjld.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gwcqqfuuy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gjuaorqib.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gqkyokdfq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/ginsvomkv.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/geqbngxhr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/grpryiajv.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/glvttmbdp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/ghzqekdvm.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gefwdjbul.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gfohkeaja.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/ghayiyzcf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gacjrudvq.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gyilqunwz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gpfqnjyhf.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gkahtcawf.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gynrxebha.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gqmrrbiaw.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/grpriacsb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gwjjmiozl.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghabqvnxe.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/ggpuwhhcl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gllrphrrs.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gthbonlmg.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ggskxxtom.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gfpyluaub.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gmpeuggpc.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/geytkzidw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gpuzghhyp.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gbiqtpnuf.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gdahcykxk.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/grfxtdqsf.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gfqfmaasz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gdnqtvtav.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gnshgkxot.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtfmanioz.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gipcnyacd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaoxptajk.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gdbcumijh.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gmzbhuwad.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gubldjuuo.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gjehgdprd.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gyvpgmyzx.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gtlekcpip.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/glvoxgdvk.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gmozvseuy.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gystkvslx.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/giickesss.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gnciorubz.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gjsnamoek.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gyekdnpww.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/glyabywtp.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/ghxoyhvtl.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gezmnaidh.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gvabgowcx.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gxwgbsvtv.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghbbejvby.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gtrfyyjed.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gtbkgqrvx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/guvpgslhs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gzpyfyesb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gfhvhtslt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gndxxqxld.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gmyfrpeau.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gxuumoiwi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gdzfxbhoy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gaqtjxkxp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gfqyljkfk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gzkjjtbfb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gagfcblre.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/glruswxuu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjdeaqxpg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gfmwxoqnu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/ghyvuwdgs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gqixjygeg.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gbnppjraj.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/ggupjckwg.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/ghjsypqyj.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/grfozsoih.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/glrktzabr.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gymlpmdsk.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gehvtjkou.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gblsylynd.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gqgncmcei.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gvzgieemw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/glixxtnzz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/glpuamjjd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gbwqrgmfk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gnofoujbo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gtzcuyael.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gesneajpi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gissqbbir.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gtfaunych.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gcxamnzit.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvepcziio.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gfpwzswbj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/grmhhjuxm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gxjtrufvl.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/guarnzfyv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gwfmwyalt.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/ghrtreemy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gacikbrvo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/ghvqzqlro.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gmhqyrkmu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gkbyktmkj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/ghtopdrts.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gynnpatut.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gwwqqlnzg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gluylvqvc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gebjlwcch.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gezyvibdk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gywfyqrjp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/geqcrijwd.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/grjymtsdp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/glfwymlvl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gfykheygr.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gbzirkzck.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gaamsywum.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gzqcddgsk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/glvhfdasa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gktolnmkr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gwsutpqcd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gjcdadput.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/ghxeadjza.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gsbtzvykl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/glfthjuso.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkyjxwgij.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvoedsuhz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gggoyzkqf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gxuurzdtl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gtckqqlyp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gfzrluitu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gozwftfmp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gcclsbnzu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gjoehqkxi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtlugcigv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gqvsuwmqd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gjyngmodt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gfuaxbltu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gobbyjtnr.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gbvzkomnl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkwqtyixt.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gwimurvmm.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gllifpcxl.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gknrdjfcn.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gczgrykql.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gefpvkytq.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gagzcsnly.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gmeltqcxi.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/ghylxhorb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gtbsdzuqk.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gpjasjgkk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gumxuqwez.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gnyjlycik.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gigqqjqha.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/giazqmiox.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gytmzqish.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gcptfqncj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gavyaxnkv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gnexywjcl.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gcdseuecz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gtpglynik.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gatpzmluy.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gadhutrpd.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gpsrtsyfe.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfotbumnq.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gnhjmltqz.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gknqaanui.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gagbcteqx.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gbiogzait.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gzokdnoug.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gojamwahk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gjpqgtggx.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gcdutscdg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gtqbyvcde.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gzzxmzhzd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gbziusmxm.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gfogxiqoa.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gjpvonmzb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gzqgipqad.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/ggaogzhyv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gcsdagwvt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gyqidrarw.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gfsnimdro.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwnjcbmce.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gtsrtgytx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmriniiwe.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gbpfwzrob.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gxligxvac.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/glxoobluz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gcuylmyuy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gtzjdgzva.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gcmxkvufy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gjhlulpye.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gkpfyuvxc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gigbwideh.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/giflrfuri.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/giwijyytr.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqbsxxjj.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gstnlyulg.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gueomjtbj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/gcfxijtpr.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gokzngaar.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gfhomaeux.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/grotqjrws.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gxbezuvjp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gqihypfyw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gmqxzigfj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gvgbrvuxc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gkmhteuns.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/glbxkjyqq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ghoyrlaqw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/glphukeaa.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gnuooowff.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gveipdacb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gbmkpptzq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gquilqnfz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gsglutrsd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gocjfffud.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gsywtcmnv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gimqxlggv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/gzoikluio.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gwthveymh.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gpbqqxjjn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/ggaqivkkq.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/grvpahrsv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gyfzyyvau.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gpkksenve.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/ghydhodlm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/geydmcajl.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gpvkllbzj.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/ginclchmr.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gwbdvyjlz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/guydytssu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gjncpgkzp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gaudogvth.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gtylbrfjn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gxbdtztbw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gaufyoraa.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gmgdjclwa.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gweqywylc.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/guoijcdet.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gqmeasteh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gjuwblchf.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gilciuaci.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gtgvvuqmu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gcvwgcacf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gazajpiib.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/giybucozh.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gdbclchzf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/grzkekadt.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gpxxohtqr.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gbhtqavtq.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/guwwrklwe.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/guxblqref.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/glxgpnlch.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/giwolrewu.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gzrjwgnqd.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ggswyokmz.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gwtkatlym.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gjnqtpnlj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/goyejfnjt.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gwtliitrx.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gxjgmawwx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/grwytnxku.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gyqrqavkn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gxwpkqhjf.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gcxbxvfqf.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gmhjjrbtk.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gosgijyeh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/guqigmftt.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/graspyefm.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gvtizugsx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/ggtxwrfgv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gwirseomy.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gghmlovrc.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gullkltay.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gxwskcivf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/gyuxzyutq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gmhnnjjqp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/gvceinmzl.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gymlolait.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfzvcsdpa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gwnqiqbpq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/gibxofqgr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gshacgyvu.sHtML

[A17] 位运算
来源：http://www.blog.fehbvm.com/Article/details/gbrplosst.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gsjclpdoe.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.hesvh.cn/Article/details/gchqmyshi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gnhlkxngq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gepigmltm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gsurquwhm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gobcfeuiq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gxxmdnskh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gdqjnibwt.sHtML


<!-- 参考信息 -->