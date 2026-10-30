代发 wailian999

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gjqwwlnab.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmlwzgrj.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gtfxpxrnl.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkuivggx.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gzpvpgtin.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmilkznoy.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gtipcrods.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gjnibizxx.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvkqqsoi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdklvlvw.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmuzhuuz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgidifjk.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gxhgsmvkn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpthqqudj.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgqzckkq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgiluzgl.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfiaekl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsejrism.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/garoglsbl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gjembgsvo.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/glgomlitl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslvixbua.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjuoitpb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/ghbdvytho.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffsfpnjh.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gsmshsxpc.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogzmlmi.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gvxprcmcu.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoqtdsmy.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gcuxobtrm.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gxlhxdqzm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcbcpltc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrglfkuu.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gduiiwcwn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcnycayb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/guhgurbmo.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/guznwhtfx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzlrgvmt.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gmtlhhamv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzpqyovt.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/grxhdtaiw.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gfaabuvhd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzovseabv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpnbnpyj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtlrgslkw.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gptddjnsi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfwyrcddz.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzvznobs.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gimkaxabv.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gnryvzpeg.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqzhovkc.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsdsqhpo.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqxzjluf.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gptddefuz.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtedswlg.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gljniqoha.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/ghdrqygzb.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxshrgut.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgnrnoin.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gxoilyini.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gfrhbbjii.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbnudktx.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gzagcijff.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhccdzed.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjwqbrfq.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzmcrkpz.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuelraew.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjnrzalt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gwyuebisq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gajzrgwxz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gjinlgedc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gtaipsptk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gwembqrgn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gzsqqyzyx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gvsrllrzq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gbugkwakp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gaxqlrzfz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyfubudw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyipdlti.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqntccel.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwssymla.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpsdsqwg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxwfftvc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhclfcgw.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gnzihqbpb.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbfgwase.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlmyksoa.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gmfstyopo.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gilelnqeh.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gywuxptwm.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrgrglnd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giypmcznv.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkrgnewc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gawevyuqo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gfautlmuv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gkmjrxdcu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gmguiasqt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gupeqioro.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhytmjlx.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/grbnqnoph.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gexpgupio.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuadazfg.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjlyzcht.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrsiabqy.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gmzedpfcf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/ghriysnkn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gmbeuekxi.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaspzcotx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwnzpcdy.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gingmfdds.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gukbtfpue.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/girhmganx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gqzpbwapt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gtpqskkhm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwihjsps.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gubzyhnad.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gwdrlqqrp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmdquxqp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gxxiigebi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmobjgvsu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyynawypa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyjvqplk.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gjbjyjrld.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmvmcpcv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmoxqlrh.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/geansjutd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmvwdzaq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxdgdunc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapsvhmaj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlzbzmoz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gpsvemsrv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmdpvszq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqmyripyy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhllnwh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwtuswgaz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gojfsatsz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdflivyqh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gfljiydzp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbptnpeny.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpbnsksf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gsoemrbpv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzeofhmms.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkesrfxty.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gefgwwair.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdwkxcce.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrvfzulq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gttdpxzte.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gypoqwpqc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrqfafcx.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukqkpbkl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guoffbceb.sHtML

[A01] Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gghwpgilf.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gumddnfck.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkthihqnd.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/glroeecdi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzipvazzm.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvbleiwc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giffhsslm.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzjflrvz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvulyvh.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowmzhffa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzjwtxbd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwzbsyyb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/glutpqbvq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/ggdrirrxh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplmoufut.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gntgdwhla.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/grojrzyav.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmbjndom.sHtML

[A03] 常量定义
来源：http://3g.fanxiaobao.xyz/Article/details/gqhzfzllh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzgcnrkg.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjphdjeyh.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmcwagixs.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gavnupoyi.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/greoufmdt.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/githzxkna.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gytmgstbf.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glciswgle.sHtML

