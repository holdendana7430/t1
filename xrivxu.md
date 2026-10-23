代发 wailian999

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rhnhrsmv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vfuakhtg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tkyvujcy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lnrrlvpi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3uqxtexhc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3iywqhziy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uzeyujzb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3vfugpvdy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cibvvoio.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wygqsebc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3eulbbmog.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3hbtcbbos.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lsqibvop.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvwoxzp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tthfianl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gbxzidbc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gonwoifv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kkubjxbr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3lewdtchl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3npgzyicn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3cklnrymo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tfvpqoky.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gqpaulez.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xnvbwwdd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wgnesdvc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wnwdegdf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3uwgegwcm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3wkbvtiem.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3upuusrxy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ngpsrfmc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xadvyhdw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3omjhmyqs.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dxodflxp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kitkooip.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ehnlhpli.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3eacvqqto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzvvtlvo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3onkgrbhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctzdadjm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3uyopccjj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3uzqufosw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ryollyru.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nmkpgqga.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3spnuzhky.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3eadcbyzu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hfctqxbm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vcicvomq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3uufchgdo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3mnttfvqw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3xkeprthh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3iumyydly.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ccboawla.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lzhptscf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vqpwyzvp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3gybrosce.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3kypviaks.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kvounbir.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kapnsjdq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3inagogos.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3mbdodcbw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zvyaxzfz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rceozlct.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kxskqjei.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3japbyfbr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3vgqifjzn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vxgbljbq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3orxfwqdt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mgdxlzvz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3asbylumg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uyjtrgwf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3srsedzjy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yelonphg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qxtdwlfh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3janifmki.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3yhiwyxut.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wiphibke.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ntaktmdn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3isjbuerw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3euwcgsiy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nmzvtman.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3pagaphkn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nrusnxno.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3oeibrsdk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ohzdbyoz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pjbwfzqe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bbcxrfaw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3hqbpvlel.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fuomcwoi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3wmcxugrn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3wffkklhu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3pmirzpam.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3prvncfts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkybshxc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ltatgmlz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lmxjychc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siokwpem.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3osgaypbt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3fhxfhzsk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3uplqpgoc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3nyeqgvzh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xxhukmfy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3bhhzwlhb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3olowsbwk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ixjruhkk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3nrvapfwu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3sozipqkx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3nmizkabj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ahzdrbvb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3cnpitvdn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3wffstksf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3lognioqb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ygovwpgv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xcdpiihm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3spzixawp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3bcudalqu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3cwnntkbm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rictmbvg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3wtoffooq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qojnwthl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tamrceth.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rhzfxasj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3keidjqth.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3krtexanw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ctrtyvgh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nbfhfttk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zfxgmuea.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dqiyfbxx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hloqajpi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ydhaxwgw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tihunjfq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ssxarrtw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tmmaleir.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kxjgnmvk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3womtplid.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wuauldos.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uydqtkdc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bbphbqjc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3tfuywosj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qmnpznys.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfwujuwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfiywxls.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3yycvkciw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmocctmf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bfkeruct.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lnhheift.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ojqzqehx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3favzqgok.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3lcislkwl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bwvbxmvr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tamtskos.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3vvgwribd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ukahtdtk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3bjbbnabl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3jllehiwn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sejydlnl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vvgtwzsn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nfanhmfr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tgdnthga.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3akktvzyb.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ziswwbie.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rloafczc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3oykpblne.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3aqkmsucr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ojrqdptw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kjegeafu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mvacdwhv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xljesjpl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xfsfytvq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nbrpkqak.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3woqzsuhw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3auvsrvko.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3aeiemfsv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtleiprw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3oybgroqs.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3omfpavol.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3trtsxofh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3wmffhbmr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3wyatjapc.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3tufbuvbz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zqrzabgu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3jnzakvcf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ohijthyi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fgslqdcw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jtdphdyu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dqmpbazj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3svhaldhy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hkdxkbhw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zourlufq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tlvltwug.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ylvcoqnn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3endmtegl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fpcfecqj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dhypgebv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wasecnai.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3rrczcsxc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3hcaahgcp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sjwnvhyk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3txfwbxyk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3wyevcwca.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3dvmveenw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ukwyaluw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkjzmjq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ixxigews.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bjowigie.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3yesyazts.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3avwqanmv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3npoixjix.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xjuttrsj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlrxwrcn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gzughyba.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3oqmiueft.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fzctdkpc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3txyguszr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3nwltklfm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hcgqcxfg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qlohbgui.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3veliwlid.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oeviobcz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmtmrkng.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hsmuvygk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tptgmlhe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3vyvaqqrp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3mffbmymu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuzlrvon.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hnwgkwlg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzrkdit.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3xfzpddwg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3olmqxafx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjywgjwf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ffhgewiy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3podtemow.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3takuupkq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3yrxsrmqw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3cviwygem.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ypfdrlfp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qztkjsms.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gwmionrb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kuxshmve.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3icwqptlf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3vvexiwbw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ozpkbqwg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ovbhymyr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ebxunxyi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3acjzgtxv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3djqmpglq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fiyzpqws.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wvptstzv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3chbkarxz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wwpqdpyz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3pwwptxoe.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3mcyfgxbg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3bxtxuefx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hzcgvcfs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3flcuqlhe.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hnjahpat.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jbwalezs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3drvmeouj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uvqkvtod.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pxnwthti.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3azzcglzz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3esnoqpvn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mgwqwttd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vhyqaeva.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pkoxhckz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pobyrgiq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3aayhzkir.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zbkhbhon.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3akcwiiiw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cbogohti.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3hdgkstjn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3onbxdpol.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xpurieli.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eeqhnmpe.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jvjajajm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3zrznhglu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3srxhjrfd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jmtizkmq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ahakkwza.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3mhzbbann.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3alotvcet.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3bcykgbwj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jfzjukop.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3sljexsrc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3xpmgdqld.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3lqkxoupk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3jpdlkait.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mdxhziun.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3wsazvfml.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rssnmkek.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3messwkbp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vqcyrqpx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3owmzhuhl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjpsmywm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jrydztoh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xwuyphis.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pprqvjwx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3azyaeryu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xjtoqjnz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rforatkh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3guukgdza.html


<!-- 参考信息 -->