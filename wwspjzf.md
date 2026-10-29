代发 wailian999

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gztsluake.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gmkraqljm.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/guibpaiej.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gbickqhut.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gvzblrawp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gbourcxoq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gynjpockl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/grpiqtkrp.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gjryacuni.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gipttqhcw.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/grqbyitfj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gaxsqruop.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gjtrolqfm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gfyrhcfyl.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gdgdzbvxx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/golukxbzj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/ghujecrnr.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gvvkyvqyo.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gshqeuoib.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gshgszevm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/golbxmyaw.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/grrwhybqr.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gtwhcaxin.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gsxefzkid.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gflhnbjqv.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gaoenunyr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gkhgtuzev.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/grqftyuue.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gfkccausv.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gskfgsfzg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gscyezyuk.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gopouvxxe.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gfhbnmuwx.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gzptgwdoo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gonlvnghv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gnavcnzrg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjmnfojyp.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gcfzhhizd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmdnynyih.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/ggktbbloq.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gcpdgmxaj.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gzzcbxruh.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gparrgoke.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gnflecvnu.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gbkkkfngz.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gkaqlbcrk.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gqvwrgqim.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gsryubsxk.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gczknwsyd.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gbmpkajtv.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gxgucdorc.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gledhpftq.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/ghzwponbr.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/ghpcqkurz.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gpcyeyshx.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gfqfoxmxt.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gcjjwyiog.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gjdegjqdw.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gktmowcfq.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gxkdwxflq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gqvgdgtrj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gppjkazvc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ggorrbqkx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gfipyxexa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gxwcbnius.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/grjaglbmu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gwktcpqan.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gxkspdniy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gwjbtfenr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gzcdmqvtz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gicsznjmh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvqpxnudx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gxklqeqei.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gznzmwdxt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/ghuxwdjim.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gloapgujr.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/ghizvcvfv.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gmnyhiiol.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gwwlhjcsg.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gcqbbjwez.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gtwhpjymc.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gqjycwsnr.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gkqswzrux.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gtltpllau.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gttrepavd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gggbdtcjf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gqmeucecn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/glvdcfeus.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gxryfvfbj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/ghgrygaql.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gwibkccwy.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gugrgvwgc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfttslypf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gulnqsvfw.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gdypufhep.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggmfaolqq.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/ghbequlyp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/godycaats.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gyonftiuc.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gsbtgrhan.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/ggwacnabw.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gxsnfhvco.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gvohoidqj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gveppeper.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gxqjzfnii.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gdjwhokye.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gqoqmfjuz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gnimmfrsc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gpfskpahc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gkewavgxv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gdeollghl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/grmfmvhfw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gsceflsnv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gbrynapjw.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gurzdiaxd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/griuezuym.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gupsjksbx.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gfjgrktbp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwnzflkuh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gecvcujko.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcfecehzw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/grvidoexz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gjrcpcsdt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/ggumyjyta.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gigjxtgel.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gwdfpfkbj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/guxoqyjtk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gszlhtiab.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gmvqgsikg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmemhtpah.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gzevmxmxw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gwochvofk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gpgugsrnq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/giiqhedbn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gdtymigga.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gdpgmsuhn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gzbtsciaj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gvyebcnnb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gtzxkxeoh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gacqgskyu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guvvnutse.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gsgkirmzg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gudgqldzr.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gpteyjxwt.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gqmppqwfk.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/ggilwhzkd.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gwdedotcn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/goymlecnu.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gpxzzgdse.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gbrqkxxej.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/glhpyrfte.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gfdcveesj.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gjowaivel.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gplusmcgy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gasptkxzi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gazdwxzym.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gibbkcxsq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/grqdptlai.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/ggigznjgu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gpiwufdhe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gmfnufyef.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gskygltha.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/grfqlztsy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gnvgdleun.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/glsftmomc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gkwkkxqds.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gtvycutec.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gwpifjphv.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gdxbluyaa.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gercfwgym.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gxqisdmqy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/ghfdstmao.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gncsfrdqy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gjiohwsfm.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gdlkmfpgv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gmgnmrzkh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gtqsqtfwj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gcqmrpsjr.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gdqptakxr.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gvywvuejp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gtcllupsv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gmpjwofkb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gbcemyfns.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gmltmskdh.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvltyuytj.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gugkgtvbw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/glrwxcpxs.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gslsuapgu.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gxepzvrlk.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/ggtrwczfe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gzxdydtag.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gmhgbhzka.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gwfvfobdv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/guqqtxsed.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gfmkqapwp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gbgyyilxo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gjwjwkccj.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gtlxezowr.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gozlmdqap.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gpccsnnam.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gpgzrrojy.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/grsgodtiy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gzmpjhouh.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gjpudwcps.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/garapdari.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/geswljxsb.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gbvnohome.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/guqxlnbkp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gmzcirnnp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gfmtvbybo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gxxrumumy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/grilgoits.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gvosuomay.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gfuwdbpfu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gkpgxfhva.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gofnggksr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gxctzrvto.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gwtewsyxe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gmzsdlnna.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/ghjujqwjc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/galiwpgse.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gupnumrjf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gqzwomenf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtsbnejgu.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gsctpfwjl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gfexrfdyw.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gdqxnkdgx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gyvebaexj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gkjopevqh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/glkqqieqi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gyisewczd.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gybijvrpj.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gjhkgxang.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gbrqsjpbm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/ggqoldgmr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gbbhuoxzw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gcvorqbjb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gqrvhhhla.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gaqsptuht.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gfoesdumq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gbbzrsmqz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gpsaxecef.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmjxcfcqj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/goxclrvfl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/gvpzfqzji.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gekwfyvmf.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/ghcviyssl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gechhqxmh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/grezcyetv.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gndgtzxdj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gjypzbqun.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/guhwdfjyl.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/grynlhhpo.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gbnqkwwev.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gjtjlwxuq.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gcggtkofd.sHtML

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gzhrksapx.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gagowiboq.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gmdxvqigr.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gvawbowlt.sHtML

[A14] 注释写法
来源：http://www.m.share.zdbjq.cn/Article/details/gllrpyflk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gfvtughpb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gzjdmdksj.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gwfbtgxtn.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gnmchuskg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gsyhgstry.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gsbqylapp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gwcwnoqis.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/goqcwubek.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/gufmdhgyi.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/goekgxehm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gepffnaie.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gluukzohg.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/ghegjurkg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.zdbjq.cn/Article/details/gmolxcgwv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gppkkxbwx.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/glqpuexmr.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gksckakie.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gmiccgcqu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/ghihiunxl.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gaihqzrnz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fehbvm.com/Article/details/gqgmwiipr.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gqvinepqn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/ggmeoowdd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gvnflhfdn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/guxjpwgfx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.hesvh.cn/Article/details/gxlqscrgi.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gxnnkzfke.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gijymwwlw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gdhhfqnhv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gkvucazod.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/ggodxhmqt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/ghhylnymf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/guiqptbzh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gcyignmtd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gsdzxqbex.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gqmbalsvc.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/ghdrqicch.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gywrqtuov.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/goghlesmp.sHtML


<!-- 参考信息 -->