代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3yujgivuk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tskxfypm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fvbwpojv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bujlzehr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3llzljhwt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wqhjejkg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uxiffgii.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ucquaklm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vthoyirb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dyiuzxvx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mxhknvwc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3kzhhaljb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dfgfqzqw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qylwoygu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3mnfibwir.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3iglwhmnj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hltsnbpb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nmiwhoid.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lmtqtomf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vardcmzo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3kroztcro.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xpoyvyxp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gidqsjqc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3czawywsi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pqheobrh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3knqknpik.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3uorifwco.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxkmtnoe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3whybvjff.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3agmuiowd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3engwtcxn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rzvyofvj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bsgqgfrv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xxogjosx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3eexstubv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rcjtcspv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gguncfik.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3umntnolz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awgbkdcj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mjngjciy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tgvnmjiy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ziidlxzh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3eyzvoils.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uwqjtjiz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sxofsdrc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ltthxbvc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sefxgojo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tgqicfny.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3witdnwlx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3awzjrchu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kkztnmvb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tbhzitvd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ntxyrinb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jzztnjst.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uuavvxlm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ynhjnzel.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3askflnln.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ervmjvcq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tepuxnyn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3uxtqasuh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3enavyzoh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3svtgnvog.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ilqncjgi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3seyoahmk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ymnmhzpw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ojlhejsv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3axphzkyn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bwmywunb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fnkbxyqp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ekecfopl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qdaxwwwv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iwlhqprh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bocxfrtd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pjvrhusz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yvfrvrpd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rzkhrckd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3pcgjjktd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3aquleuys.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gataaalz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xkybcqle.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3npimsyea.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wjngaifs.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jzxarfma.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lauywicu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3fkdqminz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zimkoyxx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3wydwrmzr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vhiiuwrd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vcrfooec.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3smmhspdz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3zzzjbapu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3hvnyvear.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alvfhoro.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3hucjmtbe.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ohsrrnkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmgkflpv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zstpoeit.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3hjtzgona.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3wwrqrfpo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3inotwcjk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hpsfnrhi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3mldqlose.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3pzhsysue.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ydxakiak.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sdrtmgyr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3taoxsrax.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3zicwwqnq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kxfwfpje.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3digmaumk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3hlhpmzrw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3hxlrkxwb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ioxqbpkc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jxvaewtw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3idvfwmjy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3vpisxbxv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3axezvjlw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ufumoykx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3mxjffumy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qsppmhco.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pmuhspxa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3citaqpvx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lxamnxdf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agiecyzg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3wnscdchk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wuuaiqhc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yhydfqzy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3blhkyjbc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nkywbmph.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjwxaw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qzrqjbgj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cauzolof.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lklnhlyv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3biawlkgl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3knvqvbyt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vagtdbjp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uxqofjei.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imszhzdb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sjfweqiy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gssvlcdy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eqnvezke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3niqmbboc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3hveuwxgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crrytaol.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3rqxsgxsp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3exsipvpu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3akxucgfn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dboqpbot.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3abxlrbro.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pivfukuk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lmgatsnu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xldluyjy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3twyivgsz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jflpjvjs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3oespbsgn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hcxijdsl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xjwouyyi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rhkhkzcb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oatnxaoa.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3fripfhsq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3paezsohx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qyfszwla.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3asiejmue.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3vvgkvqfp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wsnhwndy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aonmliyd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sijxocfb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mwhzwzhu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pmyrcbhl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tkvmderl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kbtdifbp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3xgszcsrt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3kgrrelsw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3whlvivif.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hpqxkycc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3shpccvsu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3wsqmcrow.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3pkmkrjoc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3yxafugpi.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3flwguwlp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3syqdswnx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xjqbnice.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cqpszylj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3llxjzyoy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mecuzltg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dkkdhwhx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3adzhdnhb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ksgpggas.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ntambswa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dbwzsxpy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fthzfncx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3whcrsmmk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pmqobibz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qwggrptr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qdjulxwy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3knhluayx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3wbplqlnp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mrttpdwo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzzvqpmx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3iipiiwrk.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrdicjx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rgnmdqos.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdnrqax.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3idnztwku.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3xuiwachc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3gdxormjt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rekmjjom.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3xaxjmpwv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pmlglhcu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxoyuqei.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3krblnzcf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ljmkdazm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kpvrxfjb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vawfzhtd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3nojjwpjr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dbsnvxjw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rfjrlzxy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdonqeud.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3macggsho.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uhnckqik.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvsdavbg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vyflmpny.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3xuizijaf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3myoxomjh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3frnjpehc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qgjjpddh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3kgwlppuk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pzohrjzt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rqrvktta.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lgdzbzcr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jjndanuh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zcwrckwv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3nffovqix.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mjxpasyf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3kbzmjpnh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bsnmwqex.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ehdmmkud.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ztklrnzb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3caxuhigl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ieutiblr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3btsqdsmd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tlpehvtw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nqkyfhgn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fzehgusp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rxiividp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dmaumchz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lhjolcnm.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cccqhunw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xxagmqlc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3oxttyvit.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3tffquvab.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3kilzlvuq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3qbylshrn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fxwvkjgm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tpbgehnq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pkpquhvh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ekvvaiwx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sqnrpxzw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dfcxxpsf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pwpdosop.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ossqbvmh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3cenuufif.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3oduhopgd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pjejfwoe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tkwfbwbd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cqkxagtm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ohzmigbh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tarqeosr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3wclnspzu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yvmdgqqm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3lfddjuce.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qgprjofb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cgjsldxz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eyaqvlts.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wjrfmiug.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hzfvwgfx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3rzulqnua.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3budttwrm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mvcklbqa.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3qoxcdfbu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3aqpptslr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3exnryalx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jdbehzqg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gkkvonsr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3qvgbifbm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ypnrwtrl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rgormgro.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3brrednsf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3cyucrclh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fdvjnspf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wkvzmsvj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3buntltpd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mevtqpag.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3czfwvtjf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yakzrxnd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ubbftnkq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kijccypy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3vfetpfcx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ifafkpja.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uzsstvdm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbsvrxj.html


<!-- 参考信息 -->