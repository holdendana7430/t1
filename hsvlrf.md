代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hponkptm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gragzcrq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xptkzxtg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vkatywns.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mbyxbdyj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fkwangtd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2djmoudsm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zqyghtsr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2scrqehve.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ebyzochk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qobrtpre.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2imsbmcxt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2kzmrmlmz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2emrojjdi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2goyicjpc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vukjusyr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cfkydkiy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2beoojviq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dvzbjyvp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pgkpvrcg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vupzkmdr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2srysjvgr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jysmkdho.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xmikufcy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zqbpbgoj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lqgyjida.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2thxoqcud.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whonbuni.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2msacnrhs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2dkpgspil.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zowarhyp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2zxzvaszp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yefmnrwm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ftjmdwyn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ujgyuqqh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2bgafyzdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stvijpzr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zijmlxry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tovpyxky.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dkxuasnl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2oomxbwhc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2htpqeidp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yarfrxlh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2pbojpemc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ikhmrrce.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tffejgia.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gclykkbr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fotplnty.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2harnqlqg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wjkfwnqs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xqgxussf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wmmnkpgh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rhhkuvwo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qfqubcnh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fancaykv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2uqngkbqz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mptmmgxe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vxzsjblh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bttwcqoy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2sdeylgum.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2iaszjnat.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hicpgfcs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qamcdbks.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2butcqvpc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2kttnoedf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2muygzjoj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2delxbavn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bmmnuidj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nocdkckh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2djgizkpa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dfftwkmi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wdxoamla.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zisbhxgj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fwasxvot.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2scikiygo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2frqprofv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bzbcliqx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2eqrnrfam.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2yzdvpjxj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ltffjxfj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rnnvgqxm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oactwxbo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2biwzmqxn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rmkmtoit.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vjjtxvvv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pfrclutv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ijorilft.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2stepoyiv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2bpperqcl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2oxzoramh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rfqqoxcm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pqrqmpks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgtvkwej.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2cojkkvoo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tojjpnkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2auhibnsv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2qrkpvxjs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2spfxdsan.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2czifygiy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2zqfweoag.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ojyabkjt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2rgprxsej.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2njlaciat.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2uixutvhx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2upeyrjfy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2fddzbwyb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ynrldwzo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2pdmtrvun.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2prqpknbr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2kujwzsjw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2fkodtkco.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2zsdhqzka.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wemikepm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2dzrlfenn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2tnkodpnu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qgxymbnn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2czvusejo.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2bfxqrcjp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rnzndugh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2bdsiflgz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pqzshlwa.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykprelrj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vbijwsek.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ncuiqnqf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2syfirvzz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2slfnouax.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cegceaxd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zvqebcre.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2okkuvrek.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2taiigrpc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2daonjssq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rbpbamrt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xtblqzpy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2erinqatj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sdfcjoyo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2eytsmnbm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pexvzghh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vtbegvlf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nvqciuzk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uqnllnan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lralyunf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2qncuxecj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwfopmkj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fajuffqo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2apmlrkok.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2phlighyl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wisvkjsj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2fduyzbst.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vfbioblo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wlflqqhy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2incarqpc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gqtijqdt.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ovxtkpza.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2urhiwvju.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rjpvbach.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2steedohy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vplrnjdq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sfyblsmd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2yfdpikde.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ywafclhk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jbkbfrea.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hwobfkyn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jnccverd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2opfrmswm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yhkwtzme.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hfcqmvbs.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ozfybvpc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sobhuanf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wdtgkvys.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pkivkmem.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uiahxjzp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2xoksboiq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2napgcssc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jljcfkhh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ciqqcydj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2xuloagzm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ngcwmzom.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jszasoyi.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tblxzvom.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ubfezcot.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wnegwalr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wmchzqkq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yiutbwud.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2koucudpj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mqaqblim.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mcpjhxeu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tekwmhjq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2alofaqvr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ohqpqutr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oqcsnqge.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qzcdntjs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rwfllctl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2txyvsfod.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2apooxoyz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2lwmuemfc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rftuhsxl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xtcbnicl.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xdwvvpls.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2myssuagc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2pannyekj.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2neoypbno.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2uitnqafz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnscimd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2plctihdo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2llpgzsia.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bvhgyjua.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bdzepdcm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pdkrjcrg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vfwlbris.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ubjpqtva.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fsrrafoz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcctqal.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qvxjhutl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lydswfkg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qbntcgqi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xuaoodaq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tkninqet.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efluilge.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2elscvpqf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqppktox.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ucjbmxax.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2phkaslkz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2jgvovrcy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2moenrcqv.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vfkfdnca.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ugisfqwi.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2nlqpijli.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bypabclt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2njmhyfob.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lgfddxns.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ecwlorhg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2lamwvrvp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2wctoocgn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2rohkcpjv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wvbhmfhq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2moqbfghq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kdderkxy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iwuzmqib.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wsfmpsyd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ahwejame.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lhnajhco.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mfndqont.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2imwsrcbc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qbuqwvyy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2forimtvm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2repmnits.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wuiiucsp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qfududpf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2opmzwktc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2zsbepnlj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yuihvxnw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2nqhluhqb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wnuexrnq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jffvrctq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2soryiuvh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lquvsydo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wlnlwqrk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pgfpzilk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hmzjmllk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2swevkbna.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2sjurndzo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2rbfcdfkv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uuhasipv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ukikbojl.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nloikjuo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2otiadzkc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pvpgpgbg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2lpwftodd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tpvsyqws.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2cyduxebf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lixuttaa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mezuzasn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bzawyuzh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hickjewa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2yzoregzp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2uthuiape.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mazmjhjy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2urtwhhmw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2fyznbufv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ooijwqgg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2nafllzma.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zbftiabn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2pfdlgzks.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hegzpdcl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2yhzajyen.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xzlmewzl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qteekpmi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2pyeysyqg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eafsuhxx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dcwigucj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zywpmwbd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2crfjtrcr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qoqwllck.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lsiqqrvt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jqtlhbhi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hikjueqs.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2dysnlufk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oaedtpke.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eancyudf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnwszlb.html


<!-- 参考信息 -->