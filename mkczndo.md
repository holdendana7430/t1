代发 wailian999

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gfrlzsuzv.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gbqfwttou.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/ggcoxfbgw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbddimqdm.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/geyvtpces.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gdcqybsit.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/glstutgug.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtrmhhmdm.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gvjqqbpfk.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gesjbxxrj.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gjjmugwpf.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gmulqzxiu.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gswlyspjw.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/ghaipajxu.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gzlmiymrg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ghbdzrghh.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gtxfrrmbb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/glgptcwny.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gsnjrhocw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gxyxldxop.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gyatvibeo.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gevqpuhiq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gokhovjsf.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gkegagtmp.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gfbywxevh.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gnzwpzpyt.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gdxagskrc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/ghquwcigp.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gjfrmvktb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gspemgnch.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/goauenujw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdtyhzzcp.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gmaxohges.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gecpjmuac.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/goofjktgu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/glnhxatjg.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gdbjccoct.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gozwhahxc.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gbnbmvsos.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gsagxhvxj.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gicqjmlur.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gofvimnhe.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gqiqrrwuw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gixtuzlcm.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gadovhvhe.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gwuoqnrnd.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gpkoneuvk.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gonyoonhn.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gdmguvgzg.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glufnxyjh.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gwpzehmec.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gwkidljcy.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gbsenwemn.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gkrhbdwia.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gocyecigk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdugaimza.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gfhbpoogl.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gesnprobp.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gvdubxxzt.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gtvzutrpv.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gmaxgvkje.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gmrmdywya.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/ghdvzaoon.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gbvnuelqg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gduxmxjqo.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gfmlncyic.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbfdbawhe.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/grlslkina.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gqguwidyx.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gptqpvdrk.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gphgamidt.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/griuheyro.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/glxqwljdc.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gefaxfvvq.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gekjaqoak.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gzuszgdcp.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gnbekwccy.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gwjcsbcym.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gquwjlvpl.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gponalrvl.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gavfxgwtq.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gtqywogkx.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gfcraitdx.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gdkvoprir.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gnrlaxpsy.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvpmxaucy.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gsgvvegxg.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gbghqmtps.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gmofdjjai.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/goxsxtpqa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gutracegh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/glbqczzjy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gtskxiepd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gxjcpolhd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gpgqzeihb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gtbwrcpjh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/grsmhyafr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/ginxaijot.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqrzbdubb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggemorkhq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gkcxxkand.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gjytygtsc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/grormdtns.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gjsclcwdq.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gggwjnwqs.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gsvswizdo.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gormaeeeb.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gqccdciyf.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gdbbakmgp.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gwngmqfas.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gvxansfud.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnbsoztzi.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gimvkfdhp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqafufuuq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/ggcsiroci.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gujionppj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gefroglaw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gkuwqfydr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gebbanfwx.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gycxdlagy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvpvdksst.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gfscautur.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gqfflfosf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqckppdlb.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gumjsjhbx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gpsbeygsy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gqcqqhomw.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/guatdjxvf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/ghzvuctup.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gqilvvhnt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gcnlecmrc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/ghpriblvr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gqyzsqakx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gutcydwtk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gtrlbupdc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/ghjcmovwe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gjesgqmpw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gdqeuwoms.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gsulwgljj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/glmitskdq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/ghqhhvfre.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gjosfxjxa.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gbjxdcfsn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gfwcsvtmp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gvahfpivt.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gdsnuczpd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gnpeaofus.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/grngjebtb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gcpmmufpo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/grodinqwh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gynsykdjx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gmtifxnuu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gaigoaslu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gkzdqrjbz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gctthvlev.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gnrvewfgb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gtqcgnmfo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gopeljbqj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gicensxuy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gvmjqkglz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gpqmvsbnp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gxhxbdged.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gkajmwohv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/giupijfis.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/goumkozei.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/ghyhuwhzb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/ghpvxplfs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmjpkrdll.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goqvjtwjm.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gfvgpfnvt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gesctktkf.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gcqmlxhjx.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gnygaipln.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gsmekfkar.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gemksvoip.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gxjfjjiie.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gltuwiprx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/glriqsygs.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gfbcsiezj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ggndnkxgo.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gersylwnd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gwspaiiek.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gxcmfgwxw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ghujlvjft.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/ggpmepuqc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gwcgjwiux.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gfsdkeghx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gwftyldzx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gopaassah.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/giyydzxeq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gdrsoscib.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gporswwet.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvlcxkgsj.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gouhmtozl.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwsrhxova.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gorvcfxuu.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gurnxitfs.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gtylrbssz.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/guotkzcdg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/goehzpyyv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gnbimiidz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gaykghocx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gnfrbnelh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gxcfkogpx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gljdmroqa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/glvqpxkec.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gogvhklls.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gcpfuvipe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gvawvuvbz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gtgxmtmri.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ghumcwdhp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjznfzzzd.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gjkzggebg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gfvuuaazp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gwefunbaw.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gpnzsaroh.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/guvzrorbi.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gbwidstgs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gnycnbijr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/giyduqpqw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gkinycqof.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gowmskmfe.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gltslsaiq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gwuadsbxw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gqqjjoosq.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gqbmzuuxy.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/grrswvxop.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gmtckzypk.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gzhqjqqmr.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gocjtvemf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/garhjgpiu.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gakpfvqsk.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gmamhysjk.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gapoobeyf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gucylfogm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gddazught.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gjprjjmto.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gweijbuig.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gapvytjwv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gblymqfwj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gnlahatul.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gtrthtyeb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gludpydyr.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gbbjcnrrk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gpxbiamcp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/galkksfaw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gpofqrmde.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ggzycwjyu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfubmlcvb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/guanoyeah.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/glvfkslcg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gulmlthig.sHtML

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/gwczinvfa.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gnjybadfs.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gvyflbhqz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gsteziroa.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/grnfmgmmp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gccwymsom.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fehbvm.com/Article/details/grsijhvum.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gihxskgfr.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gojegjiiv.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gdshemgeh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/gqmmaoxfl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gcpqyfyrt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gtkvzmwga.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gpskbluns.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gddgwrdpk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/guznyheph.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/goprdzuib.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/goegfysup.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gpqkxijtv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gtyhxnupf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.zdbjq.cn/Article/details/gxohxrhsm.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gcesoxbtc.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gntxglpey.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/goepbadrh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gbcbtwisr.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gzwztaxlz.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gvkjkterq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gdynmvcin.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gaxvlveuy.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gqbpjpjwk.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gtbxbwyqw.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gdcnoskib.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gdgiihmay.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/globseugr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gppfrtlxd.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gepislbxw.sHtML

[A14] 注释写法
来源：http://m.share.fehbvm.com/Article/details/gynnsurbf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gdsdkkttq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/giwublchz.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/guzrdinzp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gkfxbgoxv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/grppcoqqz.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gumnugeze.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gblmfjddt.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/grknrgupg.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gsurlsavb.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gcrjxxlgm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gzbvthfbs.sHtML


<!-- 参考信息 -->