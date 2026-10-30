代发 wailian999

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuvqldls.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzydsokt.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbvyosga.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/grqsnjsou.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/ggvtmjakt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxxxeknt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggncdpikk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/grctjlbpv.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gsinonkft.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtgprcz.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwlciragw.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/givvmhpyn.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavovstcy.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gqzjwbeit.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gjqxeuywo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicxhqqos.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/grpajoioe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gozslmxhd.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gbelybgir.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/grdcjzall.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuqrkluj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gerhagxfs.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqkcwmwra.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gljrukklf.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gtqknoyyy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gcfanhrtg.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmumhrbph.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gndfnznaa.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxficxtk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtgygkxg.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/goclcgofh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gqtcnnkjt.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfykiswf.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkemfpnjd.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwplynwwv.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/glxcuzuvy.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gaizmozjw.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqnmunno.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvelyzmcw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gtgnzwxfm.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gyomxwbum.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqpehtmg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gujgtpomv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuistile.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gwogmzulm.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/grystnqae.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerpnpbdq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqnvuohz.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzmwfpvy.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gxymyyzfd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbcqbwhp.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqdvrfhv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gseheuzta.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/ginagactb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbpfpneov.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gegxqrupq.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbsmzzbb.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmgiejgq.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzqcwxtd.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlylsfrg.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwsseozwp.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhjhrres.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gscfuacbt.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gnopdhanx.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhqjputd.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gkzuhsbul.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gfilcmshx.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gojfqjgvd.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/ggykrdsxj.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gdxsiduck.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gpnozjurk.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gwcsnjnuo.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gwvzaifih.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsiyzzwu.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gbnehuhse.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gzugjtakg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyxmantb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/goavidfxa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyhnqzlx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxtntpnf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gowzaffob.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvvzabjk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtyzffps.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/grrduflcg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrbnfptn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gumncrjhh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ggebmitjy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/ghinfsehc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gehdvdqfe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgwpufzb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/glencqpkc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghopcobvp.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gxswclsmw.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/glhekbvjo.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbqsbkhk.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gaxfmpknt.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryzvgjlo.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gywwhtyvk.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiwildyc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gisxiwanm.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmxjzkxe.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gpqqwbwka.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gictwttcx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrrnojdh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gbmauclzm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjgpadke.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoavfrfy.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gpyxjpjmr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnlovibp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqojdtac.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gvckumhck.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieenkolb.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqhstrdz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/glbpzeeqx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssrsyrch.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxphuwzep.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gpigjgzsf.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/glpkpfiqp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gzljjmzkx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gxkzjucca.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gphchpmim.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/ghvbavizi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gldalkhwn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchvgqpt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/ggvciuhqz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdtaxfwy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqqssyvp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/giyoqqyld.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gdivkrwzc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gbrimgnfj.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gpknxcfmo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjxmzdno.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gsrbwqrcq.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/glucscasn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajpezqy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghddoxagg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmsohblf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnapzpbcq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitrnutlu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjpknhcvj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjruquqgy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaqqvwip.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gytmodkix.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijrzemaz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbvctijr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gckrwszrb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkchrnzt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkrgbalx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grsuylhhd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gwvuekmrj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkgwnlxc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfopcgeej.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gqtujwsnu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtnxxyss.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gizbdvosn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/geyejqdkw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmhflsqfb.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvgpxzwg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawsuuvbz.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeulpler.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrxbraud.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fanxiaobao.xyz/Article/details/gmucuvcug.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjftktwf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwttstaxo.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxkpfjbl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcewutnpb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gijlengfc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwdampue.sHtML

[A02] 变量声明与赋值
来源：http://3g.fanxiaobao.xyz/Article/details/gkdsyrgle.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gshkxxrkq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gtgjnhlej.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gwaohcdvd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuoymtia.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gqtgmirgw.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gdyajyktc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fanxiaobao.xyz/Article/details/gnhyytlvp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqhespki.sHtML

[A03] 常量定义
来源：http://wap.fanxiaobao.xyz/Article/details/gsngifefg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gaeofyvtk.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gnadrhntm.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzryktqts.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdowzacpq.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdofudnwq.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gvivjkugb.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoewddvt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggklrcmya.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gcytrwffd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gjwgtyeid.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gjgcbvjkv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gyowsqdyj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvqxmwve.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gqndndmkr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvyerjeh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtraqvhh.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpnbulzm.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/gdinlnfmj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gudczakzt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gchbatdyn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsommhccx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/groivavdi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjvzhnxn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grcekgmiw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoyewtsw.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghabkntri.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbhjnyot.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gscfzmlrm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gadxkfdiz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuisbndm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuechzes.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gntazpebc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmfuzqox.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmmbccex.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzaucqic.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gadbeanal.sHtML

Py:   str(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcpoqtik.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfeuaegj.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddgwcvdr.sHtML

TS:   String(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gubqyufha.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gguefaboi.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtstuxnut.sHtML

Ruby: 42.to_s
来源：http://wap.fanxiaobao.xyz/Article/details/gaedepshp.sHtML

C#:   42.ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/ghxuplcxg.sHtML

[A08] 取整与四舍五入
来源：http://baike.fanxiaobao.xyz/Article/details/gluwpnxcg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbulblcnf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjcjpyos.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgkwhpwr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlyudltg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblagquwl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gsrrtswak.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/ggzbiieys.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/goruwhxfe.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdgynijh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbueezakl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrryltjk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsuleptsx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwtblmam.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwelfbyn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjntctfpp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fanxiaobao.xyz/Article/details/gjfjcxelh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaxbugta.sHtML

[A10] 生成随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabjsxjpo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjvpgrqc.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlnurneg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gdajnpvwg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpijnjrfn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowpgadlo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqukibmc.sHtML

Ruby: rand(1..100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsdumndn.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdjcwytg.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/gtqlytjom.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gckvlnowi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjuddutt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaatwdmuv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/ggbfmlxsa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geciscmko.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fanxiaobao.xyz/Article/details/glqgsdugj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gkwymanqn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gfnhlllez.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnewdrhe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiheujcw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwlagvru.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/gvdbkvtpu.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/ggjvrbqnq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gmhaurkqw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fanxiaobao.xyz/Article/details/geikfawce.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gbwetlxpn.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gawljliqe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsajuihy.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gvxgsqkaq.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gnhulplgz.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gogijanbo.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepmggxat.sHtML

Java: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gppatkgjw.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpyldlyf.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrslbbiu.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gocqfpyhn.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfyplrwt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnwtkfvq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gryfzrwrh.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gadhssmxp.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/guwhiyrug.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fanxiaobao.xyz/Article/details/gxkxkfnlr.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnalrhhe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/gifcbghuj.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjnodnag.sHtML

[A15] 空值判断与默认值
来源：http://wap.fanxiaobao.xyz/Article/details/geapwfsua.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfztoyzls.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlwpxaat.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/ghssbmctz.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gmumglujt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiuhwbwz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fanxiaobao.xyz/Article/details/gncjapvxd.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqqxmngq.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcerbcjax.sHtML

[A16] 真假值判断规则
来源：http://mobile.fanxiaobao.xyz/Article/details/ghupzpyfr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gylqicmei.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fanxiaobao.xyz/Article/details/gzsdxkkgq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/grmjdlxoy.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyibhynej.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyjtwexpo.sHtML


<!-- 参考信息 -->