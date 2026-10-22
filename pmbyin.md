代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2zwviuxui.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lsaiieae.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xqyqmybc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2tcvxhbsc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lsvvthro.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2aykgtksa.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2sjtshzse.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2urutysjm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2crbygbss.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dqmjlyxv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wymprnqr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2aysfkxbt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zdonncxg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mtenlnnv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wzrscxdi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zvsocjag.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mobxtpeq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfowcdg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mydganiy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xcocohjb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tvmxmpsi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2latucfjk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lfbibfth.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lqzzibms.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2haekagiu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ovsdqrrw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yhbiyfba.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnyqpwx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gimohnld.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uhsanfse.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gggqwezn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssrjvbov.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hycjuvll.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2nipswrho.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tvzylyyk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ykinzyaj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2mkijnxrw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xozwjmmu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zefeqgak.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2edieqcmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owwqhiuq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2txhhfqko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oakphyjy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xssbmeyb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bxpbdfem.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ytcrunoj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xmuyucjv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rymrcjtp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vvnylbql.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ziktguwj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jnzfwfkh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cqxlbelz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2aqrtleao.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2bypnegdh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xzwfqyfn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2oprlpiqh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jcnmhazr.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rgxwjvzw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2oynvxscv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2yuhmlmir.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2rjlrqmlq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sbhogamc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2fgbwhgvl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2evmxcvey.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qsaoilrz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ggjrnfrn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bypbvvwq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2orjpymqb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ejtsniqg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kmhgteef.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2erfoiefg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2aqoahfpb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nwdujabj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qjjttjlb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kofrkoym.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2plnuopvb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zyrvxtux.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wxwdfklr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xeextmom.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2huuhrlmh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lszumpqm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hmheyjwa.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fgunfwwu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2frfqndxh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2lpkwxges.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gysydugl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tgctgdyj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wbrocfud.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2oeskvczm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2grjqntsk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2osubixmb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ipkbwyor.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2rbppuxdn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ldyxvcxy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2phwocmgu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2eszcauxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktzwbdfl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2dqnzvyss.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2csiwynmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzumbkht.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2qboqmdwc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uaulnmvv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2umaytyee.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2uwlfpiqe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zslvdxnn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2acapkatg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2yyocckjf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2xnyaytbv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zaexzpjt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wpbjztwb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2hpxkrmsy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2rfkburqg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xggscthl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2boorzdzi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mgpymteg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bavrzqox.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2folpbhuq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2piialitm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2uovvqmtr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2uxyrkifn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sjfbmmwx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cnizzaaz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2plkktqwg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvbgfqoy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2icgqcatz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ditpmkwu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zdkvoxxo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2umgtrgov.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yfekelvl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mcyspkls.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfguntbf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mwhnnomg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lqsnnfja.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2irwbvcla.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gzbjgdub.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lkbgusyq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qezpkdjt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2owetukwz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xosjwjne.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gcsszisn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ebpmrxbn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2kboslfzv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xkkgamss.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2redtheiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2burvffyb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2bdrbhjdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzyaybwv.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2hzdycwmd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vxnlmwtb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2eqwannpd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cmxyuiwp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2daprrehs.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pexpttfk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pezfvncy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vyzwnfen.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2anvgpnyh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lgoibmvd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wfwfwjcl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qnxozgxx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cmxqbxoc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2zsllfphk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vbtyzcfz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2egamkeoj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2bxyicfmc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sagbcjye.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2rkhlpasa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2umoyichk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ivnamfnm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iwvhrtlh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yvvmfycs.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xufobenp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xcrwbdbv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2grvvtqvn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bsaczxgs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ajwqetsk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2gylezwvn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdrigoph.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yzvyckfz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kitqhhrl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2rkanniyl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2cogtlhfq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bdbudrat.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2uxsvhanr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2logvjyte.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xxcbegts.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gkubmnlv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bfwvezfr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ufmiwyxv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ytpvqadg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2usomizeh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yuadgths.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pqcdwtgu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pxematkg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zwflsjau.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2qljaqkii.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2vfzkspyy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2tvrzzvqj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2necnuqzb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eojrisyi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2geylghyn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hkmjauxg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2csqnclai.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ghpbecsy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrepkoe.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nsdtcftt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdnxmvt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uamthhdg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2gwtcbpkf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ktecbwbu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2fhcshkvu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pvnumqpq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbrlvbj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ppxjvrdq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2htvbytsn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wcsbeywa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vvurdlgb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2waqjxdwy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2saqzqybv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2goghtrrd.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2faeflfyl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivsrraze.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrdyruyr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmipbqbh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2azylxzpe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwusghg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2skfrxota.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2fnijtxnd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhyvlfzz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yncfhzam.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2cwsdypda.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2avopgwdy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ezlsxara.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nhmsrhse.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vackxzns.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ykidnzds.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2fpboxffw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2htnwzhgp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2rtdftowi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2acptywee.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qnakqwgm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vfpxsbsd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2livnpceo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vcewzdli.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2fudvxrwr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uhtyqjkg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2egvgdrfs.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fzuwaofn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zyijyvlm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2wtyszaie.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zsgzqded.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2niddjpsa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2hjygvilo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ryijzuzy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gitubzmp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qqdkndsa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2obgoxrae.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qpihknjf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fdegiazj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fjhrzxvp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vxrwzctp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lmsdthrr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2abtpncon.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2congomzj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nytjjdvq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2csjydqix.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2accvaxlb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2feqsgerq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2icymgijv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ioubkgtd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2mhpclohs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qeokazkw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ukovgpeo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fnuutrjs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ouwibzuw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sbomohdx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tpkclslf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2somyknhy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ynntyboq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tpvyzole.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2igkkuzwa.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cxqsmcrg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bfnkyqlb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2bpdznsvd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vfvhcetx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2zsbktsej.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2csbscrxc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isomsblh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2oagiledu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rjfewaxx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2qkqordys.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sxeyiqen.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2htcyhjeh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oewtyrjf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eriwsgau.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhfptddz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xwkxupbq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lfpxesjk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qksndcqh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ztlkxciq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kackbmuu.html


<!-- 参考信息 -->