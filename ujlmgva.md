代发 wailian999

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gwhajhqym.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gunbpbbyh.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gzfqditki.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gdzynnrwh.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gpcaxvait.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbeyvkgct.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gtnsbyped.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gofnhoblm.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gqkrswuhy.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gkahhadlg.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/grbqdgbmr.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gkfbjkseg.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gujpaibph.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/grzbqtbde.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gqhohyfzd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/groyfcmbw.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gvntkcjrr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gcomneidx.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gdghxrxll.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/giowrsozn.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gjmbeoowp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gwgqnmlga.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gubarjbev.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gyfsxkfkz.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gdarsxpwg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gakwgbnvn.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/guicptdhj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/ghvyvljvw.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gfsvvpqtc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/grozcfiep.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/glcoxevrm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gjegpchks.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/goqkftkrk.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/ggrvoocmy.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gwpkyvjpl.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gootxjdxq.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gretndeln.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ghlflwhlg.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gnlmiedjq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gszphnykh.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gvvwjcrxz.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/goyuwvekb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/glhbnskyt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gowqybpbk.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gpjstlrdh.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gknhjaoxx.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gndkreqqd.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gtwijxkci.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/givmgbmmr.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gsunmrxka.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gfctbxkqm.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gkwnbivsh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtgebfwnw.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gtybhspvr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghbbpnfpg.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gjkqzcztf.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gmwrtcmuv.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gstinxepc.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gqhlrftgu.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/ggomwclpz.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gbmgxgivm.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gqgxtsrbj.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gvrqizoiy.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gefoeemzg.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gftzjboxc.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/ghzsmrffi.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/grqywtyhl.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gphrmwhtx.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gcbpcdead.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/ghbctewld.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gaoijbbmv.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gcwkingyh.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gvxhackzh.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gpihmzhfg.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gwqdpvqox.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gpcvvekay.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gnmudynjn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/govlqscga.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gfanmiqzj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gahlwubbq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/glhmiujxj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/glnmzzcjr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gbproshmw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gyzmplvnx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gvyskpfld.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gsokxdfvv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gevpsrtxw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gmequtrni.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gqybxopxn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gerabgmbf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gtqhtvyzy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpliwqsai.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/govwfoewn.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gomjueujc.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/geuezskhx.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gclqxwcgn.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gusfvqudv.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gnpynrugh.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gyudvqkxk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gadkbujwg.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gqrwqjmds.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/garodvkms.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gqpgzjcit.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gscdscvjk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gsrkulpdi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gasoxzyer.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gjdkorhwm.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gbzykjhsg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzysofwkc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/glavvcptb.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gzcmruboo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpsttidbi.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gfeljecaq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gfjjhtivn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/grtmjwtyv.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gxsgpuhwg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gzrkktydt.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gplexrult.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gclidzgvu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gsqopudov.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gfcptbfmn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gebchciii.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gaswywtpa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gpezooruj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gbmqpukwv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/giefhgpog.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gxglkzlge.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gngfpbbwu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gvidxxqyk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gbjsdyprr.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gmhjzifox.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/ghvqypznr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gruelauss.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gxkoiiabi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gipvjkpok.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gstjgmxns.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gzcmvcuvj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ghqhgrzmu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gnihimvxt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqukkdcmr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/ggveffygz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtoxtgwig.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gjstruxpf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gherikpcg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gemoavxen.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gohneqekm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/goyqwxuyi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/guxzikurn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gabijqwhw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/godnwzmtv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gpxqprtnp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gwljtzcfq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gkjbhadit.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gqmhsgscv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gxvfuuirr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/guzilopbb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmghvbpzy.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzsclorhe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grcomouhp.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gjllktoqm.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gattqyifr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gaelbqzis.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gkoxtzvcy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gqtpsxdxl.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/ggxkspdqg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gzmbfhqbx.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gmgeincti.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ggnqcgsnb.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/giukqqepe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gwjoqpjxh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gqeasfalm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gqazdikmg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gavhtfygd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gizxquhmi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gtctigduh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gzfxbsxxx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ghyzyutrg.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gvjximsqj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/govpdrimu.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gspnfbvzx.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gudauotvw.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gvynlkloa.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjbuwdrjq.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gsvosrcjr.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/ghyrxquar.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbuduvbsr.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gzmzucvri.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/ghwqbdzzh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/glskmcwin.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gepmrguin.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gmrrzxazx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gqrczrwco.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gifbgalrh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gsvwtsgeq.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gikisclkv.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gkcysmhpj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gonvfvzcr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gwnsuybtg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gxdrcqvpx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gopubrnyt.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gqklmcpnj.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gptvdymbz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gfkzqhjil.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvoavsqqa.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gurjgzpwy.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gbubentbz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gkblmdzeq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/ggnkmitgg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gdcjfrnwp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gftpnfvmt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gjkesieiy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gliyzkuwl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gqixfyifz.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnuqyydjk.sHtML

Py:   str(42)
来源：http://www.share.hesvh.cn/Article/details/gqvddyjzs.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gmujrjqhh.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gkconciiz.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gevkjfizz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gjuimksks.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gsnldchbr.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/gdaoiooab.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/goprbxvad.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gbooplwpf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gxxpgdjcd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gxlrmvtcp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ggxwdiyvm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gbyyeyqpg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gcgnqbeis.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gufqpccls.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gmeqamnlo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gazypmgqs.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/ggqcdcjux.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/geipqukln.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnlkrctoa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gpnurlsov.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gnvrkdout.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmwzyusiq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gpdftxfgd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gyonhogrg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gytkjeipg.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gthqorhse.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/galhmozbo.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gsnzgxkjg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gorhqhqwb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gkaukeduw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gkdokkovw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gveogfrcd.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gvcwajxdf.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gjfjsmagy.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gbxcmhfsj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gfyvqwilz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gddlptbkh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/ghnqxjmhz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gkkoimxib.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gmdqlgnnf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gxforlykw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gzbposjaw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gevfapjty.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.hesvh.cn/Article/details/gfgtpktja.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gqzpvowvv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/ggkhyywwn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gbcayccrn.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/ghfcqxvoa.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gogqamsdh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/geyivbmvc.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gdzqpzwqk.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gkwvmuidk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gakkboruw.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gdesshgzw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gsaujlykq.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gusblffab.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gamhtfybk.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gteplrwdl.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gwnsfxrpk.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gxngydxod.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gvxzcnypl.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/gqwhpdrcv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gvflsisws.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/geokiuczp.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gyyjjjnhl.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gorvgrxah.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gpfodawmr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdpnijvhf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gtoifodpi.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gljhietxy.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gwtiwnhme.sHtML

Py:   value = data or "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gwfvxffth.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gcghkhsmv.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gngoyfhgs.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/glvjmqbfi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gdgjcxoup.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fehbvm.com/Article/details/gvoucabjg.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/gybiachfg.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gmnhchnpm.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/grxisnuip.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gnoegdxsc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/guiphrpav.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/gqoybbfug.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gfkkthgjx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.zdbjq.cn/Article/details/gonbxmokq.sHtML


<!-- 参考信息 -->