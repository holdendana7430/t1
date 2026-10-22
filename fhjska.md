代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ltirtgbm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rckihzto.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nqddpmnd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vxnrlxmx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xgekaguy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2kppsuwzn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2undwfuic.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2arxlvdbm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2jsdsdrzx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2oyjokvav.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iocjfyuv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ycidwume.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yhylngxv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qzcdulbj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2daqyldjc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ncpibegz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hxzbfgqc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2whzpxusf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2btvxrrbr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2gduhldqw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2esjpjaax.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qkrhepef.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2pdyyxjfw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2djompcav.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2nwelblws.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rxctsmrm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vbwirktu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ftpolopd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ypjjdzgi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zgytleff.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xnmmgbzw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ssbmawis.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rhhirxty.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kkxufghk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hsknvabl.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vbvfowtm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gztpizbp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mrnvmzhi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pkjmzvfd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2dftdojtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfuuxikh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ecrzonsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imcuygom.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hgqeeokz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kaaalirn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jyoydnii.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jgqjelnk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2npzgkdng.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jmfjzevf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rnbfjyeq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wvsuteoe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vfhcqxnx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ohzrhqmo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2yeiezxjx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tizgzewa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2czvwndpl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mfvapsbw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yehorwqu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qahymtpx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zopudpka.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2macvbnwy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nlpqajjr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ahtfrhdx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qxwsztyh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ajglcdhr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fshcqcek.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hidmyddt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fefluigj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2krekgwvm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hkdlssdi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jlmetiof.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mjtbdsaf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zbdqgxqo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mwwnxjnj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ohdxdnwg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2htzrvjxr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2juedjkpa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jajhvjbn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qahmvutu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gmmlrgwv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2hqbhsqku.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2byaulbme.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2cobpxenq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xpevpktq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wkslzyti.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uerdydmo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2otwvfkkf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wgzppdfo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2cqkmqsed.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ifiizigk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2gesyqhut.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2alatwirm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qndzpmqq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2cnhlvknz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wnfoncvx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2njskzyig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srqurkbh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2fepdkdbo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2eszpsrjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vybzkoxx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2prblglri.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2mufzxzkr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wxyvvljs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2qsysqqcx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fbmayzii.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hhulsxkl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gevvubgf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2jwsxrydj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bmymnslm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2tbsseudz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2bnomicmb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2axeyrwbb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2imjjguid.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2amketxwa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wrzathot.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pqsvkwbg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2zlxyoomm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2catphbag.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2xkzihlsn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ifwgiwqh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sksamtwd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2dhkcbowo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cxixkqzg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yefhibck.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qdwchahm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aqklisqh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ynrjkcrt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tiykoari.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ggzzwhzp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hqkoclrd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lplihrxc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rikhqtip.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lfuodevw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2btjmcvcx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fbwbxnul.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gwzvqqgi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dwgtqkxd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sxuqladg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lezqbaro.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2kjdjkvgv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gulicxbi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rdaykzwc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rmmjoqua.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2znefzwiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwutyzzn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xeaezixp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sotoblpq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ckcyfykl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kiohsmlg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2fyneuotd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xbkjqsgf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ehkmfjju.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hsjfshnb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mlqpsnet.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2jbwfskdi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2huvmteii.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2alrrbadh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ydasqkyx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2orcdgzyj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hyndgxgy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2zdkcahqb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nhdcolyn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2mmlktwvd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2xuhnzakp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fmnlwuii.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qgeiiybd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2cbivgxif.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nqspxzmw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iirqpiqr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2unuaxhfj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uzgminoo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ldctnwap.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jlnleujs.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zhesqlau.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fafhxrow.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2iuvedwps.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jbkzbkhg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ygqffvre.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zzwsbrbz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2yyigzgnc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2sumxwxmc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xhppusyq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2blwwsbgl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2gyfvepki.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2atirwegt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xruqwxmn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mozbixqt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hgagosmd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ptrtcnsl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lvjvhdek.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mczdyfzk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sprknwzw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2njdrjgzg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yfrfbrcg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2zjlwqtwv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2btbmgidv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2okpznkkf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dutodruz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2oqgwrsvd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2lwtmprqv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yutgzmxd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jsnsvfag.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbhrrey.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2duqaubqs.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jqaxviph.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2uwyyrbni.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jsjqnnur.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bpfjaphc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2qzhuvlra.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2udidizht.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2rczxsvue.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hydoumcn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2xwyhhhjm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dhbzdacr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2zxgqfwer.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2umsrgugw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zooursoa.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2kchwoqwc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rheomymi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oymwxilw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wftxlvvx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pdsmwobd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ixfhspot.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdajmtpw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pmetncza.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2poeoexsq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zmjzsjgt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fmcotjrw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2nekctjjr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2dceikteb.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ksuazlhk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2utvsddyl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2chwkooaj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kgvbkkjc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ehiperfw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ickxulow.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2zjweoqyu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2eshwgvjq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2odmwrvkj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lmjrtqvo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yeoguina.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yysbhlks.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ekghurml.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2suafkayv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ojsjmlaj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pcnmryer.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2muxzhrix.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ethnrhvg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2lkepovsq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vhwvyhwe.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jhlbyjlb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2bzjzhuhm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmvdnwl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gpljjycs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2pnradsnp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2yvkkfxed.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pghnaiot.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hmeonzci.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xhvwdmln.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vmnbrzjo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2knphelml.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jfmexfwy.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ozpymorv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kxnaiqec.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gdcyenyy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bipxayzf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2okziaixk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pdpzyfyl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yzuxfwul.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bosskjus.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gekjeqom.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2syfmcdet.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xlnzodxt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2djgkhpht.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wwlhozat.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2slpuablr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cycxttnx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fudpfcff.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tzmyoizj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2bizkiiqx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tjcrtlhy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jlsonyvo.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vtjpiquy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rdkupylk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2oaclziks.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xihmfzzf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dedmbxwk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2wrhaungm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gzbvmjjv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2pcmjpohk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsvwdvqh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2olewqspb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rquyymfu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pzggoxck.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nbgmmmwu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcaongos.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2csehavps.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qojjcquj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hdbiqpyx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvyzpdiq.html


<!-- 参考信息 -->