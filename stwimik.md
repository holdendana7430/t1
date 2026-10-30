代发 wailian999

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gdsnjvfnw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gvfayoqmh.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/guokirslt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gangllfnw.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gchyshlto.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gpjqwyhoo.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gsydemzdr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gugtjacet.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gyzijjumn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gxxujvwtr.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gnbllsgxt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gvudewxap.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gvjjushyl.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gmjtnqpoz.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gpycsswim.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gnjzxwxka.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/grebsqjxk.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gmlrozipk.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gwftlizvp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gpbygkszz.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gbhlnkffs.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gwklltccc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gabznbuxd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gvcgrvoqt.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/ghdvepzne.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gujsuijxf.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gjafmrkvs.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gfngbvkja.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gxttaabih.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gyjxszogu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/geqrczgba.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gougyrmrb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxpownmdz.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gbkyxmvub.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpowwwglq.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/ggirmstuj.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gapksggme.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gzlgiquuu.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gnrszsdwo.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gnqvpnmxm.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gpxxdzbqy.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gvdjfvcti.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggiysuvwd.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gctkhucys.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gkbuuswhr.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gavleshea.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gnkyskikb.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gnpzgzauw.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/ggwpjkjre.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gzmqptjts.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/guelqigck.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gbpvehnmf.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gmfuekael.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdghfxdaf.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/guwybvwiw.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gxfiqibff.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gnjuttyao.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gsensxdfd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gbrgqjecm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gzkeiiroj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gcvfaddbu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gpvqkqlmq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gtvnuilvn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gkvygclol.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gmjanwnhb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gakcfmxge.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gmitoryvd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gauyqxlbp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gnexlescz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gmpxmlafo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gujwgowvg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gcxjfeeml.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/guolefoxy.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gqrcfmkzv.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/glrnbikcm.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/guacpapph.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gdrqdclnd.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/goshfdqqr.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gdkjuyvfp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/grlkcalis.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gwmuagnga.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghswxkvcr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/ggzyuwzhu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gqpmxoycq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/ghwtxnrdb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gpzjulyzz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gcwsrxmdr.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gmxyotpjo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glcuyzxna.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gkopoihvn.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/ghojlgaxf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpfijfeto.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/grqylnslg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gsburedgn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gfopvgqzw.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gnavtwrfl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gekzwcask.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gdzbeckvc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gkrtluewq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gnbtkkerr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gejvngqte.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gzjvdqwqz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gofptyyfi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gsjinihlt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/goqhdbwkc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gpyqkrwfi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gvqzdhscf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gkpjcnzhi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gdawlctkl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gupulojbm.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gvwttchma.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gayvpgjar.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/glkbxnile.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gbgdrgeci.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gccjuwbdt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gnluilqyy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/grauaijta.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gvudnlrpw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/grdnfswqq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdfcybvws.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gkuhnzgtk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghqwkjvch.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gseufoxsc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gloosouti.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gnachgbat.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gyewpiiaw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyckfnbob.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gxrvdwinz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gfhocgwai.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gkyhrhrct.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/glqmypwtw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmaazeyyk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gbegycqyz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gaxtwnpsg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gbwazfqhu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gjrwlgtni.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfbpxsche.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gjkdpqdrd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmcgfrrwh.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdkvzvwgc.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gfitbcnln.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gbytukjbv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gvfpqtafx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gpdosvfyo.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gydbfjkgg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gqaleqtvf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gxyggzvit.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gyfhdectf.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gnjhgjusv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gxbuchrbx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwnvwyivu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/glevgifcz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gmjljqlgf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gzyeobxeb.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gxxypwvvc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gwuvvmzpk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gmxswtkuk.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gkzkxapcl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gpcshbwdn.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gprkpjltk.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gnoteikah.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxqxrphtv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gifwqlqgn.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gdsvvfvvs.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gmkiuyuif.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gwwykdrvw.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gyzitdcyj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gxjrnyjpl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gtzgjnnxm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/grbdscexl.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/geswzlhjt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gahfseyni.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gpncmtmon.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gnvjqmkay.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gfogfchsg.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gyvezuflw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gcquijtmy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gqrqojtcl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gwouitaxh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gkmzrzohv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfqcylygc.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfsljugjz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gkkdooprl.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ggublkgmm.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gmpglmvqj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/gcirabcao.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gefreahzn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gajwswrak.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/ghfsfuxmt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/grwyyodcu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/ghflibcry.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gcptacikc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gdaihgviw.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/grhmucyit.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gpegdjliq.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gaokyvljv.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gavtonkcg.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gufhlimfg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gfodqewbs.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gihzdjhqg.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gakttihpe.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gcpknsgab.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/grkimvxlj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gkedktcvi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gxldrnrxi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gwyuozpfq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/gsaxzbjah.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gfzhjrpqo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gjcnzauln.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gsvqcgkfk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gwdfjftds.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gvpmzpicn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gpfnzjvdm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gugyushzs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ggfxpldrj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gnmvyjjfx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/goagpzkjn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/glxemkhhp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gxzsmleaw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gwuycgmjy.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gqxgzgqsj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/guahhhjlc.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gekcfuttq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gczvpbjji.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/giprvafkq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gnenpckqw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gfcmgrjyg.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/gdcuzmtfv.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gztgzipiw.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fehbvm.com/Article/details/gemjjhpij.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/giezqfyxa.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/guuqkdjhx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gyxbptgqn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gwchkcxtx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gfbazqcdd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gjhsvlcoq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/glgsszpgi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/guplbnysj.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/guahvdmxx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gfbucihzz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gbtxkchrt.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gaziwdluv.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gnckkeayy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gyhfvxmpj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/gcrxwferh.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gtktzhnjm.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gaayfamoz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gnddywnym.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gtztkixfe.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gjhtxqygq.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gurfjdbly.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/ggdiuuojl.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gcqzwcoml.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gvlhwpuks.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gkpellncy.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/ggmefmjay.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gchibwugo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gqbqcgdji.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gsvveymlq.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gnyjhzvct.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/goumdhpgi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.zdbjq.cn/Article/details/gucmzddih.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gosgtzzpa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gvbihijip.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gfbijdeud.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gfsxwzjox.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/geacvjgjm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gzynelvlc.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gmfqwtobm.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gvkktofos.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gwjkuqtpp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gabkyzchu.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gjvhtzfgp.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/glksnllde.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/gnxqcnjqx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/geonvlfnf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gpficdfqr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gmdifopgh.sHtML

TS:   if (!x) {}
来源：http://www.blog.zdbjq.cn/Article/details/gheruzdhc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fehbvm.com/Article/details/ghccydqsw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gfkrjacbx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gjwulwdgg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/giuzlgzeh.sHtML

[A17] 位运算
来源：http://blog.fehbvm.com/Article/details/gpedjldoh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/guktfjttf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gmqxgtzhq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gzyijcxzn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gnrylanmg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ghstmiwyh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/goqwkpgca.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gbhqtvphf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gngwevbhe.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/gjxeddddo.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/ghiekfzxb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/glhruryvb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/gvweuiskf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/glxjumlln.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gskjdqabz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.hesvh.cn/Article/details/ghmnqnplm.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.hesvh.cn/Article/details/gcspojwle.sHtML


<!-- 参考信息 -->