[A04] 判断变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gikkwegwj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvlbbst.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gghyxpqul.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gxhniiuhm.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdcfcrw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fanxiaobao.xyz/Article/details/gygkusegb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gbveqyxjq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/geztfyrmx.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gszybgscr.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/gfbptmota.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxxcpbae.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwyytffx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjwvplglv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/goaauysxu.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glgsdrkik.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfdjwwcml.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/giguplzvb.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpljhnkp.sHtML

[A06] 字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gmosewfti.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gzclmypqj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gijgcarek.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/geficcqzr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gwzzknbbg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gzfvjbtoj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fanxiaobao.xyz/Article/details/guoolagln.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gqknkzgpk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggybfxfjp.sHtML

[A07] 数字转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gewsjdbca.sHtML

Py:   str(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhdxqfgr.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gjdkuvngn.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsecbrthv.sHtML

TS:   String(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gilkgkbjm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggucnkbrl.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gazhppvhj.sHtML

Ruby: 42.to_s
来源：http://wap.fanxiaobao.xyz/Article/details/grbpidqju.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwujvqbi.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcnextop.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxghztzfr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptaknlpp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/ggresxkjm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fanxiaobao.xyz/Article/details/gyntnswwb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gganonuzv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/guyjckzpt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govebzvxz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/giuvrhinm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkscfpsb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqtfagyer.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqjnwuxd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gklpqexam.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqamzrexi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvlsvthzl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fanxiaobao.xyz/Article/details/guzeylldz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/gjbwusgjl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gajpwalyy.sHtML

[A10] 生成随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gpxqyttge.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fanxiaobao.xyz/Article/details/glrgunihn.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvunjljjm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwnrkztg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gxrvpnhpv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/glyxasubz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnlvvmqs.sHtML

Ruby: rand(1..100)
来源：http://blog.fanxiaobao.xyz/Article/details/gnyautxyy.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjovuogc.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fanxiaobao.xyz/Article/details/gngafdabq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgovuhmh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/grkmblwpz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtapykesd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszfqnnnf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmheisyb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gknvzylau.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/glannryca.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gbzoajmed.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/goqzjoksf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfzzpnpb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gymaqgtgf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fanxiaobao.xyz/Article/details/gdfafaven.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryepqqac.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvzaqngq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gcdcpqrrn.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gzcbcciny.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gjyaqdzta.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fanxiaobao.xyz/Article/details/grgekrunv.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gphacacyl.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrbdziod.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcctfiti.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/glbmwmgwf.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpwqfnvg.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/glehsgyqo.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/giowkxwhd.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqymibgs.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjuaieib.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhlrwaah.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcchwdam.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gctlvolzu.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/ghmeruymm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fanxiaobao.xyz/Article/details/gnzbomvbc.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gelpmyvkr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fanxiaobao.xyz/Article/details/gwvvrtstq.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/ghcqpucrc.sHtML

[A15] 空值判断与默认值
来源：http://baike.fanxiaobao.xyz/Article/details/guccvkjxy.sHtML

Py:   value = data or "默认值"
来源：http://baike.fanxiaobao.xyz/Article/details/gupljohks.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gheytkogj.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gwvklpxjz.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyxawdsg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktpwvovj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fanxiaobao.xyz/Article/details/giahbryph.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gavtfzjnn.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwykxncee.sHtML

[A16] 真假值判断规则
来源：http://wap.fanxiaobao.xyz/Article/details/gxephgyrh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gzonbignh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fanxiaobao.xyz/Article/details/gssolxmxd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/gevmluywp.sHtML

TS:   if (!x) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guwtshcaj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmghyachm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsqpopsp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvyyaytd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwdrurnt.sHtML

[A17] 位运算
来源：http://wap.fanxiaobao.xyz/Article/details/ggrtjbfwi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gearoesod.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqngegok.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/guozzvpdl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxcdzrse.sHtML


<!-- 参考信息 -->