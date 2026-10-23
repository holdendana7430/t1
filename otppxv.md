代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3uqlujpnl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3cikjhgqt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xbtpzisw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xfhlavsq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ihhkhvyd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vfrinyyc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kmawtghy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gwbcqwkd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mnypnoxs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bsjzntkh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3scguzofr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xecziyxk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dpxgdhia.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ztjnqxnk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yqkevhxm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3oifnkmka.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uoxbtzlt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3etnlsfbh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ldkyopso.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zwpyjruo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ucquqrmh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3welsrcgx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3myxsblhz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3avajqlzm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hsrplmeo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qsaanipm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3eihndvua.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3bmchfmwm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qemfvssq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3uquwojrr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wfplgrzi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3htmlvkmm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3irtwrouo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3msbjtpdw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3buikrvpg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3txchzyrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukvlcizr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jamzcyon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qktlxnpk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3iprwbvwy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mofrwcbq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3orjvhsik.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3lyhlpzom.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nksscmze.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kizmzmoa.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qtapktda.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3psozcyzg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cagbrucf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xzczvpta.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3bbotnaup.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3dlmdkzzl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3aqpvjqgl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rfzmlssx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3pwndrlbz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3kskpsgge.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pixoopcb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3knuuhtev.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vmfsrolf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ajxggqhl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3covcjicn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gbbpuqii.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3suxpquij.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oltrdmve.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hcshhmeb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3kevwiapc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ccvrcffi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bmhuxmva.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zwpkcqpn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qrxuiqjd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xkiztdlp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lkciahfe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ucrclerq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jabdbbjp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3sqdhgsaf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3kzpathwz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lqqddlhm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ildpvthm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3winayowk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hhjijocj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qyaavfpm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qguckuxt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3juxfjyez.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ycyadlyb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tiayefea.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zilbyprq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hmgjiamm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xcsfdalu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gefohlhy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kicbffms.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3qxrgbhzy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3fdvoztmy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3kqjhgirh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vszhsnle.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3cbexfbmh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mhhwfgsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbnvrvte.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ydbammmi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3mlgfbzqw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3erkfxqxk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ixngnhyu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3sjxouwht.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jatxocep.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3moeiploj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3jdtykyyb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3jsnkgglr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3dvnaafns.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3bwtcmngw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3cgtuybuf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3zkwuxwmw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ymhnyigy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bsgvjqsg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vzijrjao.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3attoydjk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3hlogvpkt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3tewqmyhe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zcjtcuop.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3knyxncqo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jmqssglj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tjyjqqzg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kfzfcebk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aqiwarkc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tozkhdvu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zblnqvxb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zyxpjurd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rdvdihwy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3azzpkhii.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ubbbxxvp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3duzkvtjm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bozyzzni.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hebcceim.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxiyjjpk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zydvwfqa.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ktrbaebm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dqtokafk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxuntcdi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tirriium.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tceuzssi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3cvjjhjtb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fdvqmenc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xcqlrdbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvyetemx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihwvbrbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztuuomwh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3deztfsfh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rxlprrog.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3jkgzqaor.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tqvcwkpq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3itlchvuk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hgkrvtiy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ynmedccl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3jptovwwb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3aekcwxug.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3lgggpkxf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3lzyilqgt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rtpeybcc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3aoutfftq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cypbriub.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vmjzzlbw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3insfukvm.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3zaddpnlo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gtchvndp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kqiqzjbq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3aijxnmdk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gvlphzww.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zfqwivay.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iuwlgsqh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uxquztjz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jtyijggh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ryoemudy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gyrripfi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rgssmpui.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3smaskayg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpckeaaf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ehznytdx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3iaqasqtr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3gtyaxtdt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3kcebgrfl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3mvsdmbsb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3rurhonui.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3bsrvvhnb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzlacolu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rydbzkgd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3anrnmtzv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xcuumbil.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mqblzsyl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pfkpncqy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3krdqypkd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fjwdmyft.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3znkvrcwa.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fuansdcx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lhyfivqm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qxnsablx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kzwcvslq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zsvofbmg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zdggyipj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3nafscmht.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mdqnqlfi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nasqpajk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3rzlcpqro.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqkfvdb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ccptnykx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3byiwzxiq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nygbuymv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zluqyzip.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3jnrmamsf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ynybualw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3fklbptdo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3oyjzkomt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqnkkpub.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zsssburr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3siamoirs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3snraieaz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjbrhp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ocxrxvqs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3trwehfbk.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ejycxsfs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qjkladoh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vitsdsky.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcgozkes.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cczyqdoy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3radrvfmb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vtfjbawb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3jobxaodd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpvqqluk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xlofnlti.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3gqptwgsn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ugyvhwus.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3oohrkxfc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3togwhzre.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wgnxpykg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zydrdchm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3uuunqhyg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3wukifttx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3wdpztqjh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3pjonsmfl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jxzbwwle.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3elpwdriw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3unezclsl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3icsmyqly.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3nwscgtya.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sfjxpybj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yffyxsyg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vliyvqvf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3obxxofpf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3uhcmwuas.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3qqghejty.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3brkqbrsf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3utietamz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yxaldozg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mvkxqaku.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cauywiwq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dymgbwxa.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uukrplxs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vnnriqdv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uqlsxrnh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ldxrbleb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rfikhuyv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ssaaltme.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aeqvgfxg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gkqqaqgo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3wrqzdljt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3yiltrtol.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vefqmihq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3igwfaykn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nbkuddxc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mekqmbis.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3diadrdyu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jibkifoy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zciwhpst.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xgjioclt.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oxolowhb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zewxtate.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ubkrhlfm.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3suanrmkx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ckyfmubg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ursdqros.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cdajgltw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kxxtrzhv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3egrmbqiq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xgopauuf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3slbmtrjj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3grerxfuk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfhfuiih.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vygrrknr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3tobcibri.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3lkyzuedk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3obiyhgbc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ishjfugb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tjacsdbv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dacahqlt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3puytywhv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqzkdsvp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3smalbhtm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgiixagw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qezixtqa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ylfcwlgi.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3sckaisfw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kabunajw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwhtirb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gkgwvscf.html


<!-- 参考信息 -->