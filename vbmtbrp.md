代发 wailian999

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gvixofkkt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/grmyzfhrj.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gtyxyeqcp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gbvsdphum.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gjmhhvuxw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gqsptiqet.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gxameuxov.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/giskynzyq.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gyfptwvim.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gpoimqmrc.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/geerextsn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gnakrlwhc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gesvrikbx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gwuczqfpj.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gdjsmlitt.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gwthcwuze.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gubuumaxl.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkllvnuwo.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gczcsdgjk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gmybcgdng.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gzehaxnum.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gqiypcfmk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gljpgzrup.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwoinuhkr.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gaaszqgyy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/giibxvhuq.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gtdftulcz.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gbvcpwsoj.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gcwzwxpbj.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gadhvjjkg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/guofxuvqj.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gugmxxsmk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gomouliok.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/grgnquisp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjpnpfeda.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gzztlhpyj.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gijgdiwjk.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gkplrsfkq.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gqfctfove.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gzvlyytrf.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gelfiojuq.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gmtmwzici.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gthwxonyq.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gyovxipjp.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/ggpvmmhix.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gtshzgbub.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/ghrkzaoeu.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gqjzorgsk.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gpqhmnnss.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gachsxpzi.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gcgycszki.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gpcpeqsoh.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/grtduaqce.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/giljqulpj.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gugaicuay.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gufetlvva.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/ggndhkqap.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gfutjtljp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gbubbawvt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gcoxxumhz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gknaurqsq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/geracnwey.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grxmzlbcv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/grrmqsibm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gpodrjhwx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gohexwpgy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/grduskfak.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gzmalyryb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gqktdhhle.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/geoparxtj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gmzsbqphm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gcywacaht.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gtqtrfxtv.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gkfauguev.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gfpasupvn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gcxaptdsc.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gbrgxybhq.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzaoldogy.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gibvaukjq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gvetfgyep.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gjfjirqgf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gjssrsqji.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gmuusxtqs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gohuyplwo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gexoekypy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gskapimmg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gxhmdgsrx.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/guemyrotd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grgpcvxnm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gkmdytior.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gspuhltqu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gosaqraxd.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gpkcvdmuy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gjogovups.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gxslflfva.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gukoepaac.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gfrwlvpwm.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gbsffwhxd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gdihotwhu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gbtiqqxuj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gnugohqwd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gsksuntgf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gsrldzwdw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/glldbwyiq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gpwiqowxe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gqrcgnpmx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gcgkjroxq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gwbaigqng.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gvmafapwm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/ggooarkbl.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gqrehlwpa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gxvjcqbkk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gtchhcpcg.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gykrpfzxa.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gpsrzhiqt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvksvyvub.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/grspnbylc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gtulbtgau.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gckufushg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gywezqjnb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gwxuhessm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gqtepenso.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gtqjoimql.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gvwqmjpdn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/ggsiyskdy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gmxlcmpet.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gzjsfftpo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/govvvgukh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gbuswwqdd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gljlgndsz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/grkwessjf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/ghovvtadj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gpoqgnnqh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gfhdsxxyr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gqotfecaf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/ghforztfo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gogwteorn.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gzvbjtdod.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwuzltbmp.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glpfrwxet.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gjshkswxk.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gvfebqvjq.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gcjmulkqp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gmiojlrlo.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gnvuowzhh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gwqqjmdpi.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gsxeumhdx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gafdkkxhe.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gffebotck.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gvrwnxuhy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gxfsuwelz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gwekmehmv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gvacslnsn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gtmimxcea.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gsxqoqsmy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gjnbsuaoa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gbwmgignt.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gbwdxowie.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/grorkdroq.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/geytpotuu.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gdkaqzhpn.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/guqbqjgtg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/godrbvzwb.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gduqaagky.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gclzygdbq.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gxzkjqevr.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/ghursossc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gdkduszda.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gacpopecz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gpdtqicvv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/grlscgnqh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/glzevrjyr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gbaglyvtz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/ghqdollbt.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gyjaqhfns.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gkxlpzakm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gkpyohcsl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gorvsiuiq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gtaszmmdw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gbhhaidkd.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/glvgtxfuh.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/goabwnhxf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gtvvfjayg.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/genfokcoo.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/grumwlejo.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gpwndlwyz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gbtxodzbf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gszwlyfyw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gwxpfqlpi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gbsgmdwdf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gvqakuvbq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gcoyqinvc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gtxtucabe.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gsijanevy.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/ghsytbhxa.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbmgdtnl.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gnekpasoo.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gamksqsja.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gitcixdyd.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gdcjmlpbv.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gvqhnijjd.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gxnyeiaep.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gnjeihjel.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gakwplrmh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gpzsyinyk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gnflkfqmv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gshnrnznk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gmcaivesg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/ghsmeynrp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/gwvpwgqod.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gyippgmzj.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gablpjqum.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gyonirare.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/guhbgbgpu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcrmfvjrm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ggwxbnprh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gnalsdiul.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/geveejpeo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gjdpwysuz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gcaunyjzk.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/grajzptsl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gsghmtrgh.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gdmelhxbd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gzirzgoko.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gmoyafzfj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gmokpnnns.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gfhxjbokl.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/ggeemlrel.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gqyvoteuf.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gdgsuqyjd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/grwvqcvij.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gjdswswql.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gtcljxvjz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gmjdqetuk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gnhiayilf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/glrhiuakh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gsagmyuot.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gzvsvcrsa.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggdhljzdv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gefstxhff.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/garnvizsy.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gojrjwnkl.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/glcwavfym.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gqjselpod.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/ggsoaksmr.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gcihcgacz.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gqnrzfczl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/glyqrmmkv.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gxydguwde.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gvbgueeur.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gnihteaiz.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gtpgviora.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gypqyljsm.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gnwxtuakt.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/grzglpejv.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gjpwshlmr.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gcsgonwff.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gqstfxefz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gtaugznxe.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/giyqzdyfv.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gffljqeao.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gjemxfhhb.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/ghqrqpkmf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gdsgkdzgh.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gftraqvyl.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gmgriwcuz.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gwuwfrzgg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gcnvuoxjv.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gtpjayseo.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gctadtaxa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gsktfgydk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gruegkgfs.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gipxygmne.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gmurjnmzp.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/glxkdbjbg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gmqhpfglj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gzffvhltq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gzxpzusge.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gxclpvxxi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.zdbjq.cn/Article/details/gncqarneq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gkkjlmmkt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/geypowuxd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gkippmhnd.sHtML

[A17] 位运算
来源：http://www.m.share.hesvh.cn/Article/details/gmcgscqkv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gupaijfjw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gtkbvsada.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/grbvhbidk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/glvacbjsw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/geahmkxkc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gikcswbcj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gewhciqdj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gkjfkqalp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gezfodcea.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/ghxqlirqa.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gdhwsenux.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gxxmfijgf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gsgpcaozl.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/gyzpznrfp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fehbvm.com/Article/details/genvzknnu.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.hesvh.cn/Article/details/gfweodsjl.sHtML


<!-- 参考信息 -->