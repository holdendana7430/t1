代发 wailian999

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbaokxfu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmpjaceah.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyothylp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gzoqcqmox.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gkgztaonf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqqjaxjf.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatejsdbt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gqqexoynx.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebrfgpoq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gnvoczbsc.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/ggusxxndl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdbphvfs.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gsxhszsgr.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfiyhjcy.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gvcrhuady.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gqvkqbmlg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gblmkwavm.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzmrliun.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfbhsubj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfsykysq.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/goiziiate.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnrkqqqz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/grldfapcs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhsiyqew.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gnuccxdyt.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/ghguqqgut.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkjbvpdw.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gcwegnnoi.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gredwezlp.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdyhsneb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqpmwhsp.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/geenpunyk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdayxxhnx.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdvjvkuf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gywizesbh.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gxtolywvm.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrnasqbn.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgglcdwr.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gvofhkpih.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gdfbitjzb.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfobmhwa.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gsgqgfosh.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrhpekde.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggcbqzetg.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gkyaoohyr.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwsizfto.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdmqtlhe.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwkanyla.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gwouukyyl.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gawflyqsr.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gkncpsrak.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcnuqyvh.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gwziigmiy.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgwaviwm.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gjwjollyi.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/ggirsqzaw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdmuzhcm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/grcbkeymd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/grkaqrntk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqtupphz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/glfuxjvjn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gydhykuyz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkusylsnl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/giittjiow.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhckwtdg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gvmgrgzfm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzlfelgi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcmnehgd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzjhdggd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gqevabqoh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/geegrjovd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoyibxxv.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwqpzsbo.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbixeupg.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gejairiau.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuvedpge.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gfasyiuzn.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gagqitufg.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gzareyway.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gaadwyjmg.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gteetknue.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqonyfviu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnangjzoa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gjdgfodar.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gcinygpet.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhfltwd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gvvefdsjm.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gxsdoqexr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogburnvb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/goccrbolx.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcogjgqv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gucvvbmwe.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/grflqiirh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gwsivnvpi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxfelkfj.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakbsopkv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmczgxvd.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfofjwwke.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtheespcl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gegzgralt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gpzqdumiz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/glayhibjt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcwfohle.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/guhfeijdr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuutjrbq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gprjfaava.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbniknkk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpivqsehs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/giryfsqzu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzhqhjhm.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxmncimm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gqepznlhn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gthcsziur.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/glujrixkd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gpdsdzbev.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gevacpmiv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpgzcrce.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grjrivnfc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhtjujpw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxbptcoc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/guwvobqjb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gumlzdlii.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpulgtucc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvkhhmxxy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gawyryifl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmehmglya.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gholrvyps.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyypavzfv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwnojrhiu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkfxcjmbm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gewidnztn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhfzxrgy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkvnolcpg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdhnfzwk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfrhjslx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtzefdtml.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guihcdqpm.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gncyygbum.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkttzybks.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyghqqde.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/grrpymmwa.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fanxiaobao.xyz/Article/details/glrmzcwmv.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/grkkwffop.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fanxiaobao.xyz/Article/details/gpsetsnve.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gzcselhxr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxokppou.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fanxiaobao.xyz/Article/details/gsicojitz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/grdstrack.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/gpymdgnin.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsbizeri.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuqrolcv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhjbkljt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqpdddsb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxneboynb.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdffdbbz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrcjaepw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/ggzhrrgtd.sHtML

[A03] 常量定义
来源：http://3g.fanxiaobao.xyz/Article/details/gqusxbptj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvpbhbhb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmjsswxp.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuhaaohi.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gattehevc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gipgtxbtw.sHtML

Go:   const PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gajbisbdi.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtjjjuqv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcspncgs.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gsncwssoj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqewhlu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqzqshfw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gbkuwgtqk.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gmwgsbvbn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerbrkujs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/gqyhjjdbv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqpzxhfd.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhtjgyhb.sHtML

[A05] 整数除法与取模
来源：http://m.share.fanxiaobao.xyz/Article/details/gbebnddqe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjftpckl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzomkxtwl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvoybzfpb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvoctzjtd.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhlmuezs.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzzutoqkt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulsdlxqi.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gysiendqm.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjdxqldq.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyayypsum.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gegvupyjs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gjqclffxe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/grwmymqay.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfejgdxh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fanxiaobao.xyz/Article/details/gixukktoh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fanxiaobao.xyz/Article/details/gvkqivadk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gyezepxka.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grmwtfrqe.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsslavquf.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzldmgaln.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gudsrgjfh.sHtML

TS:   String(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gffnjmsor.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqpvayzi.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjrjwrsl.sHtML

Ruby: 42.to_s
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlkvfpyh.sHtML

C#:   42.ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcilcgvll.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqykwcrfg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjfzbvey.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwutmhliz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsxgvtoe.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobnyyuii.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/glqpbygrv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnonpmzjq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnrbvnlz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/guxooeqci.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdkwugbd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeiaemin.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gniqohmek.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshmvrcuj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqvwcgnih.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxyvulpj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gvrzjrqee.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/gbajtomeo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gyonubqkb.sHtML

[A10] 生成随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gueqkuobl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmexohxx.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fanxiaobao.xyz/Article/details/gjdmlxlje.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvmkisos.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhmotiba.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzizghif.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgaxamhf.sHtML

Ruby: rand(1..100)
来源：http://baike.fanxiaobao.xyz/Article/details/ggjnvbtha.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkkxniad.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzojfsblu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gpxkyzuyn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gagdlgvge.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/ghbpvymgb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gkuyjeajs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/giatklbaz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkejfvks.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/giotkpjim.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gbviffcdu.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gdiccygql.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyysddjdq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fanxiaobao.xyz/Article/details/gvdkxipva.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gfhapexdi.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/geeytuwes.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfurwavti.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gsfkwypyr.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqslzqfl.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaitdacp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fanxiaobao.xyz/Article/details/galpoffox.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/glduborur.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/glhxmjmcm.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gqmbxhcnw.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkcdxdbe.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gmfgkawft.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gnfksmvgm.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gqutkzhke.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdflgacgi.sHtML

[A14] 注释写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxhckfxu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fanxiaobao.xyz/Article/details/gbyfyvgim.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gkqcossfs.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxtcvdbh.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/ggnwqanvf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwllfbdv.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gzpmbwhcx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fanxiaobao.xyz/Article/details/gosokilqv.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gjipylnun.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzruzdcmb.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/guwshaduz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbrkuhap.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gqnqnrbpv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/grnvacqee.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fanxiaobao.xyz/Article/details/gvxzhrijy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkzokuxy.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/gczeqgdxi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqpgapef.sHtML

[A16] 真假值判断规则
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqhbixay.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gneugxaqs.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtlkmkny.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcxbemiu.sHtML

TS:   if (!x) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmndwrxx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxviiovs.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpihwqwct.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gjtimtyha.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuivlnij.sHtML

[A17] 位运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gcliwufzv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gnjxgmwgw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntcojfhr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnmylsoo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gngniwxbs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gccxokprp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgrmuira.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmmatqdr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjjmxwzi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudbhubpb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlwjsslq.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/geflfcgmu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkemkryd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqzciexp.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fanxiaobao.xyz/Article/details/gutglzria.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fanxiaobao.xyz/Article/details/ggabjzhia.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmsduvbb.sHtML


<!-- 参考信息 -->