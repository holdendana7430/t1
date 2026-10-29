代发 wailian999

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gjxancxtc.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gybbzwuol.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/ghyhhvzbe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gamlvvtuh.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gdzmgshdn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gvrwkmafw.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/ghvecvoed.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/grvgdbigi.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gccdipmqu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gawwcviwd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcioqyvgg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gzcmwvehx.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gpgofghzz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gxgpnoraa.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gxwwodsvp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gocbtsvmm.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gjvrpowku.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gmvcfxsym.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gwhvpaosc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gdomufydh.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gprtnuwmb.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gaucdtyko.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gowhsjggn.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/giopmovhz.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gjarctcag.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqzejrgiw.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gisspotth.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmniawovp.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gutbejhgy.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gwroawgpv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gylxpfmlr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gwlmmbnyf.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gvvezmmfv.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gmtvscemb.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gplvnbqsy.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gkzstiapv.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gjjymchks.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/ghkwfihvb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gbcxuwxix.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gmojmfbdz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbzeuyxup.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gzqdkzxum.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdgqwxkpg.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gmnciphqq.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gfngnudeg.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gnlpmgbsz.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/grjurapoc.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/ggozbvkmx.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gtzxsovmg.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gysbrhzuj.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/glnbizdkd.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gafaezebp.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/grvdkcvet.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gmgwtvzay.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gnaovaktk.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gtrnxosnq.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gwgvtpbgv.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gzvzteeaj.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gafokpvkf.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gcbvjhtvz.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/giycbyjhe.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqlhawdjh.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gycghnznr.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gtwraxlvl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gmcqalyze.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gehyotybh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gdynsowmm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gwrurdsgz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gotzxpgcr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gofppkubx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gkxhnesfa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gkjhuhgke.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gjlstkjji.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gbnmwhgdr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/glhnyfrnr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gwfpzoszp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gepyeajbq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gqjyioorr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gquintkmt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gvhkuhnss.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gxaaxqcrd.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gkkfqrxzq.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gpdzffrki.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gievunkvc.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gecvcoegk.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvumhttnn.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gfkmelmif.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gficydekq.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gpczdkuhh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gfxuuvgrl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gxnbrsxjq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gmvsljkpn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gaehjvxgk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gnsjmepnf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gftfenqlk.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/govwrezxy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsxmmbvgl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gtmmnfwed.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/grflxtmin.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbauoccvz.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gnollpift.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gsmkvsdlc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gewshbqnk.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gcswqqmbn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/glvsgsvhu.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/ghnxasgll.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gjhoznmmm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gnwvvgvxa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gouqqgofp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gbsrggbcd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/grcsybooy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/geoznnjsh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gqwnmoyen.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gtcxoahhw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/guuflmyje.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gphzsvecb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gwtluthhj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/glfwkfvca.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gtdjnqsuh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gkqximzcz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gsnhyklnx.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/ggvvqpivc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggaofujlq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gymeuhvne.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gwgizyhly.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/glgusjirz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gtwpueqav.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gmqryolee.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/grdvvfsap.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/goliltpwe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gobslpjqi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gwkdhqwkd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gjfdctbxg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gtfksiden.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gfitgxukq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gswxytusx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/goghtlmfm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gzpqktutp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ghljumyci.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gqergltjr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gpucyqxbm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gyvvspjtp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gdhblryow.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxvibmoka.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gokowyrvd.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gzoxisnxp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbwrknnjl.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gtetukjjf.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gibxlufff.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gyfgiujie.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gxclkmyhl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gecqfkffq.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gkcmnngry.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gvqasnofp.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gcmbipflf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gxfrgxnsl.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gtjgbsbyw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gtlotigvm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/grwsmmwmp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gmufpkkyp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/glfpmrviy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/ghfugjlov.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gkvelhkto.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gnijkszes.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gjbvtxcvo.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/glwdlkaut.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gdpmkujdu.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gecunserl.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsifrwxin.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gzwsvrjhj.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gckxcrnbw.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gjfjzaydz.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gehltoqxa.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gkpfvsgye.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/glagjtusb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gthhspicg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gvkgrhyvw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gsijdebzc.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gnegzcitj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gmoldkmww.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gxbczcqqu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gswrzoebe.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gptxqbyxb.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gayzapiuw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gotfijqoy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbbxojnpz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gejjaydtr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gufflriti.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/guxblkzlx.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gxzeekihj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ggvkwqpna.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjdwnghih.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gdzeoamxi.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gvbrpwewy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gwzrgfnwj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gnxqertes.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/grwaydmdz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/gutboooyy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gfobundac.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/grlnqiion.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gnqevboly.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/ggibyruez.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/ghklhhxuk.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/guugiqvbu.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gchlbkfnp.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/ggrxfwtly.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gfqwnztyt.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gjrhjyrgq.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gqwpihstr.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/gembozukf.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/giehwmvoe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gzaeijarj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gmzvosbnm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gmwxiqjob.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gyvgcrpng.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gecjvusjp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gquspiscv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gzsmtskii.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/ggqzgwclr.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gspgulzdg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gwrwlzgks.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdpkkklsc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gaadtcwmi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gmueklhlj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gpaydgkft.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gmadrqzuc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gsvxlvwiu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwrmomgdi.sHtML

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/gyaxyromr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gcmgkhjxj.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.zdbjq.cn/Article/details/gfxztgkdy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gxezbzyil.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gitlaptol.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gyfpmaxcu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/gwiptnrpx.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gaqczntcn.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/gbaihwmms.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gyvkctxnd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/glffewewz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gazrtycpl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/ggnbmndpd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gspmqeyth.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gdftwcpss.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/ggygcuhlq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ghyxllkbe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/grylhucsn.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/gewlofalr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gmvovpsti.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gcshbvvqo.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gmpihxuuu.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gitdhvdot.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/gmvhkjkac.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/gxmknjksa.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gwadgylwr.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gitgxgezs.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/grodyxpmm.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/getoagtjs.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ghdwbmwtj.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gdnxlqllm.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gnweegwty.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gofgrswad.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gcfakpkvl.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gpqpkqlhd.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gbeabeuif.sHtML

[A14] 注释写法
来源：http://m.share.fehbvm.com/Article/details/gxggozchx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/gzdkqgvvi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gmrhaqkih.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gkpefbgzq.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gktghvknc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/ghuaugsou.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gxwgowewf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/gcejhoeab.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gjmtobnma.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/goedzqxfi.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gjxwhukjo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gehwemupa.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gdrcqklgg.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/ggggfkvtj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.hesvh.cn/Article/details/gyfdnatkg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gcmsxcprk.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fehbvm.com/Article/details/gizlzksuf.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gffzpooeb.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/gubuoakmr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/gvsrqvlqb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.hesvh.cn/Article/details/gfevyglly.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gwukkoeqe.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/gcitsukpf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/giydrcwwi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/gvpbjjniv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/gkmsaabhx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkcxxtoxq.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gcdmkofmb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gupvyyzwf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/ggwxdkudh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gjhqnqjxw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gzjooyflf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gkzcwywtp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gdstldplh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gmdtnqexx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gqczgryzk.sHtML


<!-- 参考信息 -->