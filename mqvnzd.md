代发 wailian999

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yugaojxi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iqmytqrj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2sqnvfxkx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hccxdqkc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tuxuyrpv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kpcyrszh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2baqnjuss.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qjfomhlt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wixepiyh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zbyfjzqg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tgijxepr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2htusxtjm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2gwryewzq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ibyeuooi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vgjrkdex.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2llowcewj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2njqenazu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xaxkgpbh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gkjdakou.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2enqpqweq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hqcbhmrb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mcpxgnns.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2tirwijci.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2coogyict.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ytgxmarl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zgsfbqig.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hpaqyjde.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkpeleoq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sjgcvzvy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nagdndbw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2sgagqgzh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2khxxpjga.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2namsyvgv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2efkncmoa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qayuapwo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2alszryxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zprupbdb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2azyyyzwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgdraohk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vrpsbtha.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tzolxlbh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mmfzlovb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qrywgtmk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2imosiwxn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2swdcqjdj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ogsljffq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yugmbtxm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vzydgyhh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ihauhtym.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2xsdnmlip.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2flojbtqc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2axglldmj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kwvzettz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ftymzwkx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2zzidlwzg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yoqkwasn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fqfjansm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rmeydvan.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gedljiba.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2swqjcqhn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dgnpfbsc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2leagqbvm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wrvyqlcl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qemrniso.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wshiexej.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2utmtcdyi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qgsdozuo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fugljrwq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rxijmkuj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ljozysjl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lzmpeuzp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gasvuewj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ugqlcncn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2onbwfvmd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lxjvfaxy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dwnvrtix.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2bucyfzjb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ammobffs.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hixziuza.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nxbfjgfz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2dgvkujfk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lvgqfjkv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2dppjeqxn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ojpvxwfc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ocgnfarl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hebljqvo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2fuzmrspl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2isovnbfe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ygowayiy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mpjgvixb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nqjkvvqk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2xqiqflgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jahsmcyp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2wjcfidqr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vytdbybt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oezmsucm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2hqirrenu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uevvycbx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2fsrfclct.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2cspjrtav.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2avswdzqc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ofytympy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2qzayoilb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qadrzmvd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2qcfqkcmc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2bhyurjaj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2hotsizyf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2imihlwgu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jowwdjpm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2mcotxogk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yhooaakt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2rcjawliu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2tgymkhpx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ngipsexu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dcdveenx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2lssdesai.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tixnwvkp.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2oryvamgw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hvsxifis.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nojaakjk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ggsawnig.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yhmxswii.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2liufctpb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2cgdjcxqb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2racvpptk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nogkewot.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iwtbplkh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ofenkwue.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ptdfwolm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2suroyeee.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bohgurqq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2askqlpue.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ptqkjfqi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2tsilczhb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mickgtjj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abxndsnj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dhugbibi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edrbmaip.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bnldgtgd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2icjdkzgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqicbdsw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qgnmofsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrtjwjix.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2qavkqydt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pimggrwr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2wytbizhn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qpgpckzs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2rxbrkgbz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lityaian.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hvvdmisn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bcewzehs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qligxamw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2cmprnylb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2blirrgwe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mtlbhtix.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hqflgqfr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vcswlfpj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rdvfuuov.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2feuexqzs.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2wqzrrloy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cetmcizg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2qqyvlnnm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2trjlhoce.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dfxdeayh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rkoznohp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jhgeixpw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2klkurvqq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lyzsoqoy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ecdxtqis.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qzyuvmhp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2trwirrta.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2nsflcebb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymcakmsc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2trzydkiq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jlrkgkfw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ticemayp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zqadlnxt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2edhjisvu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zpdtkcxw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2yivpxlnn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vonglgfu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jhkvsaef.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2orfidiwl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yhqxcrat.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tqwimwur.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2svbuikrb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bklcrmfp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fezdoovw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ofjmztlo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zekgzdih.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2rpxurptx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bnunqwdn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2whmpyocd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tptbzpxo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2pkvudelt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ctzvzxiu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yakobhdc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uqfibfes.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2nvagctee.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nmykiack.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2abofdqtz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmvkcmd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ftvnnmcb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kvwonsgw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2wetociic.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cptchjsz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2fvtomqan.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tcstxmwl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2sklmbywe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cikbviey.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2fcorjdvl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wkeffsdt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ngpsnouc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ylurzbfb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ftbcohpr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gcemrywe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2auodxpqa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huqzkniy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbnirzan.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjgdejtz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lsbdmtwu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2clszwfsl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2xwgnxihh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kevuejww.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wrmspqej.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qpqehaci.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ncvedhsp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ibsorzyc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xsvfabdh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fdepratf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2twsvelnp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xygsjedx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2kqjpkjax.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2cqiweiih.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qqsypbwx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tvpojajd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ucrzvapi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hafmhbyj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mgzuvugt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zvvxmbqa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lxuczezy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ivpsfhsf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hkkpxffw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ibkxpzpi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxfuiah.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dkqkacho.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lmmbbsgv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2dqoalufw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lhwsivjy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2twjcjqrj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2oplvvkbm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2avagftzl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nwurjlxe.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lfsvrayi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ffmahpxc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aeysqknk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wnabxone.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ldnfoiou.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mmjomdpb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cayijbda.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2doobtbua.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fafkacas.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tgnatpmf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zianmiix.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gkyzzvzf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rsfykdze.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wqqtfrti.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ffhpswoy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fnlmjwie.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fsgjggoc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2solxmsqj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lrywbqdm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qamsctoc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wiyjlogn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2pgnbgvia.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2gwsczeci.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ynjvhdah.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hbeccxva.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hdskyrlh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tjyhepyq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wtgzxhjv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2gxxshldg.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbxbrggi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nifichwq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2eourbyub.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vximsyjf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sxrmjphi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2fbnxatgz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hwrbwjce.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pkxigtel.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjsratzx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2miftrhdb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgkwxffa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rchlutmj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2awvbmdft.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2axtoxiqo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2xhpzhilp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aujjekjs.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2amidspnh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ctpzkkmj.html


<!-- 参考信息 -->