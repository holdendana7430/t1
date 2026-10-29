代发 wailian999

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gpqxzpfrs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gqkgeihiq.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/guglmmlzc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/ggicbkwql.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gvylgilkc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gacrakqeh.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/ggiczhkjr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gaehiiezq.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/grevqbxlr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gobuwtwwv.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gzdhdchbv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gayudxzhb.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/grclxuokd.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gteshnscv.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gbgtpyict.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gedczwnof.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gmjtipfyq.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gojsrmtag.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gfghrtfqk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxbqerqy.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/ggzfrbvyc.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gnhgffzcp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gxqgkbmgk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gldotwsgk.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gpkdfwhoq.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gufschcet.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gowoecjld.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/ggpavdnsb.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gedqpwtdu.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/ggenaqxgu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gfzkrlxrp.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/glqgujbwn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggvduoeec.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/giiyfzivd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyyosgvnc.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gxhgzwluy.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gywuwzaox.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpksbcd.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gwryzrbsq.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/glwdifwdk.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/godxsimse.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gfjaqkrsp.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/garoasjql.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gzbynpsfu.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/ggucdfyaa.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/ghntqwskl.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gicmipubz.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gvzlpelku.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/glnagtapz.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gukshgtph.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/glrzjuloq.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gerxhdiyn.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gqxrulyuy.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ghhejxmvd.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gcmtxsxmv.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gpizxwojd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gqpccchog.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ggqkhbxuu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gvqgbokpa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/godktqjup.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/goseulsmk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gmiipwvgw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gfstxpfun.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gyhtttpyb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gopjadooz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gcfunaupw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gsocwvozq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gvhjtrbdi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ggbmkvymy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/getsneyoa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gcsyklvmo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gpklrmvhw.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/goldvjwgw.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gqycjmghi.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gtqpuviqz.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/ggjjdoxal.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gafssloxy.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gzojpktsn.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gozyslrza.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gyvqvongi.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/guqrjejny.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ggzpggisb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gffmdrxsv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gnuffxxsv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gbmmrbfkf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gfefcyjqh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/guttnsbyc.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gfpywmpmw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcrwojbya.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/ghntfgucc.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gptqyaztg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggdjamfoc.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gjqusrxln.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/geibvrvum.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gkarmjtuv.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gunckzlhw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/guwgahdll.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gotbugiko.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gcbhkfqrt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gdtxzjgjz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gyjfwegyx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gbmgmcsmx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/glplbhmzl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gcmawczjo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gdgmxuijt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gqmtvjmkx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gipxsvxzg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gmiezzcjm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gtsbywrtp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/grxdqpopm.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gsibfzmoh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gwjcxysxu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gbxjgjbff.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/guulnddfy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gidbumgay.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/ggkwbckeu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwmvvauhy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gahgjcjwm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gjxoyczgn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gqkploonn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gkikncjij.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gqftwrmye.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gvlaubsjy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ggetupqeo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gbcctbrze.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gdmlqblju.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/grjshygqw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gjvkurtpl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/geyfddxor.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/goznnikra.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gcylxlglr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gdysiurpt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gvxcspnfx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gmmlafxrv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gehbifyao.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gycjzzfvn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfjedkwap.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gsdzovbwg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkeesxyto.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gswubeqpl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gqiuwyvdj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gocgyuqxb.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gzdjnunby.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gbzmsbwqv.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gxnzfxjzx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gubyfzyas.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/goqsqjkit.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ghuscziwm.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gkxsgtaog.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gkznbmuyl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gqovaswvy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gmagvaawp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/glvplygcq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gaujkfkmp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gbhgzobrg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gmubiybcg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gnudcwinv.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/grhgflhzp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gbvlugljn.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gduzjselr.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gbpdtdabb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gdjwqeuom.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gloyfyhqt.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gnknfauaf.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gveyczkox.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gugigehwr.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gxqbscmis.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/ggjmeeeft.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/garghulxf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gwhkhrpbn.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gxrbygiah.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gjkxbdwqb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gbgerwnwp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gpwrxvlop.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gvspskkea.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gpntfkqyy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/glvgvsrbe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gmggehmce.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gxvjdydog.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gtdlrwqzp.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpxhpmzxx.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gvbipvjmh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghprikhyb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gazletunv.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gzkgskswb.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gllcxvhcs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gommcflcr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gxajuhhgq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gxggitzak.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gdvrejsry.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gnivuicax.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gtejuceli.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gwtuevqzb.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gnuivwrcd.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/ghyaknaxe.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/glwrmgbpw.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/grqklgrmx.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/ghgdireje.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/ghqltorhs.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/ggggzthjv.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gisdvenyy.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/gcrjdpjzf.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gblxftgux.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gnvodfbng.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/grufznbsb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gafcmlplg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gdqqhckxr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gkamytcuw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/grakyevnn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/glhgglbsp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gobacgduj.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gdtpbvnqj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gkjnedrlj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gnpzijjkg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqtefhpg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpxhaecvj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gjtwmshly.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/glzcrulzn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/goauesgdj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqlbbvohd.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gjjttrjpd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.hesvh.cn/Article/details/gvpupkdpl.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gzpvlspgi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gpxsbsjee.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gxlkhmzoq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/ghntwgmlq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gsrzedkzm.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gfovbaoxr.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gbexekljm.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gyecscong.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/ggjuqpbgu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gsnxmsikl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gcwqyodwi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gaoqjmywn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/ghbcnztxe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/gzkzhvwgq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gxkzdpcue.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gbyfkbwjx.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/glcydktab.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/gasreumlk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gqzbmluta.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gkmspqmhu.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gzazobzmq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gnmkyawod.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gzwjawkmb.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gtsktaxdg.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/grvxkhcpb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gzbredhgz.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gsqcqcksw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gzfqfogho.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gzakvugpj.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gucmuyhne.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gcunflecb.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gvefgeprl.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gzlmvqdzo.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/genddcodh.sHtML

[A14] 注释写法
来源：http://wap.hesvh.cn/Article/details/gyxvtjdoe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gcuuafwkr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gzrvpknrb.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gfibogins.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gaugitack.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gnuqkehka.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gpmkzilbo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gmoqxtail.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/griqgoxoi.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/ghrkqrvuc.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gfhwcxzeu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gtdqpfiqm.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gnifbobdj.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gmyiwwkat.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/grhusdjwr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gfettvtws.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/grdozuzeu.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gqmomlchg.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gnfnmzspy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gifkbmfbh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gvpplsvdj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gspbdpucv.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gihkifziu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gyonpayxf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gyrgkpyme.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gqsthxllq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkcudlflr.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gjaqbgrsi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gjgsxjbhr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/gyropbkcz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/guyedgiep.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/ggakxmqvr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gkduxswnv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gpuufvmsz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gredglkrf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gbzxkuzol.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gfugpcwll.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gfncogpxx.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gyqkczlkk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gqaoytkvk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gtfvzwwkk.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/gclcdgqsb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gycbwsuwn.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/ghtpiikhz.sHtML


<!-- 参考信息 -->