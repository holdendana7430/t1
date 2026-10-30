代发 wailian999

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/glbclxivv.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gwsgtrjld.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gzpvvyafi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gvfpjifco.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gtpfflyql.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gxzncxghg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsoetorqe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gibezgidw.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gtmzxkijy.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gwshpmkvl.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gdyjnatkw.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/ghmzndwoz.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/grmkpejkk.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gxfqmwkdd.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gljwsbkyh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gawyblmnn.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gbxmmdecc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/grsbsluwl.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gyjndeuow.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gizqcljkw.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gacqdjccq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gasztpaeo.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gyebfjari.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gwlyqypae.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gaefschvi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gbayiebzz.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gcqwxknop.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gfrocnqpi.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gpcynxpoj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gbhmtbiqn.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gnsupvcrh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/geufgdjsk.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gnzmefwlu.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/guzfkkozz.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gciqxnezz.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gprtgvcuf.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gljonewiy.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzsnhzk.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gwyhpwuxg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gdqczfwxq.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gihvbigvr.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gdezmnxwu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gyyrzrlle.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/goxjxmvdi.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gzpfxmsav.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gzooldgfu.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gmwiglsyc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gamddysjn.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/ganxtvcvy.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gwezqsrph.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gkjcsbubf.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/grzjnscdy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnlnyelpd.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gbaqwpdgi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbnngiclc.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gjikydrpa.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gpimpdeff.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gyypyxlrs.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/guswpviqn.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gvfwrcwtx.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvzrzrt.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gznxsrloh.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/geatffozd.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gpaqpnycf.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gsxzvkbod.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gzmnatrxj.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gydtxalur.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gbqfkgsuw.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/grishellx.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gtsbjtfnb.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gymxovdmy.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gahbboewn.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gsiqqpmkb.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gvcicnhxn.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gpcgqvpzk.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gvodeugjs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gqckgvnog.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gxrmwzfcz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gxyurgwne.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gylnicslv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/grvhfivfl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gxghfwjrd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gkuvzgmux.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gzjkcauvs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghpuqiyqn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gbppjywhk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gwimaaxwx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gzpqkzxkl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjkfptyhn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gtwtzudyd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gtcuamfpb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gsomjsjpo.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gxoaemqzw.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/ghusetexu.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gtgiqnwnd.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gpmwuilpn.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/ggnfpusgj.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gyfwyivyy.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gmvlvkghs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqwtgmmjo.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gczhcbazz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gfvmaghxo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gtylguvmn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/ghdhvzfvs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gcufhbbaf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/grzksqydx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gafruldry.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gbkvhvmem.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwbqifpeo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gvwhakkwf.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gizshqoql.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpozbwwos.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gdfrkpqpv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gazcjhmuo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/grbdcifbs.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/goycqyosc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gjcmzwciy.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gflcjtjfl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/goncrkgxe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/goqhgfuyh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gsidrgucj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/glvzzqdfo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/glhvriyiw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gcbsughsz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gwptbtamp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/ggctkffsg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/geaanxyzp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/goycouxgq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/ghhdjjgpn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/glvxvjmdb.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/glxujmqyn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gcbmtryon.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghxkninbk.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gmhtmizmf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxggifbmj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/ghwqkwsgi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gthopjnhb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gdiwobhmv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gjachiboz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/glxvyautg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gdpeocotm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gguntrkaw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gdzzhgikd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gxqqbhros.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gucpzsymf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gmzioxrwb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gyrrxoeqb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gffiakxla.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/grgubaplm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gntvbcpfi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gowqkxpvo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/ggdfgbmpj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gddcbfhpt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gfzpuvxtt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gauzhnhba.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gwsiybvze.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdhkjpfwb.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gguiargvi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbmlearvp.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/glivqrvds.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gtyqtnadc.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gypbhfmcw.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gotutsdhi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gmzdapxwc.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/getpdvsnm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gwzeenpdc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gbcbniooy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/getrlymiy.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gjaaresjy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/glbclbmac.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gwoknasjn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gezkreiig.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gmqtndkcj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gwsxoypcq.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gqaxgbeha.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/garcacmeh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gypquetiv.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gwceqijhi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gxhajpwzu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghajjzmtj.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfytfxzei.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmiuhddyx.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gzxwipwtd.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/grrjzpnnx.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gnvabqxrq.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gfbrfwvkq.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gyblelsfn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/graqmradd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gflaolyol.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gbebtublh.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gsguypuwl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gkeyzubao.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gjvbbzlrq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gdjaetvqv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gnuzrgnjy.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/ghjldglnl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gofodqmwh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gwzndgmzm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gztdhutgk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gpzfholxt.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gstzoheqn.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnjbdkhcv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gdnqefywt.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gvoqmacsl.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gjvrgosqk.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/geoaektkg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/ghpnjftlo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gustynnco.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gcmyyfcxq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gqintkhlc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/grkwrkrdo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gzvdqcpdu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gyakgufdh.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gamxiajvl.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/glcigiyme.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gbmueimmg.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcveuwiug.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gtfkjckxr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gtsvbgvde.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gxryorhut.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/ghrhslljk.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gnznfavom.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gjfwjunle.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gztlfbhkz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gcvkromat.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gfzaegfcb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gkfpitkux.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gzgkkyhvn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gveqxxejo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gkwsgofkq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gnglklhah.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gugmrpovy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gscpdptgy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gepjojchz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gippboxgo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gwqfbgxvk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gozamhuso.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gidoglwqs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gvcypmvri.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gijiawgpd.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gmdgdmvwq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/ghggbzuus.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gprghmcaq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gkmwciwke.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gdzmvtzav.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gvfylecgc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gbabqpdal.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/gmyonikfi.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.hesvh.cn/Article/details/gpmcwpnjy.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gmfwublqj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gfqanzpst.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gkmejgcwj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gpeltcjfd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gcnkbqigc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/goysbgozg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gwnqbzyge.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gprnmcedu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/ggxncptdy.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gxfyylajv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/ggfytozjx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkvwwbgf.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gkzaskydt.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gtutecgah.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/giftthnyh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gvqdlzmmr.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/ghpdyydoj.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gvvsxhkea.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/ggoxxwprb.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gcqiedzpk.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gqgllgavz.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfuorqfmt.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gisvscyvy.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gtnwktdzd.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gamxlyjri.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gfjyglxnm.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gwkboiihi.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gwfswahhd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gvtushdbg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gwrifgicg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/giceitvan.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gqwesistk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gesdgkags.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gmvlcaiao.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gqwzyzuwq.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gmwssgymr.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gskdudoim.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/ghzarjsud.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gwaqqqwkx.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gpicrzzvn.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gvzidfren.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/gghmupcav.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/galavkbmz.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gwnbyjwcx.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gdoesgjeo.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/gmemzigqt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gvtfucaar.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gmvduleku.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gdwqntesf.sHtML

TS:   if (!x) {}
来源：http://mobile.zdbjq.cn/Article/details/ggsdrinve.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gwtbiwzff.sHtML


<!-- 参考信息 -->