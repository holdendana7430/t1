代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ikafqyhd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ljmvdirb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bldsmfsd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2rdjcszxe.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vvdbhamb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hbgqofdd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2emtqdpxf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kcpjhaxr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2bxwwzvrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rjmlxxmx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zghjstar.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2tffmbehk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kaqzswht.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cpvoilem.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lsrzsalz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2shocoozc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xwjvogxd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ehxanqdz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ptroutuk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2guvclzfo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rpfukibb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vmmaembp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xdhkqdxw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iamzwiko.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2efwwcsaj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uudzlobu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2scxioxny.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eavccpyc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ajlzvlgc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ccknuqpp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2giffgyth.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2eeatrcff.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2iximpdwr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2eefpxsxq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2yvfgyqmv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wnjrnoez.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xfofshfj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ddtgyxrn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2povvoqkp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2tcrcquec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odcnwrfq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dqnpqjgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guuyofok.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ejtnpbnw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gsfdggeh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2vxvjirrg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cncjjsme.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2urakddmg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ltnbuuda.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qimjrsle.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kntqjevk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rcgevqvj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2rrgkcups.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ebcnoyye.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dldqedfi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2eqxcvyey.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2xxdmekhu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yrfpwqbw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2yamviggn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gzmjbbxl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bqntqkfg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tpyizgbr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rqvihbgb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gjizkndu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ekkarcbk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mvxcalkc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zvipnrld.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yamykhel.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qnnwoiji.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mfoftwge.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jsryalbz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yvgfxctu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jcazpwkn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2krqsvehs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wssotvwr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eexdbems.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2szqvuukj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oxrpjhoa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2awaxdtzy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bkdwbknh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rzcodbsd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vabrjzze.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gjspluzt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rccotxgx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mptndkeh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mtxqrxae.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2csepkyzh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zjdflgba.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qqrrdaps.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fanorwwo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2atgfipzy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2chasxqji.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fbpyktaw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2omtxwybj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ekaumjxq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hdayemvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqyhgcwy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qyfvlllm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2zpsylpam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzuqobrv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2nttkmsuq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ladceles.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ahpezcyk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2sxuxeqpb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ijwlzclk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2wnrkpzfq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2vtfegozf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2dqmoplwv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wqhoviom.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2czajwlkq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2kreozhqu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2feiggjbg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ygzzgojh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2xhjgmmdx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2clzzzpnv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2irjnurgo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ajvuevbf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ouazqlga.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mugsaslx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2fnrspauj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ucurmbyz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2dhkllpzh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nvnwqnuw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gmmvceak.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sprkcfmg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2urqysaco.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2exqyaroa.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iryknapd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2amukeyke.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2viymdseh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wvqpjuyy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ylhmflsa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nzvoxoty.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iatmaazt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dspnoytv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcnhhikc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vvvwzhbx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtftbvcj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axtsxamr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2sditxdmh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xnqaihcd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2aszzbdes.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gddllvld.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlnztjpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsjdzbvp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2wojjjpxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edlfoxpf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rfpopvbz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sabqneix.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2omcnecsi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zwxrchqf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qqpnnfdn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qpqhcrsc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rbwvaria.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2avgppabf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ebdqdqrc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2toiwxpad.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2krhikafc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jyothcnd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2asbhzuah.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2evatocyr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ddcuegqt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2hbjompre.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2etcnbdnd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lpbjnwyi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2iamitkvj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2wxrllpry.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ibgmmray.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yyghsoiy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2evajkbrg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zoovyrmz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sizupdvo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wrpuzpro.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gsfvtteg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wcyjjhgj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ajbmynfe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tfpdkyuy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tmsocsku.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2aappdops.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kklnwdzj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2wwtgqxij.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ukqvilvv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hkaadhxz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2smittswq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2wobtpvem.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aywxrorb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pebafrmk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kifocfgy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2razovrbq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cgftmhvz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2toxiifxp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dglsjdcs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2urwsqyng.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fcjnmfny.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2owfvudgp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dszdcmzm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zuoeypla.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cswblbwn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zurvoynk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2opjkpmzw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wiwuchuh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dowoxdvq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2uigbfktf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2hgltxfvc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aiancwpa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2rxjsniuj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2vrtluble.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2inwxenwr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2oxvkkddg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2bmtazubg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2qkmdtyni.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmkofiz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2opyljexv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hoqmihfa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2qovxdene.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2btqzhkzp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhjdene.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2elvtzcae.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vtbstbwd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mefoejus.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rkufcugh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zraacaem.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mtewcnyd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdeizulq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubplamtx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2exypxotf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2rwntqcjg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dkzkdlyz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ojyieisr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2yhpvxqvb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ipldijbq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcftfwiz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckkjiefw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mkfseeew.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mbwlolmv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kmjwkris.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2jnmeudvm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2tvuvtfeu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mhpcthnw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sbkpbkav.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mxiurqmt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nlpjlzbk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pvvbcxzv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zhkwjzpd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2splshzpj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bqwzrxfu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xkkwopbo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2pcjitkye.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2aamltcul.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2uzzdfpmn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kqbikrnb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2wtkqortj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ysycaxhf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2kfwjbcnv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pnsbbcfs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2trtxvibl.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tfojvpco.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fmaqxpru.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ytamufto.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mhjvvxwq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qjedqbxz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mxnixqbr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2avyuwogs.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pntgryto.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2uchhkeed.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mxywitvs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rfgkufvk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2atlakdyo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xojnuvdk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2myvtfcbt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qhuryvwo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kyfyhoxd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lkkpegcr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yhaptdap.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kpfknmru.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pbmjrhhq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uipmjmcr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jklpomyg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2xzglemzf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2reszzrml.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ttvcfcax.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cfoxxjco.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nwtacgeu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dbohgncr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wndkzdwq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2aumwmxqg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2tbcxgoxi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzevugxj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wdpshmuw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2myqiaxya.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohvtyybn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ihahhwts.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zhidsjqp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bopofykh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2navhdiiy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fzpcsfca.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tsgnkpbk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cuthappx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkjnrudc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vdgtvpgz.html


<!-- 参考信息 -->