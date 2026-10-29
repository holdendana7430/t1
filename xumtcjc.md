代发 wailian999

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gecjoncdy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gevjjmxer.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gftacgktb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gikjalefa.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/giryrlqah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/giwiswyxb.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gwfgghuns.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gzgczlzje.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gipunovvr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gvkquzivm.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gneizvufc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gkykczwfq.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gdzucnxni.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gbqsmqhpn.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gmrlwpzyn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gyvexxkdz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gdptcvcty.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gbtqerpfn.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gauybblhb.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/geuldcgfl.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gwcfwhlkc.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtfcoffex.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gmeohnnpw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gocbbytaa.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/guknnpdrj.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gchlrfpla.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gqvfqkifz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaswodpbo.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/guyghetxy.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gxptfkkaj.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gemstbkym.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gecxuqwbc.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gwxmlwhkv.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gylrjmbzz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/guzkmsscz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gcosgjeto.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gckzowvsz.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gfpvmrsnm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaiojtxqt.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gybrugjll.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gvhcxfslh.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gqbqynuuj.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/ggpdxifva.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gpeibjkyh.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gaovdzzzn.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gkmurjlkd.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gqkakczep.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/giopumfto.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gdonctgyh.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gxzmdcaha.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gjjtglcbk.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gdelztaix.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gsrkxgjwe.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/grplmrniq.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/ggzwnckdg.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gxswnccwt.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/galrurfet.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/grlqrwvol.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gvuwyzwsv.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/glxfojngv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gjkzfcfkt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gvivjqsep.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gjgpuopdy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gitqfrsid.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gtulklkzk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gmiuwevlr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/grmrdjpsd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/grqkpcvse.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gkludyawk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gjqbzprpl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvqaabocd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gpzndzquy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gfslcmlgu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gurkcsash.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gpdotwulp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjkypeuxr.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/guqvpnbua.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/glytkugxa.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gpmrgswvr.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gvugpjkyj.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/grnqorwol.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gcxxklmoi.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gyaaftdjl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gdiormlob.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gnjzgfnmc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gyhzzyckq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gxjrdnfwa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gdjfiakts.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gfwkufvjx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/grnhxhzur.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gkjeelpyg.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gndkudtya.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gessfyfvo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gyyplkqsu.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/grngjrldz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcmddoimw.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/glgpvmyur.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gypllvyri.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/ghamupmyz.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gisodterb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gnvpqpndm.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gdtifsvhc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gteuffcdo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gpjczmvzs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gnceqrsvm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gxifiykti.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/ghnpflany.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gjnqhbemy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gtyfgkrgf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gnogyxhbx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gvmbjbicx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/ggosyoqdz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gwmcuodxy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/glvdvzwtm.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gvgqywrqc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/grmtqmxcw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxuxlbddx.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gucdrkxpr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gcodljfll.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gwnlrulrt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ggbtgkcqu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gyusdaxgq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gbrzhsiqa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gbvoxxdfx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gvetkuvdk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gdwdokurc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gvzxjmwjv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gbxondkft.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/grtxlwwcr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/getaiuvxk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/geqklowvw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/guueoznmm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gkdeaardk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/guejtmmnh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gewopampa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/guyxvqzfu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/giubcnknc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gxraxlbnb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gdgurwvzp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gfciqkjau.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzjevwvwb.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gkvurazwx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gajsecddm.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/grfiaufbk.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gwjnvxekk.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/grxpmejpx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gkjhzokyo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gpejeuvtf.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gpnfwescl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gybgzbvgz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gqnlrdqja.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gyffnwpul.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/genjttneq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/glhqfvknn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbbinslni.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gighjhqll.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gnjyxpyzu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gptngiaqn.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gyxrydmqd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gwbchozqb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gzzzdtftb.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/geovkondh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gfwudtxvc.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gkzklapvc.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gaqbnqxau.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbatudnwl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gjjiumsvv.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gnvepfanu.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gwvmqjvml.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gibodigpm.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gzlbxebij.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gcktxwmuz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gxalwaews.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/glbeipkdr.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gaciostpa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gvevdfggb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gfcdftgql.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/glrlwqmzj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gjhffnmya.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gexfjkxzm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gcvjcigcj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gwearvwzs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gxcncbghc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/ggmjuvecd.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/ghgxmkzkr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gwqwozjnh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtjkhkrby.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gouwiepol.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gtgnrbutq.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/giclfprkc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gvkkwpjtw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gkygdlkda.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/ginxkecpr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gtzglojis.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gdvrynklc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gdwcenidf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/ggozuhinz.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gkfboqkgk.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gpsziqqac.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gaiokytif.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/ggewkcurs.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/glxplxbpx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gkkyosxgu.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gwpzfzhcg.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gcvmjotyd.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gstqdeviy.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gctndyubt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gjtklszgd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/guyexsceu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gijcetifj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gjaneymlp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gnwmvkhzt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gxuqvhogz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gdehpuiyr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gafmyzpij.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gimwlidzk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gwsbepmju.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ggzugibbt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gvmczcczk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxfzyxrae.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtypuhfss.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gmqhlyyre.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gjwlyavih.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gayexdqfn.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gvcyduxcv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gegzvyzsp.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gohblilkd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/giluboqis.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gmowgbqxg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gtjzqphmr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/gxemgukpp.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gsbecddlf.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gzftcpewa.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gmnootkew.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/gikbbpkrz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gfmgeloow.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gvbecruds.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gfvzgijtn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gwddlzkdz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gcydebxzk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gcdzwzqbz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gpyeocshg.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/gzifxjgwa.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gryslmsjp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gwkzjvbrt.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gioqdasdk.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gujcryswp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gxmxvtbme.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gxzqxrmur.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gyiomaihy.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gogotrhzt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/gbfeysqmo.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gtveeukiz.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gcuusjjqq.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gzaoigmwp.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gvzsnnxso.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gkoxylwgo.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gwehuxrxt.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gbrgnprbm.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gadajkezs.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gaatwvpfu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gjsdjohsx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdjpoxykl.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gjoqumsjd.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gvudiisvt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gnehlafgz.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/grbhdzszy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gkmdoqgfu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gyyfpewbf.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gndngdyjf.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gvpplverx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gqddqcrys.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/ggxemelke.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/geaiiwbvh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fehbvm.com/Article/details/gxprdpgbb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.hesvh.cn/Article/details/gqufzxypj.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gaiakecki.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gpxfzojlx.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gsopxuflb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/ggtkznbux.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gfpzaruyj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gqebltmoy.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gfmwxwgig.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gcphnvdaa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gwxfpxbcx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fehbvm.com/Article/details/gtjjtltuf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfentchnn.sHtML

[A17] 位运算
来源：http://www.m.share.hesvh.cn/Article/details/gxjbxpjjl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gyigksofz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/ggsamkeig.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/ghziszqcv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/griqpgmej.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gvmjbyhxs.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gqrzmbdii.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/giwyzwwzy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/guzbtpjre.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.hesvh.cn/Article/details/gbroeyafk.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gdahwregr.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gihqwtfen.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gkmnxpxdj.sHtML


<!-- 参考信息 -->