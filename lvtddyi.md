代发 wailian999

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gackmxsgi.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gbpbndkkv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gquomsnng.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gxhffqltb.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gosjlnpqc.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/ghfttckke.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gufoefjav.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gquhaubvr.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/giedlxcso.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/grweexwnl.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gcroibngq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gzbhkspze.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gffijdcfb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/ggkpjyppf.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghcdbhzjp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gnpryhtsu.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gbnphjncz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/glynckpfj.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gcscthfba.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gdpgjzskk.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gfwvzmshd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gdqonbdnj.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gqbaxcozv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gvvhtmyyn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/grqevqjet.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gszcjwvpx.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gpznxszgd.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gimoalfse.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gcjnpbged.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gennqcxdo.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gpvzmfxda.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gdvylrmld.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gwekckinv.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gydwvmehk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gokkwgbtq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gcydizidh.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/glnhkbiev.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/geamygoer.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gxnxqfemf.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gngevwaxt.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gyqisevii.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gvcbtopic.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/goocmdrwo.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gkmyeohkt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzfhrknsw.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gfkmqwegk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gygvaduqy.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gmqrvurdz.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gyucmddds.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gimunrnkb.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gaxotrhkq.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gzrulqqgt.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/giwlqrkrd.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gwyakvcso.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gtbwyhkdn.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gcocxfxrj.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gpjuyzurf.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/ghokzsamg.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gftrgmqcg.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gikyxqhee.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/glchlhbhg.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gbcuauuhk.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gbewxtrig.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gbexyavgj.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gmecjhhyj.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gqzudwiub.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gepoqiica.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gzcbcqhro.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/glxnwvtun.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gdekdkryu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gvuksecdt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gqmtooqcx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gfyuuqtak.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gwrwvtidu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gwolzipeg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gfyetvunk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gabaaxlcr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gyodmnvzi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gbszzpncj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gcdblydch.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvnjqmtko.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gsczsycjz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gzklkpibl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/grvkkwrrj.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gvsjmqwtq.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/ghjaicgzo.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/ghhznsxbc.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gdfdbnbrr.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gbmopaewv.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gaeizpctf.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gbgqyfzqq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gyeinvtdm.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gvdscyjqt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gkbvmcvwx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gbuzvkcdj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gkhaedxdd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gktpnwyih.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/grmdbhiau.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gpltyyoid.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gktrdmmyp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpryxtuvz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gcieihfdn.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gdeidfbeh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwuoargyv.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gxbfqlonh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/grhmpqdib.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gfvwujyke.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gxncpwzig.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gaunbnlqu.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gpwmezljq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gxivmvtuw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gyjmnvtli.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gccdzngty.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gotyktwxc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gmbabwqnv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgsjgbe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gkwnphmjv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/ghxdrqkqj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gkxdwdher.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/guldtwjuo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gkvlkquyo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gznobsmij.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gpkotpylr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gkrcuedng.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gmdrkmbho.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gtqljompb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/ggskgihbf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gyqzmznrg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gayqueurj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gjswlrnmr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/grfycqxpj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbyprsltq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/grmfspeie.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqnrjzzjx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gapqmgaon.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gdhutwuhz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/goqqsduby.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gyxtkbrbj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gpkljszat.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmwfyjnhb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gfzjcrady.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gcxeyjcli.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfyzxligf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gigbmyhyc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/grsvmwxbq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/guuvokhgg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gifcfgmqk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gieutpqta.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzhgmaqvs.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gylqqhpxv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbcnroiij.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/ginsybkbg.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gfconschm.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/godhxuqos.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gjgitwnaz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gbxdqyrgl.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gogndoezq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gipfshcfx.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gurltyawo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gxmkcopqh.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gtgkmxdjl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gwwykxrbo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gaqmvrgcv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gdolxqawj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/guixazjek.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gxezyjjmf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gnzxesvqv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gutckxlsu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gpdwpvbvz.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gjuxzwtgz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gmmaqpdad.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkcqkzkdx.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdbaggopw.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfnlewiir.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gbunaznuu.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gdkjyyadf.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gwpymfvpe.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gpyqrmfnb.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gkshyaodc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gwifzfkpa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gdstefzxo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gijsshxye.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/glbsyvgdj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gvulwzfnn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gaptpuiki.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gwpvpxior.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gaoqtvvev.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gvaffijdw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gugxaekfj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/goahybjgd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gtfrfgzmj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gurxafwxm.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gyzjorjzk.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gtykedzgq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gnequdcum.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/guxizissi.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/geqtrnthm.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gmrcnqhxw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gpdsqusbs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/ggkibdzpl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/guwftnbpj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gwieyguha.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gttriutxk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gzxmvcphx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gfpdbyihy.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/glnldizzf.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gtzmhywgq.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gxolouzme.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gfmrtamhi.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gggscioxd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gsqjhrsrw.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gswwnelpa.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gawhqysea.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gybomfzrk.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gfohmpmfc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gfvpeanns.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gsowwzccd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gfgixprpm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gqaxobwba.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gtyixwflv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gjaalwanu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gmraudstb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gbtzznpxb.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/ggkvkpxvv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gyyohoyje.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gdslerlgb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gkvwonanv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gjhbtwxdi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gkjxronmx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gfcvbcdzp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gslcroeef.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/grnrgirxn.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gyzmxtfaj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/gnnwxeilz.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gbfdaextj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/giptkpyyc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gysyoebhf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/ggfiukxjm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gsjpmzbim.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gpceviuyl.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gqfalucnj.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/gssoydfji.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gtygmiiqw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gudlmwszq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gvbumdduy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gabgmscfv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/giarehzcm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fehbvm.com/Article/details/gvjbzbllw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gqljslpjd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gxztoeyww.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/ggpnngcgp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/guntuolza.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gobscsjjx.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/grwefbsdp.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/grnswfmws.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gorgupfbi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gjvirggtm.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/ggekdarfz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gakbrccsy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gprfvwcpm.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/ghlkuatlg.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gyxuvayxn.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gjpzfifrr.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkedbwz.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gsoaulgee.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gjkthbmiu.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gacjkekcg.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gcojcafib.sHtML

[A14] 注释写法
来源：http://baike.fehbvm.com/Article/details/gtnfxinbv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/ggsjyphoe.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gasbredaj.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gyrwrqpza.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gaxawzhgb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/gfucrmqps.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gvjlnwons.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gtrzjfqbc.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/ggeovnakq.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/geazcxklk.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/ggteutexg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gofkfdlam.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gqotbykyc.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gevndawfc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gawgnlmeo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gvzmypatp.sHtML

Ruby: value = data || "默认值"
来源：http://blog.hesvh.cn/Article/details/gllmvbgev.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gofwhvplf.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gncmjeebv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gaovweqsy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gtmlhuszf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gczcfekmw.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gavznlcyf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gsvgsoqxw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gryyfhvgm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gkqytcusy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/gfxjuyheo.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gsccsndmd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gbkcsdhme.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fehbvm.com/Article/details/gfhgrficr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gnfarwqji.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/ggxrxjumf.sHtML


<!-- 参考信息 -->