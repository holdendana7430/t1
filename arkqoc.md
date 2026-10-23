代发 wailian999

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jyrlnxpy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vahamhzy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3uuglrodn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3vfaydgvk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3cvnnvzgn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tfshiomf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3yijezqxu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qlgljhjd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3cxfoxquf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kkvrrgox.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wuibdybg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sscifynz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qjxisgey.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fyjjujjo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3oysqtldt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ajzjozsk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3sxfpqcqd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zquupkzz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hgednxzr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hktnjmbm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3suubunnv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hqocyzve.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qmnxiboe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ktnrshdc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ihwgwgxn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gegphtwd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3gkvpzhsv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pumpnczo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lffujklf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gsjinaiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njfydgii.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vamqnixd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lavendjr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mnlzppvv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3sggplpbk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3rcdghpea.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3htfixlpk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xoaeozlo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xcyvyaym.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3svvkdlbe.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3bigjdvue.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mbotubzf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3xoxofdke.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3oavphdzt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vdopcwum.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3kfertstb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lbjeimls.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yhqfnhur.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cejuhkhd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bshtnmmh.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3llgqtehb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xavjflbo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fzukvgle.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ktivfokg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3avivqitn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tyokqkel.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vbvakcxk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ogkotfsr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qgaupnjg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3owlcjekv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3phtnrzap.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ldbbcpyx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zzxhneki.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lwypihcm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3arrczxhf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rfkjhnck.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qdduqtiw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jhjqrkop.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gkcbdenn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3uscaacrc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rhdqnifp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qyslbpog.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3sfrncevc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fiihukcz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3esucwytb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3onghzqes.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wwiuqlub.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xubocwno.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3appsvarv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ssihqojt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3llyaqxbi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3gartrhqf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3vlxskgdg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vhjqzyes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxerabto.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3peuhijau.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ordumatn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uothmppb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3cqrtehii.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kuifhpyr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3xhrllhiu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3trabdjve.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3salfggan.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rhwajekz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ewedmvsb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3kxujvqkt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3uqgadshf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bbzuqeor.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gopkpmcr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vddppand.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3cgvrludr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3gbdfqfrx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3emkqytsb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ekgaslpx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3whcjblbv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3volukccw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3scplltiy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3zoobogke.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hxjlgmlw.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3iepoagii.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fakrucvx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uubrvjvd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tclppzuo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3puvxjnfr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gvcjgjtb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hqrarxbi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sahadgaj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnezxcwf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3abyrowae.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nvqgybem.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jusvxzgm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wwsihmfb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eeqktukk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ttovdnjt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ksyewdub.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dsdullka.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnygndnl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lodlasmf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3knhyfwiu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wavqvrpj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ojcgwdsq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ocvuvyos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umhiogwi.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gzdmlitn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrbrjscq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wyqqwhoh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3htudvmhd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3jnokppji.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3taynbspy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pkfixjbk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dpjrsoij.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3aaqiqccr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3zhkphlpf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jildlari.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3seompokh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3cthyhswm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kcxftpkt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vrjdduxi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gjnowjfc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oogldocf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3benhaedh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bwflvnho.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xxouszyi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3hnotviso.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3jotdwjhp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3urtfcttv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vrogoaip.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wzkblvsj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lahokaqv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3iyixhlbw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zxzgkbok.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fgrxbhmv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pwonmjvd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3rsajzkve.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwbjxbsh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3toonojnn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ymuktucx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3luaswovs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3sztpurgj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ttthqmiz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xfnqxicf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tgcyfnqe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lusgcgmk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cpeiyhqu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3drmxphoq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rpqttlju.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yddnktcq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3huyvlsjh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wxulipqp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rqyyyzfr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xxvhittk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3knoegkri.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3iwdqapyy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xrylfnxq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3phefqnox.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dalxqcue.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3pxygrlbi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3xfwdjxoc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mkbesvtc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mlcmuttz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qovclljg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jutwtwiy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xupfzurb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nigeyemt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3avntutxq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uxluklyo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jygbfxlw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kzprydpj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3pwxsnkeb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvnitqn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3jtoccmfd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xsfpuyhm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3rsnxbxpl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3voryesmx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bfdllawk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jpxubcaf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vdvbzyfz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oyaksjij.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ubipzarq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gzckvkhe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nzryyddz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3szarmnjb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfyqhszh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tdvywnge.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3psivlnos.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3elfbbfdo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ktgsoscp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3detdscmc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3yfbyspij.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mudekylr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kawsftbw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fdryegyo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3runolpew.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3azklduwb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqjzmzm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3yqwyoobk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3boxzsvgn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wvwigouu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yxdounsc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3edinhytb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3biovuogs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3onzfochw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vihwvbui.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eopuykja.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3iwhqsjge.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqftsgif.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3augqcrfs.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ctqrubou.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3qhkezknt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3avpqwhkj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ptzggbji.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3apnuneme.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3oekpqejv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3crgijwha.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wwlsvvrt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nuajrgyk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jwrzdjmb.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vqjksxet.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iywbfjcw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qxzctbad.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tabincss.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mbzslanb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nbruzfkz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3oqlagfqj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jozpdcyv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mxlhtbba.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3duhtambj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3fpmghggf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3afhlgvmq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3emdweegc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uleovkhk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pzgqdfgk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3luylczjz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gdbpshrd.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gwtnroir.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tfaoctau.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hciiqzmf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3jerhsldg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ybapjwov.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xvraynww.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3owahsrvs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3rvpputdu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3kcvaqgrg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wkpcrhko.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3qcpxxran.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcivovfb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3kwgcjyxq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3aucugcve.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ekzivork.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3nsepjqte.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xperdeti.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3phdqoyhe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ixckyznr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmvmqmqw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nyzaexib.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qiyyzpcc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zogkehjz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3waainddz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3mutjjurd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wurpoovc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lrpdtcny.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sqjuhyik.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3pabjyepj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mviyzimc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3aamkriss.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fiwxoirw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3pnnyvolu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qrjneuio.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3sljktjva.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3guboomas.html


<!-- 参考信息 -->