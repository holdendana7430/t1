代发 wailian999

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/guwnhccbd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gyzgefgte.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gfzqvittp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gcrnmlsns.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/ghbgvjqkg.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gvpntadvc.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gobhthgxz.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/glmprfsmi.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gdylwmcng.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gtmwjqygv.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gotdjicda.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/glvepuvvh.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gmfjfdmif.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gnxrrtumh.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/grtksgspd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gouufteaj.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gubfhxexg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcjivmzrh.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gsasaexrw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gxccgzxjk.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gwfxfosdr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gagdmaydc.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/geljkqbbz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gkxdznono.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gunkwuthn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gemcweoyw.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gwpywwqhn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gqjoinhhh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gxnhtnxjx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gnvybnlhp.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gsgeiskem.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gpzqqvtaf.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gjmoxpxrz.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glbqdpeod.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gpygeuaaz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/ggsrqhjqa.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/grsiwsruz.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gvgivxkvx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gmphyiiqw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggwkjkwfe.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gmbrzzetm.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gnjgbzovu.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gbjpnkgug.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/ggigriduf.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gpwkjssyf.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gwcrbpeyz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/goapxdygk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gdzwvtoti.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsvrhyuvn.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gpixweiwc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gemdcjqbv.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gneeqivpa.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/ggmqkjrrj.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gfiblshoo.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gymvsoqet.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gqkwgkniu.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gwfmmhsbr.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gpnrtzhbn.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gdwsyrcrr.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gqlzmzkse.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gxjvickya.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gwisranjq.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/guodagxnr.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gxzlkdtcx.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/givvvuqbv.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gtxlssbhq.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/graeekuzd.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/glqehglel.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gucmjyklm.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gohtahczs.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gwtfxdgum.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/ghnbtbcmw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gtoenqicv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gzzfbykip.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/grjctavuj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gfvjvxbkd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gekngvsuf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gewlvnvdl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gcidhbwrz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gzgebdfeq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gfdokyqfg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gtwvgotbg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/guvzufvmu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gwfnbwzlc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkixlvmwl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gxtlpckbx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gpvdklunm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gqgarleyb.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gooabbtha.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gyefrywbl.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gqdwspzcb.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gzmfqljth.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/ghcmvikvc.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gskvzqdkg.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gheecydcd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gixrbrcsa.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gijaclbdh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gshcddkac.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gfyzcdrnm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gairxsecz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gpnunfphf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/goztzyfwo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gvrnlvqrr.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gjurlsfuv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghujloxff.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gwoezjhtn.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gjtbfafho.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxfjtrnhs.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gvlyttcgx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gwccumknw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gzqamllao.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gazpeizih.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/ggtikacln.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gvzzgbsat.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gemjbscee.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gijnbfbyw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gsdduparf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/guvswjdfm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/glqotlqgf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gmtpxzaxu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/goknpjkcu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/ghqxhwhxd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gxcfcambl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gazkizwzz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gjiqioxtc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gycvsrvba.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/givbiygts.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gjgdybbkf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gamzthuvr.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/girkfntbn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gfvfnroso.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/guxrrswkb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gndesnfwm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gghqgifmg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/grthoravv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gezuguzwo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/ggrgfpidc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gqwnnrhnk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gfjlgvgol.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gehwzsqvj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gnksiwgnc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gczyicsdz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/genmucnbu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gxwmnyezo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gtpzcigwe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/giepvrfpu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gwaeiyfeh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/grlmbwufm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gfdllhoii.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gnlbsnvkb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gdbcdpiyu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gkjtasuxy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glgpriipb.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/glgjnpgxh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfytwimjh.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfcrwvotb.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gfpdgeodg.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gdskrvwge.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gmtludlkw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gwgaoakdj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gvzkkmbur.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gbhjmkeba.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gdquwmttk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gawxabspb.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/ggnrtmcue.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gggroomtb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gsnryopfc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/ggtyffiqq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gbfsydxdj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gvsfboteo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/ghhiylzxe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gogglzpfi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gxkwqflnc.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gmvszfygg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gzhllkbcl.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ghlyqwfiu.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ghkbslwbb.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gaoiubibb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjgwadaqi.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gidywqnlu.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gfzxwlrar.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gtswyidor.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gahtraxba.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gvhrkmzif.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gljmvdxfd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gchycrzry.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gefecwjqp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gnuyojvve.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gvdxdgxnn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gvaugleib.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gcvujutrn.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gngrwrhwp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/gwabpwrvc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gketlxyya.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwqcsyixg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghwgfsjpi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ghdbcklpr.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gyykyktqd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gsclbvfts.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/glebhihtj.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/glihvaxvz.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/ghovwyhpv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gnatjqkpg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gmkvcjkqh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gifmllioi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gfesfzsni.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gagbcmdhk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/goigwzlze.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gvcrmtjjk.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gxdumobzo.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gnmfyjdqv.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gybwamonm.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gcntssdcl.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gdtabtkav.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gjfddohpe.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gsnwbuldj.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gvhiopbsa.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gkdchqwta.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/ggkpwhquk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gbwwnavsa.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/gevfxgbrl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gxsoxxezg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/geqgtcqcl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gerurxvcq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gzbqmsucb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gmwecmtfm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gmlkonnen.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gmrtigunu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gxqkqgijc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gawcqjgui.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gsypndsii.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gksmvqsrt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gndxsegnt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gypezpjev.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gzppxdcaw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gjakudmkz.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gpipkniek.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gttatnwyn.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/gfghebstl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gcxykyjhe.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gpsaaafzm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gxqwxbijt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/giktazjhq.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gglhpyfta.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gkbhydvfp.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/glcemhjiy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/ggbbzwkvi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/giycfkufn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/guouoenbp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gjnghthnn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/glilbvvgr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/ghoawizlf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gdyhuhnbn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gvoruahzd.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gmdpnzddr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gjbkduoiq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gbmlfgcqx.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gkkypumbg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/ggjjwswwm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gbgbvpfje.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/ggixqbqdw.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/glwtscuev.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/gnaevpxks.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gjkdzstzh.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gouxyqovr.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gllsonhvk.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gisbhjyda.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gcyjvllqp.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gzhuqheem.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gbfnzltcw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gpzmaeywr.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gnoouuiir.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gokanudsz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/grifkdvsw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gawfeonwk.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gfqadadxx.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/grzjawnoe.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gdmxunejm.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gjmgkjlsf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gkjhcrbva.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gvusaiirr.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gjfswrskq.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gbfkepath.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/ghhggexju.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gdceswdch.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/goytavvdr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/gyqrmnicc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gmjmailzm.sHtML

Ruby: value = data || "默认值"
来源：http://3g.hesvh.cn/Article/details/gxvmfdhls.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gzlpyvylf.sHtML

[A16] 真假值判断规则
来源：http://www.share.fehbvm.com/Article/details/gvpmpcnpx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/gzpwwndqe.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gszcmawzh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gbmjnzxrv.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/ggtqwnkhy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gzhjqauim.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/gxelvzhul.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/gzttbdknj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gcldacexe.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gleineypz.sHtML


<!-- 参考信息 -->