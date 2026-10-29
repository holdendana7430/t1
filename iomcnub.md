代发 wailian999

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gonynxkuj.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gobrgziuj.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gzfycxxwk.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/ggruuvjfg.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gdmfotxnu.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gqonmjyxk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/geqldfmla.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/glypoqdlv.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/ggjjxliyr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gqjuzbiul.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gcimyrump.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gajkolrlq.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gdxvotcrk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gwlatwglp.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gpimsfgjg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gtqkufmhi.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/glerfrdpt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gocwgodyl.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gyrwjehtd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gzinpapis.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/grcagzslj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gbujvixpn.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gapdnrhzi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gpdkgreve.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/grqgodmwt.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gusqvgcxe.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gqeshbwoy.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gjbjecyvl.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gcrxesctm.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxhaxhqbc.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/grychvyrm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gtcrvcrjj.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gbebwohrm.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gwziavuvv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gpzynqknt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gwvkdqpvy.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gtekzgvbi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gsdogpxqz.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/giclblcqy.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gixtbgpyk.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gtttngesb.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gqpyelayq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gwctcomwc.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gxeusnvev.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjxrwxepa.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/guggvjpkm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glylohfxj.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gsztgzimf.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gruuikkks.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/ghrqtvfay.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/glfarlmiw.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gindqlqzu.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gwtqpjgze.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gbgdghjgq.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gpnwjgsbg.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gwrogmimi.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gfcwdegcg.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/grenmbabc.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gaqgyevbu.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gbijxmbay.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gchkutfzn.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gjstrwixh.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gvhlohlox.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gkhybwtbg.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/giedmhtwe.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/grnfldgre.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gqjyljagr.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gsibsfeqj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gianvvlmw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gavfhbvii.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gkfqgsmwt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gtmvhamqi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gssqiiygx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gnjhibvep.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gesdmefjd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gljfceqgv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gokozvrqw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gqcrilifu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjatgpxnf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gisqndaoy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gguervcea.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/ghetvjeon.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/ggdllqibu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/guhwpakjk.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gtxmffirm.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/giwpmovxf.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gswddcodv.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gxcxxvpgo.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gssizlgoq.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gyrteqlru.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/ggjnabcun.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gncjfzoxi.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gfpghlqhv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gvdrwtyxy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gfexbdwqx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gqmvonupt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gwetdwchb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gkuqwqvqc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gyqttjmux.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gxjxlpdrx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkkzrgybt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/giptcebba.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gtekqlrdr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcauchxwi.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gsphcdcpg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gnumajrtd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gsfarilyz.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gnvobnwds.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gdfbwjkff.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gjhofbyeu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gsphrkgnl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gwnvkdbkl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/glqatyfls.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gvjqwnoez.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gghltlghh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gcbozednx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gthlntgyb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gmboeamra.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gedmismbs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gzcjjntau.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/ghxxaldlm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gggxalskj.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gcmswtxfn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gpqtubfda.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gygcefmsw.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gtnzkmyhy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/grztjegkx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gtitqzkpl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gtnofiled.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpdyqepcy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpmtnuoov.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gakeqcstk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/goafaxdwg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/ginyazjnt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/giedyrnye.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkbokvyiq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gzjlrolwj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gvdcylgmw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/grnixjyzk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyubkkjnu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gtajcduym.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gwvoxfplr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfshmxizp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gtqqxhbsf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxdybcq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gijzbejtn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gnjolwhie.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gijyfupqt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmhkqjtho.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gknecfrei.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gojyakhkn.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/genoxauaa.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gpkydjyyw.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gkbcmofxs.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gyfjsrtlu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gwgbovdru.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gbqipmvzh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gvyensgav.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gsmdonpvu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gibdlkzhl.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gbcxzqcai.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gxnzusdkk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gdtypkpfo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gpslrwqvu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gqbzwvpdp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gcjxsujsf.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gjzzlnsid.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gllwgqgrt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gyumsxhrb.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/guispzqfk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gvmbjjhbq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpjeldjzm.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjliihsem.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gywxmpdiw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcjetwbz.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gwmqawqkt.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gzftnxojo.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gwulvcdrt.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gfypwqusq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gdwrxiauc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnglnxla.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gnmhciusr.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gctuiaqea.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gqkrsbkyg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gwnzxalwy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gqgonahpu.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gnezipriy.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/ghmgcjtbw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gfjxckqbe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/guqdftonr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gpwbjgogp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfouyjlms.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gytvpgzey.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/glwkerzhx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gxfjrkhmo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gazdphgfr.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/ghcdebite.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gqyqyvvzs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gymsubovc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gzrjvspic.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/ghcdtevql.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gwdpwfhiz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gmilztjvk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/grtwsdpyx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gfbzywuyq.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/glsujrgrk.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/ggaafklwd.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gyxmukizy.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gefxqqwoc.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gmokpgjgg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gecwezhoq.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gjfuxwigc.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gbltqdxmk.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gethpjhne.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gnksboefh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gjddmkhws.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gjshufhgt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gaopkutyk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gyxjyuyul.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/grwgjldpj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gtzymsouw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/gquminuwu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/goyhhxdwm.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gqrhnanng.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gmixzwqat.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gxkyrutjo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/glfkzhcad.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdagmxlbn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gbdpqwmwl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gxybrktzu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gzgpwumgo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gdigfkasr.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gumvqinyp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gilexlrwp.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gpfkiaepe.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gkemmrejo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gyasakmhm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gzzvgrzbk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gzmjfqzfy.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gfjygesmw.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gzqtajgwn.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gbrmmogjm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/golepxpxs.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/ggeekngpw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gbpvwlaum.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gwngvhsfc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/ggmqlkyux.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gorfaghcq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gxaqvslte.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gmlwdsbfc.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gflrbixsd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gqromzpdc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gaqyqiyko.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/ggnjnaljc.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gkfevwwln.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gbqcwxjek.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gvfqaddcz.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/geuxrblep.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gzcbbivar.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/goaemoedl.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gbjnyrgkj.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gaelhxeqp.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/geqjytdny.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gdpqhkyqj.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gewavezxc.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/grihhcqrd.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/guwcdovhk.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gmqlrtcjl.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gowtwibdg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/ggkvtugqj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gqexfffpk.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gxdxndows.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gqdjqdpic.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gwpvsfthc.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gcimhbzfc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/geahbqhzp.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gilbtvdjr.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/gkmddaeoy.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/galiktcuo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gpgzjezam.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/glarqgphe.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gcxmyfmep.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/gofgdiwdy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.hesvh.cn/Article/details/gxccwurbx.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gqntrlqdl.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gntljwwmj.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gownidocv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fehbvm.com/Article/details/gdzxswuhe.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.zdbjq.cn/Article/details/gqprzfvet.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gqyxlokln.sHtML

TS:   if (!x) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpjxtbbiq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gmjdjivtu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gqcythrez.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/gxquahbmp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gzvquhxdp.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/ghumqhrpk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gqltixnbb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gikhptjpr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/ggezwtjjg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gastxvirr.sHtML


<!-- 参考信息 -->