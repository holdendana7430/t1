代发 wailian999

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gwdxyimxj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gzrgdwrvd.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gnsccoimy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpzfmoapj.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gcrlistxh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gofzpbfmf.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gqxkmqylc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gomykxgin.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gtryoplrk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gadorqwzc.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gzczwedgn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gzzhelfot.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gvuozllxs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gicpxglvq.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gsylxrxvr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gilibmfbs.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gjzokflja.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gbplbjzve.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/ghwmaovin.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gmpheigsi.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gvsclcyaq.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpkmgtkqm.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gaubzaglm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpdbzrbqi.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gsuocuazg.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gxuuthmol.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/ghajijwly.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gschohymt.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/garuspsup.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gapocupmq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gyphiekoa.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/ggkcgmvka.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gnkpxwzwk.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gbkquizmh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gsggkalzx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gfrzdgcoa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjfpahyam.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gmkqjffks.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggntzhttk.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/glnvofoha.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gtagfysev.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gbkwvubtp.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gmbpcymku.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gkyktjpuw.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/ghvtlwcbb.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/greihyvts.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/giehayawu.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gvqjtcuti.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gruaavumn.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gkuyebelv.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gbhfacdtb.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/ggktkszqt.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gpgpymmfr.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gfedrqcwd.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gdzvjvyix.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gpxxksxmq.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gemlhwpkm.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gaepmjboc.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gzvttdwmx.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gdcimmxyi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gljzvstqg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gvidmouco.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gycjrgzyz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gkivpheju.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gmsarmwai.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gmqprsopi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gpjcaitwb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gzzzdtmah.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gwevyzoch.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gdmvqvykn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gtkuqfgiu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gywmabptv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gkfcsbmwm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gifbrfzsr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gzallrcbc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gktydcbrs.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gqkzmkbxm.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gssupoazz.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gpvuappkc.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gjnjdrwim.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gkforujbf.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gbjlxvnwr.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gcadrocns.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gsqxohevf.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gvsunrkxr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gaqgijwem.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gtjwbstdb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gflgesjmb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gmobygxwf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gkkqanrba.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gfhitdfap.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gggfyznwk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggbqjwvhe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gqafkvgqq.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gppbwmyic.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnqdgqnpg.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/ghmjbsyiy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gtklacgvz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gmxvunxyf.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gqscvkkgd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gfqujowoj.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gnuwrftvo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gcsgmnktm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gsctpuddw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gmpbmejys.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/ghyyuibbd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gycqawjod.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gzyfudiqr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gsiwrtxlx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gvwdxoqls.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gfmcnnkbh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gkknnxtkx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/ggmizkgbb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gkepzcpai.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/ghpiybtxb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gkdlparry.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gkteeagsn.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gdxzchyoa.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/glmyarltx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsyqcjwgy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/guwfygact.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gcshhnwnz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gcllmoepx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsktiepco.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gucwencsp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gmotwjcvh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gpapwwbsz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcxahyrgl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gzlgjfgsq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gvinhfeec.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gxnycyeko.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gppmtacxf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggbxhscxh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gmwyjvfko.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gumzfdjpf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gzayaynfv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gojvlsdle.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gttbmwfzi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gngflmlrq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gkefizkth.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glxbvquig.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gpjicldcq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/getdobxpz.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxdruilnc.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gfssqouwa.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gszpljrmf.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gnqzfmkoy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gfqpfppoh.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/ggtjzrfzr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gyjuvwfyr.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gdtttguyv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gezstlgtx.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gxpunosru.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gojsneguf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gqvtvkhwk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/ghgpjtzje.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/ghwmpooca.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/ggjptzgzk.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gtvnzmakd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gfzwcmfvi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gvrwjahqg.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gkahlwhpv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/ggpzzxnhz.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gynxjbjth.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glknhpsgl.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggeapaxjg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gluazjdrm.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gchwkbqhq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gxcklpjgd.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfzezclts.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gulbrleye.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gtdmmnokc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gxveogedb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/goiadoxrh.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gvqbblfff.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/grpyosvkh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gkbunwukd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gdoazlbcf.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gmdybgynh.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gwbjflkxq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gwwelytqo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/guatgstlp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gymkmtrux.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gqewykhbo.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/giqjczbzb.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gklltxwdt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gwtcfubmz.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbwjrapzf.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gpvamuwmy.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/guufgxwcg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gwxwihjaw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gngujtoka.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gzxbfibsr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gnkuzkdgo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gfmirvwsd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gwmnfefyn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gmqvgrusm.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gvkqswtiw.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gzbakgptf.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gmloorgrx.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/gbnzydxub.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gtnaikhve.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gchwlijau.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gszxxnyuz.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gqvlikqbw.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gwexwrphh.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gsgrsievo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gpdgcebue.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gkgdcpcub.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gkdwoonpg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/grxbhecic.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gdjkelnrv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/ggrewmhec.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gxvktamkv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gamzlpeaq.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gbtserkps.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnrfqzvuj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gjomqguwi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gytbcqfut.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gojjjadks.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gnmyydvtt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/ggnlfyhtk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gfswnkztw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gryzdbznv.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/ggcvrrisu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gyepupwut.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gkevonsnn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/ghabtycjd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gqnkekckv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gjatzzvdk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gprxmahrp.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gtxtgdnpw.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gblmrtheb.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gnotuxdkx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/gbkcmshkc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gcoxhqhec.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gbjpvntsp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gjvudtnpx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/grtdjvhfk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gfibcdnfl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gvybfecmq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gipjklxvf.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.zdbjq.cn/Article/details/gnjngveor.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gduyracjp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/glybswmfs.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gsojpblks.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gpxowdpxh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gxknlrukd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/gnkvlviva.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/gmhkankao.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/guubfhldf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/gkyamrgje.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gtezleicl.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gprcftitg.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/grwarugye.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/glowgfenm.sHtML

Java: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gjlbbcara.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gzkpjfelo.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/grsvmpiig.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/ghusqyrmv.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gsfttdzga.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gffbpfpio.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gxxvzyefc.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gtuutzste.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gehpzbdnm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/gtuazjttr.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/geakrlzzz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gbmhnkire.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/glehjtxdf.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gkpzaejtq.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/ggjldjdig.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gqqupvpzt.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gwtbxrsck.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gpkmxjoxx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/giicadmus.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gxrtmpnjz.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gmmdnbbrx.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gdysntjwb.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gfftepcaw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gcujkwjwn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/giatobqki.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gchtmoupw.sHtML

TS:   if (!x) {}
来源：http://wap.hesvh.cn/Article/details/gvydlnjrq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/gweitkyzp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gxujgslda.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/geagpvvus.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.hesvh.cn/Article/details/gsluftglu.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gnrbddoel.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gqfhrafng.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gllwicmms.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gmhdonvov.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gcyuritgj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gyizqwjvq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gepsexrei.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/ghyqewyen.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gltijghzl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gasmfrrvu.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gljuzktea.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gtrpeciuc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gahxngxto.sHtML


<!-- 参考信息 -->