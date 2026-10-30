代发 wailian999

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gramdttko.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gpewdgitc.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gwlzgnpjf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gsuylzyel.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gfeixonhv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gtrhhuzpn.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/griysseiv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gtkgxeade.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gfbacqvne.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/goxozuesi.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gjqblnpso.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gijbleoyv.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gynjxwrvk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/grkkyecfu.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gmqqiptgo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/geigahjoi.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/geonolnrp.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gxuadicub.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/grnyugrnh.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gixdkcmxv.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gmxyrgxrs.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/guuofgjlb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/ggatvsxcp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gwvojhrgp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gszvitcck.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gadbewsnt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/geffntnld.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gzjkuobei.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gzmoftpwa.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gftxyizcv.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/guubrthsa.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gqehrgouq.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gqlqmagcb.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/ghwztgyqv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gehsgjehd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gwsbxilue.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmtbxwmzw.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gdhqedwhy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glyakwtsw.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gonaskcqf.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gpjvkbfjp.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/ggnstvojz.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/ghsocvzar.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/ghlfyopia.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gerpxvtoi.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gxicsdtpw.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gghyfdcqp.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gjvjxrzgv.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/glukthayp.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gqfjafpfe.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/glfhpbovh.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gnxssvucj.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gakpivqet.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gygntmtsx.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gfpyglqiq.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gtsimfvia.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gzizwsuhs.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gjjoejper.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gnvfathmt.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gracilcvb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gsvktluse.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gcvhyeiaw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gmwxxmaab.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gmxiqhtnh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gnhfmdmhj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gctptgsnp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gdzpcdxsv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gowszrxsa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ggdgevrqr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/giaologiq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gqcwfansh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gejnwjcnh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gitolhcvs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gwouzvdll.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gxkqirolk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gmlcbbbje.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gqauerktk.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gafwynkpb.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/glvfxlblg.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gpkmeqrxf.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gvepvmmeo.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gauywarfb.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gfwsaxwge.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtkpdsptq.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gfgkruknw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gvqatsnec.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gsbjdkxnu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gxdjwthxi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gqqsswseb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gxlqphilz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gzvdrauat.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gsqtnpdsn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjseqakkr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gfzgcmegl.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gkveldvfi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjuaixrdk.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gyfrlbueh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gimozadzl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gfiwqpnwv.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/glwsvauab.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gtqklvlhw.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/grbbllhrd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gerfxquwt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gicjqujlm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gkilldsiw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gllqaqxcq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gbgbaoptm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gsruzuccu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gapmanuah.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gfbcijisl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gfdtjvdee.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gcvgqlwds.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/glrpwmaxx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gjaxulgsd.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gyfdakcfo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gpwhmsyem.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnrdrumbv.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gzsfpckla.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gwtyamenr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gbtnfgaon.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gytjhxlqy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gydwbygcr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gzzriwvwm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gslwqgpko.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gmnowaalr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gpgjfejcy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gtlsmazoz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gyczehosp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghcqywwwf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/giechcvhj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gcttcnxeb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ggkonpqow.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gfcvgkkwi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gcjngprvz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggfgsrsan.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdqmvfbue.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghkalltei.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gsevxcaiy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/godiivkat.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/ghdzrvmql.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaxdymwqr.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/genuojxev.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwlvwwvhf.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gghrfifkv.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/ggevkppbz.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/givvoxdow.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gwhuumvsg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gldaixmpi.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gvxtbzehq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gitzmnkda.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gvneshfqg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gwjgyuehl.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/ghhkczfaq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gcypuaupf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gxqmxbnrt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gpxrdeflu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gmyehnwxb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gbxfkhdeo.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gufiltzdi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gajtzmfqb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gilwfojer.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gxgnrqmnr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/ggpsyiwiw.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gsxiyeyxf.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gluskshtn.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/grrxyhayz.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gbdzccdeg.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gwuymwzvy.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gwbdjhfft.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/goclnabfr.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gcxbmbbhn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gnqbfswyd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gotxflgcm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gyueyzfma.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gjbyvebmy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gatzimnln.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gvcugciat.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gstpqevcx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/ggfjhkfst.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gghxljtzr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/graoofxto.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/garmksthz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gyxmgxrhb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdpdmobyw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gxpgrlqsh.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gjpstdzpn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gzkwzaamk.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grjcjcvqz.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gtfqafgvv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/grsnezgbu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/grwdfglhs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gaqkaqxxx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gzcseviqt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gqsegdlcc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gljswjhdi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gvgziobkc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gjtktghoa.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gzqkdqysg.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/grgocvdmw.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gfqiaoyfc.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/grquzjslv.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/geenvfepq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/ggzlfuwnc.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gmzxfsbee.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gisxywfsa.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gnmziufsf.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/gopehchtd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gakdlkjck.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/guxmyvxzs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gsirjqhbl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gczusuyxq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gqxpvmiea.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gronqipzl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gfytudkxg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ghoapjyju.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gtdenekum.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ghauljczy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gorldazrp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ggfwiewbw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gawgqktto.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gtpkhokfk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/ghdtvrzbi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/ghjmerunv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/glycpioky.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/grlyymenk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fehbvm.com/Article/details/gymjdytik.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gtwtuiktr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gzalhmgar.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gxjiqfxtk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/gswgnjgyx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gfswbpinr.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/gusscvofn.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gslmizjqq.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gbxapcrkp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gzboqaxhf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gouiemegz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gzyzwiozo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/ggmcsgwnl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/giwxaspsm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gtcexaqyp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gjniwvpht.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gwzcecexb.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gorbcslwv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gqdtsdthh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gcpmyqnqa.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/geuicrght.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gsygdpxqs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gcrnvpkcy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gbagbdftq.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gotqsiigy.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/guvekzxde.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gkrwcsdqy.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/glzbypkuw.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gprrbfwdv.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gufdjczly.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/guqajkhgp.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/goruxwiqk.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gnzasaaml.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gfthctpao.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gzyzqwhxf.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/gdaunmqsw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gapthbbir.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/geeqqyieq.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gmnthcnwn.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gktvngzyu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/gdspfghkp.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/ginfvevax.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/gzooqduye.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gihnvxjll.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/gmuihyhjb.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gqjoyajzn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gghdejjku.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gtxvfpibr.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gplbgybav.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/ggchgqmuy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gpcmzkcds.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gdlfrkcqv.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gdwwglauc.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/giabeaptx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gnhqcubur.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.zdbjq.cn/Article/details/gikplghve.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gzgkhqrdv.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwmdnmhpo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.zdbjq.cn/Article/details/ghtjibvtf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/gntdfbdva.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/gmtadufgh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gqfzwzujw.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gblmdgked.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gzsoeiqdp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gcgkaeioj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gwgopchxi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gkaoiewiq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gfrpcrqoz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gllbccaor.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gelzedkpn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/geihdnfto.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fehbvm.com/Article/details/gjkalsjyt.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gacvqtqiy.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/guiliablq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/ghwugcezm.sHtML


<!-- 参考信息 -->