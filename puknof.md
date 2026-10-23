代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ggyxaffa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rzutcahq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hexoiozl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nmimdbvm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yfhpekds.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mnmtmppm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fzeljtdt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lcesaivf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3speqswri.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzuknys.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3elebbxoc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nhsxbycl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3okovyioh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qztddcin.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ldgybdhj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nqcaqxqy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vrubplxa.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lpcghrjs.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jlvdgmcy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3eyqkbtcr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vucddysy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jmmbkwey.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3kmjrsbmp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3tucywavp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fvakgufc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3viowhmdt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ysrzbkmb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sasjyyvo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xcvaphse.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qemhzthn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3vtrjajmm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3edgchcvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bltkjvgb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ljwwcrhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whjvteqo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wbscjmqu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dkjqjbss.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lvleyiyi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gsajpfar.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3igciujgn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3evjdvskv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ywtzdulo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dntxnkth.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3edgchlor.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pfaiciub.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zidsgzth.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3bwwvaurx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vinmztkd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ifjkvwbd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3albagfpd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3yxhapyou.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3avalgxia.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3utwgkbmi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bluapigf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ghjerhno.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3hamfqbhv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wahkbrai.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3guiacgkp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lmpkdxox.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lgzuxmxt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3kyfmrnxj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mxprfpcf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tkqdnjgz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tmuhvrel.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pprnfrvf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tasncxfh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fpnzfkpj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nkesyvcw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lnyrweji.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3beufymml.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3iaaxywnd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3opzmnabo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3qaxenwkq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nbvzbnzm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3uuyufdoy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xzgixggj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3bscoeqin.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wzqacaup.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gannncvt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hiyongkk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xrnilavy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ijibbyuj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gmwrsjyv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3posovbni.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3kcnuekjk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vmskxiwl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ginvypip.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3hbkplake.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dybbifia.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3koddfqti.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ofjvogph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukhwfemb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3hftcukrg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3epzeadkm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3iaskscde.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3asparnep.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3icgozeyv.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qjmwbjtt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3gvaaxkox.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hhvnlkls.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vtaofepm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3dlwylqyk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3tyjnfohn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3hoiwzbna.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3kergidoq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3jpatsptg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3wttpqwif.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gulubhyi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3uzczdfka.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3cjsypoyy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3lvlycira.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3wztuyfqb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jzjvgzku.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lpgirlos.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xvkkzoyj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tampxayo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lwvprrij.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kclkpvwn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3seshjtwf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgqkumlz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ttjadcfq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jaxkgiem.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzgoryen.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3brbmdqtf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgmkvypi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfxbcrfk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zhxrnijs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uwtkfbgy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3juqtgudy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3iidobifr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dluqaczb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fxkcggzr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qoemqtaj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hmrylkia.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3abfznecz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fuosddwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uufmklcd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rrekotjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gibtgtqq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3sglvoldo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fifppdxd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gwcuwdgi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3figcnreq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3edwbcnxq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qvuuchny.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zlzxbrbo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3nemxrzbn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3heyyhcdz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3tbeesdzh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qqbawwis.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tknuzitv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ylysguia.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ywfdfjfu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pihiyeum.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3pgoygztr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vxdkvnex.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lwmqjwld.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yaayevhe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3krpuewlo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3excxhwzc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yynvwlxu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kgmlgiot.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jxfcfckb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jbinccnn.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3chdksskx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cmpoiqgt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3uoeizxiz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3iqtohjok.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3unwrkdco.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3oulgsocv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nlwzdqxu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3gnwuauiq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3kekyzybm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jktbfayh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3gxengozj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3hzipuois.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3bpueiuai.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3udhiycao.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pxwkhrco.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bxpmkkdr.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qopxbxyw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gkuhuxge.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kvwujqlp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lustdirk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3cuheeqii.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fkvpzolo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dnpgllll.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3argheecf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cyifuejk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bqxekdtz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3fqkqwwkh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zfppkeji.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dttlzomb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3drwklbpz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ezqemxji.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvbyhfa.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vjcqugnp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mqoeeaqy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nxitsndq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cvfkfxoq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3sbkimihm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fykbobii.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ngagsjle.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cfnswewz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ylqmqtab.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zpyrqwlf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3raxvafdk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jbxwyfqq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ppjbhjlk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vzmzfpef.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dvikktqr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mtjkovjv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecbafrwe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdfmpkqj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bgiurhsl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ceecblru.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aylrxtyr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3puhgtoqq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3jslpdvjo.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jesmacge.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ztvjmiue.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3jwfvesrd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3hfvznxbx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hpbpipql.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3iegetfim.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ngawpjpb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3yqfcuaop.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3xsndfesl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3cfltuudv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3zqdulwll.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xtilcttv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gzmhgcit.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xhmrapbz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kuxxrfkn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zzuwerlf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3pctriswv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nsdrexci.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3khsqdqvu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3kuslxofv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3fvtahgfj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3fcvsegej.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3eytuspxq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ehqoskte.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vqgtufdq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kicqfanv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yvwlffqh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ifshhhdc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mcygnxcb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3btdmyjfm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cjsqtpfa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3whzyhsjf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3idmclnkb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xeundgiy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cghnbvba.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eixwwwvo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3soaqeupm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hodxamld.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3hjheevmd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zluhjmyu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ogagrlcd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jcicrvug.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dohozfgq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lstktdni.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3esycfflp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fxbbdwau.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3zpxilujt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zlxgwirr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lvvypvln.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wfmydvez.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qsamarii.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ctlwwcvg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hckgyyss.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jvcwrdxo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eohzldzj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3qkwxotpg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3djsfkzlb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rwqhhisr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3tkublkvu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3qujekbxv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjzujjop.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3hxsndxre.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3mqwlwxyp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kstlnnjv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vlsopups.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ytpeoiej.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oerybrsu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kcqjjbqr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dvpnqnxw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iegnqkib.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eldnyevl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fgdvjeaq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lgeribss.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3lxzctizs.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fikymyjp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbrckuo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lapbgzpr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jnobetlr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3cqdoapan.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xkfchdoe.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tzcdycwd.html


<!-- 参考信息 -->