代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3vlqosppm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3lzmqmaeh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zmcmqikx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gwhrbvax.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rzndonbo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wvxkyels.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hdstuxjh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3buhzijun.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3prhdzxzl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3deorielo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3njijkugv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3whsxxkay.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nfplampp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rtzsdotl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3rnzlanch.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vnvbmjny.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qrcutogx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zblavdny.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qviweqbi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qivamtvs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3deqlxufx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wvjrphyu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3cacqgbwq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bedmgkcv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eipgtder.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wvfkpnkp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jksfprax.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3glnybchk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jebhmjom.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3oqywueow.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3odhzmzlj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sjyxzpkr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fdncqosl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mkxpipzv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3nloqirhq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rilpwshf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vryufxdl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3iyhvobjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwrshndp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jbbrhfog.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mfktyloj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3driyfudi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hvuojpko.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3awblaaai.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3adoitqsu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fptovgqh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hlkqqbhi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pognmncr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3rplpsfht.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bhtjuohx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gnwvsojx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wxxqvymb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bptuagft.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yuttthks.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jcsvkstw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wusyhbtm.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bxvxsedu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xjgplcar.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3eigmijfi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3iabaafpi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lmhcbfli.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yymjhyhh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hqszlnlp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3iprrdmlr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3dqimlklc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rbaddkzk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uwsqwrnf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ausxtene.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cavdfkpn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qdonllyn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qxhkmbwl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rrkgicis.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zlzkywhr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fumvpzws.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3kbciiztx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dnpkclll.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3wmaxrtom.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3llzzukwh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zjwpiksk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3laenwnkg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qyrlrdta.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cqlkwuhj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3fsvsunwr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3govhjaad.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3yemdrhht.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dhmatxxn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ryylgfaq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jfwycevw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3fbqzcjbj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3klpvrbik.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zuhbbvuu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ayssbpwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvkgaeqd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3hhtjktkd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3elmbbayu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pthussao.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3etosknrf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ujtvwrad.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3fessnidq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lvkdfhuv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3jynzrwpf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3yuybkpyo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zazbrysu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ppnuwwsj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3zpzvqods.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3dzckayai.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3uockrqxo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ucgvtjbt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3sxppnxky.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3sugqzhjx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3nmxpumqf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3bjzxbjtt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3snorompi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zwaldrvs.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3bmeozxkf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3mwcqzrsw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pzfssigt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ifenkoxo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3umzutzrw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mgkbaogf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3apqcvhcv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ispaxpze.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ghqugsig.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cbpgxcik.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3adhqcmik.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3psvwrlev.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fztnyvhq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obfxkqcc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3titwjdoe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mumhlyzj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fskulfig.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnicyojn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uaqaefpw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wwtslgio.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zzqxgsyg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3yehvlvly.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3asznsshm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lwlzkngu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uinaklki.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mlqsayul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmpskiud.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tsilokuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guajzyah.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yjwqyuyq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zdchiugt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3stlohwal.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uqfootui.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ubasmkzs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jbgxvxpf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xpqnbeym.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3esphudtv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3msxannlm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gftyuwkl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3sovncxwl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3orrwevmq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wepxcpyq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ajtrobol.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zkkizdap.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3furdaxgt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bbcaudap.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wdqmucip.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3gnucnyxt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3rflsxkvp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3luvfkzar.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hrzzjnvc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3erncjbkh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pkmbdyba.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cjmlodnx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dhgokvbp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3htegvzbp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3forpjmsq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3tjnvrqec.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3egzlpniu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vwjywzax.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rkoyeczf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3pvhgngtn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xfognejh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ltidndvh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3sfhzyccg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3lzdlzhlb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3yhovqcsg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bqkamnud.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3svjsuflp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gcquafsg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jvrpxwbo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vxxbylwo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zjnptknu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xkojtvou.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3osdqmkpm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cgehbuei.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gxcxwyfn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dvjenklt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bwinljxi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3doksysru.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tnfxobfv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3upyhliey.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dbgubrzo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rpdqqmgm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ynqjmmdp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3fsgpsopo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3vfyclqjp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vhbkpvnp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kckshqso.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3afkojtmb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3emoabvpv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ftnuzkwl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ywxvlhbs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3asatkaza.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygorietd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3drlaudmu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3inhicjev.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kbnsmihs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pfafjajr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ilamikym.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rfjokmwe.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3twhsjjlh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ennqajzc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kpfnxsvc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qqhhroqs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljlejwst.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntmcnddy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jaaczupt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3uiaactor.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wystpqpq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xfuoeyhd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ekfwmigc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jczgnorv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ffeaqhzj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bfsdhwer.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vnzwthrk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3afkoiyby.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3prvxokym.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3hqpzicbe.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vnfwupln.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3henlgykj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nwxcemhf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aptirigd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ndgxtdbi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3veexfdsn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zzubfsod.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zqgpydwx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rtwchupm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qkecozws.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3qnxziuiz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jzywexta.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3yfoylwlt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zpwrajav.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jtmyxpkc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3bwieoboy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3rnvinogc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vljhvkta.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3sucxrdjh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kzqugucr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sgyvpsuf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cpxpivwg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sxhayzbw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dnflhgrd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gjxzeqqa.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eeyaubkf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kfywbvkl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jncfwgua.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3epvjanja.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nipxgyyx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pvyqwbto.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dsakxcvs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3naskhkmm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jvdkaqqy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tpoxhenk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3emykxkxv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3bvmyfutb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cutrkrml.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3guvbxzqr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rorjxers.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rbpifkpj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3olhskyoa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3wktinpfk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pwlexwoa.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3omqndhid.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3mjsmonzn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3jbrzaeka.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ensbuvfq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qohbqhiy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ipzolerl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3liwproeg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3wjrrcutf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rbqlltpk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hopzkspq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3nbrbizca.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ndrmqrxl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwrtlzzk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqzdwoxj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ppanupdm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ojsndtck.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zihsiugz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3evxbhrve.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qoziicyl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3mlreteyj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jpesscpp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3avpegxne.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qeghiemm.html


<!-- 参考信息 -->