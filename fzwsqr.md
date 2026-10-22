代发 wailian999

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2iytyiiwr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2juwwodkz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cbdgxiis.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2nccqlavm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ahstboje.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jcfjuroq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hwhminmc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rpjvzzka.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bwjxpwpw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bjwnhhhz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rsocfrdn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jpgwnhox.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rycsxwwd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xrjmhdjv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ggyyvhex.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2tukemgne.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fdkexnwn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lpwmkoyn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2zlcxhrsd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ptamyeqm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2votzheno.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xzcafmoh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bhwaozpg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rwsqyilp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gvstqbhq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jyixweas.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2huqotvqf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tdqamsne.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ndeltcwn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2royunpsy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fhovfqed.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ghajchic.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2celhgzlc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ahzsuety.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zwcfxxkg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lvjjmgph.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tucnikbq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2etavraen.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vmmxsuzp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2robzruxd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2sqpzmixo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sysirdvc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jubbdhmy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2acpnukky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daxaphfh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qbwbonqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsgmoafy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wbxlxuzp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cgywcilr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jrnozleo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2oniqdytz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2taohghue.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dtivtdue.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zfeywjuv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lwftxugq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xqkpgeai.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2gebsxmjx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2acnjmnzl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jmnlqdxd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hxfrdbyl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jupjvpgd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dzknugid.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xdaipunp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2duxmivkv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ggnnyunw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2giwoageq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vtgwjven.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hecpolzh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lascfszx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hftkxdzb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bhjdzggw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xbsvumja.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2mntpodqo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2fimtslxw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ogqkycfp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kazykwtw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2klcebnom.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gpzviipy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jctgywtd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ncfrqgnq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2leexuiee.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2stdjrdgr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2foyrverz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2roewxpzv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vckmgqzj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lwgmiarg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hnjgfpzk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qdeocdir.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2iouccoua.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2chqxwbkr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2cmdpiauq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tcvyjysg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2cuohzncv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2amraezbb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2snbcmnzj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2uaqxzzgq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dvyvwqbt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2fksudwmy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2pwiiobmx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2rhulspet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcgbdgxq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2edlxafwr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ynianvia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrqlsptc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2plcsfdlh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vaujhqpa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2wdwiscvp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qgocdxyg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2amybzssn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pohmvlvb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2hljxwauz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2jjdnjnbt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2buaigsnq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2yaotlplq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2pkpxjxyq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2olszubzq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jhiqkhpr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qgudvupp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yqsrtudd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2thrqdvwj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2iiimmieo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2vowwdeea.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zmefrzcq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2csjbsvya.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lwostrog.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2hqpefwvy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vbajqbuj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xiodblbd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ahpxzias.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2imntwlyz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lkwkskpa.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2wyothxuc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kysnmbwd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2skekljwf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zpjqghed.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2optdzgvh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2owuibdgv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rmjfllpk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2amgfiyzg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eouktmei.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2izrirtdj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2owvnbwva.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iwvugugr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vnpxyazn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kpgbebyf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ebaevvqy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ikzcqrds.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfmgvnpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvctbvsw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2khbbeeyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrmqizgi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2asvdjgdc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wdgdgjqj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2cedhzagq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2loxmrina.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2czfdvrmk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2exwrwkfx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fxyeiwss.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zwgwwcsk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bfxljwoj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2fnpkwgff.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ymxnirmr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gpcjgbvy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ywqjrhhl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2obxvcuod.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kgypkwru.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qvvjkjam.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ehmpkvlc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xihlkrps.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2rbheadnx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2lhmoewap.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2idqipqdj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dcxclvor.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xrllpdxe.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xftlhoxq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2trvfaetr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2osctjiuk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ssporxww.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2zaftuqzs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2slvhcocu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2erlhshsx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2morfsrjy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kcfcwqtv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2xtjxhrlj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2dsdjyhkn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2wzpuqtat.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bfkxtxvp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2vvjskhpy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2cuqufaea.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dmfqlguo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2djgscfsm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2llpufcbc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zpnhptpw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oefkiarm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dzspndkh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xmxxphux.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dkexihfd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pzzienru.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zgffvgmj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fuhkxdqh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kxrftwlt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gyitdnjx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2rfohkgxy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2aivothft.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2eeudtkds.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2suvjcnoj.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2suxetslx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2xxuwimke.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2bxutsvkl.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wznqwclx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bszqjyzv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pkasdimj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vqixyagt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2utytxfnv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2wzxtvspn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sveqfhxa.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ojnhzhpv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iaujrpnv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ipnyfryc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kxjdpscm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pmdsacqy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2awwddjmu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bxwiyljs.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vwtuvnsx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ogjqxech.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2luhztpfq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tyiutfsy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ftlngwmj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2taguermd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2zvvtzelk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gbzpywph.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gxtstlbd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2kdhlqooh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2txjwfkrp.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2oovtjybp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sbukqwcj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2znwiujzu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2boilrdty.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2svyfyefb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dvupyovj.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2rboirkrz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2fjscwzsc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2umxwhztz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2acrceusn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wxdcrtgn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nsychtba.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wgvkopii.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2bkatnrqt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wpxyyfwm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yhraubmg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hndfarmm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bqxipkoo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2yaxaiiwa.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qgmagvgb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tfqzumay.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rspvvdud.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2khceaxny.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2fiwnkiys.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tuphlxmi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jlkiawrt.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kzihhmqg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ybbdtwfo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jhqxyjck.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fgmtvxae.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aluqwsaw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mdgrhavt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2knmtbyqz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xmabsszf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hsiexusa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2thkpfnam.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sbhkvqlv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ztbixmmj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2shkwihaf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vsauaatf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nqouldfv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mjxhrrfm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kgcewznh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mdiurwic.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hrmldaje.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ltkxlajw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vlhzopbb.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ufpekuyl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ncaihhcy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2tijodjmc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2emzebutv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jiuzfbup.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ygkuajip.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ztobnwpc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kfyzzqul.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fwsgjegh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2gpjghctc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmevlgpe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rpvocipu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2exwxobaz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jqvpmuxp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2qnflnkal.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nckmygci.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gtmsdjve.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tsjwzxth.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cuvswidc.html


<!-- 参考信息 -->