代发 wailian999

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gritvjbfz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gbhmmnfmz.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmlovurm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/godrgeyvo.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gqatvrqwx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmudaphov.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gqepvdepa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgkuyhat.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gvvdrbfdd.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxvwmsty.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmdmdlzx.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gometnmks.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntktnkja.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gruzrzxho.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/glxffzdbw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaeucsmf.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gkogqlhrf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/goypimbmi.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/ggtgpxovw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gywuaxtwu.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gccexovoi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhvyfgdr.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggjghnfxo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gwflxlfyo.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gtnkpmnjp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gtgqkeqpk.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbolqiqsf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gydjvpeks.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/ghykqxwon.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gyprgefku.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeezlcxu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbipaagk.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/guofmvrwc.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkbsjlg.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gaceflfos.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrkyclsa.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqmubkoy.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gcapbbttb.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdecbviwr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhyatayq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gegkvqjxv.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmwujbav.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrvgjwfb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdyqvktnu.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcikdxog.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gsbwqjrlr.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/guvykxnjv.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/galhtzqll.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/goadccvog.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/ggklwgokq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gtnpwhxfw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/geoxzxzji.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gikzdxugq.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gsczwefxs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjeudysdy.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcksbjrby.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gcidrueoq.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxzhbjgw.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwfcelpg.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrvuokbt.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gonritwje.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/grlfddvbv.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/grgpilfrv.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsalipssj.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gisnfvtjr.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwcwltpj.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/goyydqxub.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgxoiceu.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdvwlsga.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gfcjfmxak.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxeabhhi.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfnwjflv.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gjyjvpnpn.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkfnmldz.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gllalrwmb.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/grpnvcxbg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkgeaari.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwparigc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gfemywqel.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gqsdqsuix.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmosvpvm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/ggbjrqeib.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcgraxiw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrjtbkxh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdwxbucl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/ghswylazl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaqxslwo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmipmiwto.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gkysftnvr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gjewjigus.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/grpbnhkuo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdhlxknx.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/giiimjauh.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gommvdtfm.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdtvqerd.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gsxzzivgh.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/giddxnwsd.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqatkgcx.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gediqvltq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gheurhnii.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gzotvexfi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gplzicdzk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrbadzkn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeskbrve.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnwyislk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsqgcpfe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpolfcvf.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gsiahlrjf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gropianzh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwonjdkpy.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gslawaldx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goawlitjh.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjmkgoue.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/guohmozhe.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwhjfwzi.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gqpptojao.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtruccect.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabftlpui.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazczhgbf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/ghflnmwly.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpofwjif.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyxfxzhj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuwolkog.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegymigqt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxwwfcaz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkijqipo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gidmotdfd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gsclezckb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsajrhrfr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpqachbu.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/glsqtptol.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gerrptpfs.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjoriesmo.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwsxpjuu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gmeiyhcar.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafjhrshb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrcmitii.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gfsdzgcww.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzlwbyuy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gvudvlktc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxowwjtd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnntxbwy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnuwgjgs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gracfzgkq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkxyjeslp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmrsovzr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gknrckdxq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gsxcoggna.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyycodxks.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvqcetwpf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gjfhobvuu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwmtsimh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkapluazt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gifvtscbe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtjzcyxv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuylxebx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbndzwio.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmigffho.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyktumff.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfofbxsm.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrsdihtf.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fanxiaobao.xyz/Article/details/gpdilsawz.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gminpwkqs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fanxiaobao.xyz/Article/details/gbhnhflie.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gawreubvd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaawrbwv.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxasqnxwa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gytkcvufp.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqideomah.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fanxiaobao.xyz/Article/details/gmuzzaxrp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gcuxokznz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giydhzfxh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gnzubqprz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gluuebxtt.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gqiakpugy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/gxhocqkdl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnocsttu.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomjlbaqh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gltxuphnj.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjlnqmkfi.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpweowlnv.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gsxsfnmvy.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfvhatxq.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/ghbrviakw.sHtML

Ruby: PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gouepmkzm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijglpnyg.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/ghfkrqfxp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzqjvpvl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwjlhwuu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gxpcsjlhl.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gydrlmrzy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/glzxkmmmi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gxsdwdnhc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fanxiaobao.xyz/Article/details/gajhjmtzm.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fanxiaobao.xyz/Article/details/giqdbxapy.sHtML

[A05] 整数除法与取模
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuqpsubs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gowrlxqcf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gydzwxgha.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpnzhwmn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggotcigut.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/giaqkqfsx.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxvprfcpl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusuhfehm.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gudnjgfly.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gpjxrtqzw.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfracrehj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyjudchb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gavqxxnea.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpvtzues.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gnfmhlbvc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gvkpmqbeb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fanxiaobao.xyz/Article/details/gkhyguktr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcifustm.sHtML

[A07] 数字转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunlvbrkg.sHtML

Py:   str(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gcuyvktaw.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gogmkrznk.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gzcqkykoy.sHtML

TS:   String(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyoboihd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gqgncytev.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaisimxar.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlglayig.sHtML

C#:   42.ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gqmtnwwtf.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgtuvlqd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gbvnvigag.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntrumywv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbwruupl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fanxiaobao.xyz/Article/details/gljplkiix.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnnrevkg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebearldi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fanxiaobao.xyz/Article/details/gihkazygo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwcjcohy.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gwgthvlhy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gootefxeq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkjwzbyr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gndhtlxcd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjokfdbdu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/grggurkhz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdizizwm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gichcbcsl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpticlhg.sHtML

[A10] 生成随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gvdvrblrf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdiomlxh.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fanxiaobao.xyz/Article/details/gaswzkzzg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gygauaynv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpxiunlnq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkgylesu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoatezkn.sHtML

Ruby: rand(1..100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gggpkkimp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfwnoiys.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fanxiaobao.xyz/Article/details/gbcraewtt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fanxiaobao.xyz/Article/details/grbnqnkka.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuaiilqy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddrwfapw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzwlfiti.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmswzowex.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpnfrymh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxmyqpeg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/guzlislmb.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/glhrdrpwi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gerymcyck.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwipizpqw.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtjzacvv.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/gixfbvlsi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fanxiaobao.xyz/Article/details/gqjnrhyua.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgueqnka.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvkvgola.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gsyolcaam.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/gsboaorhz.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgvxaejw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpitthxzo.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzphhqaob.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrsqfalz.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkivlful.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gjsupxxyj.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gbaeynezm.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbbdyzmf.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqucgieb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgndvknd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyzkpkvy.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gtehbjthw.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gxfaulyca.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhyhqxyc.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gewvghwpi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsctevzqf.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gzucfeqjp.sHtML

[A15] 空值判断与默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gjgbxlpts.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnadjxfb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqzzylgi.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gaqxjgtdv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvtrafdx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/gjkmqpliz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fanxiaobao.xyz/Article/details/gnuubhqhb.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwlytnra.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gtsnwgyjn.sHtML

[A16] 真假值判断规则
来源：http://mobile.fanxiaobao.xyz/Article/details/gvigafovm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gayvgvwjt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/ganqmdybj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfewppls.sHtML

TS:   if (!x) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfkfhwoj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxkttxkpu.sHtML


<!-- 参考信息 -->