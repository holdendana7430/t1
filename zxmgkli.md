代发 wailian999

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/ggcffsirv.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gmnwkpbhv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gjybveppf.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gvjsxmvyu.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gcnyzgfuk.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gazxydkcn.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gikezzbzf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gtrkdhohe.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gtgtjawyd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gmtboorfz.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gsgarhhkl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gpmzvueve.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gtkjjikry.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gzszbullt.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gtbfsbgjw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gmtlhfmwr.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gysqinbtu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gqgldimli.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/ggzonnrcd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gsokclaje.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/ggrzgsxdt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gpgqquvvx.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gdzugldxi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gcwfflxnt.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gdzaykeda.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gijwcdrdx.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/glgfjnofw.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gzetulqgh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gcvkhynfl.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gunlbskki.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gpesbqpkz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gsnpreezg.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gxcxwncol.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gawltjtrr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gghmuluuw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gfaviwqbf.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gjygsmnri.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/ggiqmgyfb.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/guyxjcevi.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gilzbqpni.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gqvnwmeyh.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/glfsbqmfm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gdzbzolmm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gdkdbepqc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnfrvemiy.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gdczfypst.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwwowkqab.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gbqopdbdb.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/ggpmyxrmy.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gqeaysocs.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/ghchydqei.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/guzadjcmx.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/grfmjwjae.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gletwozzx.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/ghtcqdeus.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gzmziaddl.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gdwvqfqxz.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gmxotvcnv.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gamjlwdrz.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gasmhetma.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtqnxoj.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gjjkdmloa.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/glwylgymr.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/goyghtsvm.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gubidhaak.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gwsxayyzb.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gjohsrpra.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gukqfezmq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/ginnftaqn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ginzbxeid.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gyholeycq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gingdkqxm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gipgegexm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gfamzhmww.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gebqdchqa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gaswuhpxb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gqnfqdthu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ghazhxfnz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gzpmadlsn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gufszklsx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gnwhynhtr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gbxfpctgr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gpxspgwhi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gopaojrva.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gzywbquhr.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gamoudwnr.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/ggzxwwegf.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gdmoiyqgc.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gfxflrnji.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ghdxfstrq.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gjmyduwgp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gnshgbikv.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gjcgjjbyt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gdyijsroi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gdrzuoblc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/ghgtepteg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gewkhltyz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/guokqeufr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gcboxsvye.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/grboimfic.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gymwyflcr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gyksmksxw.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gwhxrfaue.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjrkhdrxu.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gutnkdbql.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gzipqnake.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gcjrqwjdu.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gmwowjpeh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gxkrertej.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gjpcdhqwk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gifpvaxiw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gpfhicmod.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gysupwapz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gtlcntdcl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gbrdsgqdl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/guerhxczk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/guvyuskok.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gnwvhtjbn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gtqysjfie.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gouvnyxep.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gvwbqsoem.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gdnvysjhw.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gmaodqoid.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gpcnluydr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gidiacizy.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gcnlwfvwe.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gemgbvfgi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gkhfklxmq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gqqvqawtf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gfvgtgblu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gessvcaxn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gzfgvpfye.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gvzgcbedw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gqwgvpzhk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gdekpewqd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gxyakxflf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gwsowzpqk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gphvkdusn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/grpwrchde.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gzgbyheet.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gpvcxoljd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gpxxzsgnm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gsfhehdcd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gwjwnerul.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gxcxictxv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gyngimxpf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gjawtommk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gsvoscayj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwrzotpmf.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/ghzcpwdnk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glylvakfw.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gjmobwgid.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gymbpvtzw.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gmxszaejs.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gqlfanndk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gepahmbtu.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gahvoggwy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gakhublrt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/ggoooytxi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gswqegnux.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gcchuxxws.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gdzbfouwi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gsngadlnq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gnyzhnnot.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gzpiiarmt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gfhqcoapv.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gkhzvmvef.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gsltuooyd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gzccvzivl.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gzazdbgrc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gdbovtlrb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gteeflegr.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/glufgggeq.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/guuynopnq.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gcexrtmoz.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gifuhvhwr.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gapyfkaxl.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdvcvhdgx.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gszacshuu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/gjzuxfgff.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gslshnmqz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gcxvdpiup.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gchwptwse.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/guyktoocz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gzxdfuaev.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gpwmlvatn.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gydpsaecy.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/goegauhou.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gcttcakxr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/ghpvzruon.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gqlyzouov.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gvpbdyyje.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/geguijiib.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gkzzbykxx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/guxymyljs.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/ggmgmubyo.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gmbddriqf.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gmfplykyt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/geobhybon.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gwgizoogz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gdesggxoc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gdycqhapi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/gqabzpygb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/getjmfzhy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gtocjason.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gbbtiiqcs.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/ggrumsdme.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmkfuxot.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gfkmkoknu.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gcdrvkibd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gstznxznj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gsiuvavja.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/gqfgnlcws.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gvnymktfx.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/garplrkus.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gzzcebyzs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gcqnrjzpd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gqjvxnqts.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gcyoabzru.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gnvdsjewl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gevniiwsp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gweirxhbg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gkibuzkkh.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/ggzbyojyi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmevtfuby.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/giyxfnenh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/glcbtfilu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gjhsqizvl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghumswoks.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/ggiddjiqo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/ghmzhieea.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gvygwirik.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gdfdnjnft.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/ggknsnzxb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gomkrbsxz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gjmycepgd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gjdlxzjca.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/gbjzrvein.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gghcaulpl.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/gwzkdslch.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gncgdzdjl.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/gacxnrxkk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/ghfowcafc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gpapronvf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/goakxphdn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gmpmdjxfe.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gwchoztwg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gwlgvqrly.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gibvuhdfr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gervbjeyo.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gznuzukfy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/ghaojwovf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/gtpspnovb.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gemfylzyb.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/grltrgsbz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gpfvjpird.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxtgpdcfi.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gnwxidoew.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fehbvm.com/Article/details/gwljjqanc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/gdntozibi.sHtML

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gsiucssgd.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/grvydalqa.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gtlzcpmtn.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/guwakphgn.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gkbizrgjy.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gfmzlksvm.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gzpedcfrz.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gjfnsxlux.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gchqtncfj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gybajhbly.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/goknoyqps.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gpfbzohei.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gvlvzwgxb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gpbmfeipv.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gxbgpytpt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gqmurguaz.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gdqvmhych.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fehbvm.com/Article/details/glnxsgexl.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gasytnmul.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gwzbtwznz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gneeawdwe.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gylledcyx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fehbvm.com/Article/details/gclcxegfo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/gswdjrzdg.sHtML

Ruby: value = data || "默认值"
来源：http://blog.hesvh.cn/Article/details/groirfheg.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gprgqseym.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gtebntanq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/gsffbboiy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/goxlptjbf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.zdbjq.cn/Article/details/gdetgwruu.sHtML

TS:   if (!x) {}
来源：http://m.share.hesvh.cn/Article/details/gyiukimqh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.zdbjq.cn/Article/details/ghujygqvi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.hesvh.cn/Article/details/gdgixwszm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gszvtobua.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gifeygxgn.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/gfggpqleu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gydgwzgzf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gdzabfedh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gwulanncm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gwkgdabbn.sHtML


<!-- 参考信息 -->