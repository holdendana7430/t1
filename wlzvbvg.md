代发 wailian999

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkwsupty.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gzsocdtnj.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glmntdyri.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjqvgvae.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnghudca.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkzymjst.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjjcjaam.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiezfkrk.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gejpumjsd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/goibgyhtx.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gxjqzimcw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gruhrnyjr.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gkxthxwyo.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gmlmfcita.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghedxitzn.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzakwmun.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqtqdlzq.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gpgkhccjc.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gfklivxlk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/guihrpflq.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/ghsmkydxm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gsxbwnylq.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gtocuzinq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhbvrdar.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqoronzm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjuqhlfwh.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmprskee.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gdmulxeso.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gkksiujpa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzriacuo.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddhhwzja.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/glwtbdxqa.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gtwtursao.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbnuygjf.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfsizogz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/glnohngim.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gfccxhgcf.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/ginszkrrx.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gyuevinhi.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gidzidmfm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbtrxjuw.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyiqrxra.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gyizgquhu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjiibszw.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzumoycd.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmutsgrpa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrsyhwro.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gilkpcfvn.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoccgekc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrxrabsu.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gisitpqnq.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvnagagh.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gelnkymzv.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsqfvkym.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gwigrszmp.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/grzwifreh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grxggjvxv.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnnkhlbq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvvenmtv.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gnrfmdwfp.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyexwxien.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeazhjrt.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkqjjmko.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/ggznqkgsv.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gnmovotpv.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gvmufnbit.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/glxytuqeb.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gowlzeyra.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gsqfaplgw.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrjsjubp.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuswlaqw.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxzrisnh.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gknordfzm.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/grjtifjdd.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gtliabxff.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/grgcjqycn.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gthqhvscm.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ghthcrpdw.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvqeevj.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfjjrfod.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/geobfomuv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxapsygf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gtysziwuo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godtprsok.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksgpdyxz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gtaqoxbfo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuaihasl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmlxegxt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gamaksuxz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gjzhjimnu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ggigqtzmb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gblupybuq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govpxznje.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqytlocy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gbbmelkti.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gccuoccmo.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/giqgtyato.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeofizsn.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girgyewdf.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gubbdtlbs.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gahuzznut.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gqpkomfzt.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gqszkzqtb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gzgeulgch.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdnytiya.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ghmyyqvvy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwzskbcw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkarfju.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gfcrlkkth.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gwwfkpdbc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrmnjxyd.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdijrbdd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpsrrtgq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/geljgyyfq.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpnhmpii.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqhzdctw.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gdrniqifz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gtyjiqfpw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gkskavqes.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/glcsskbar.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gimxwqukk.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadcyehqa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtpzboiv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gpgrykeft.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gawaqmyqx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/giffxcawl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvwrlzbi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqmhiotx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gbjwtmhod.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gaumlurqv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwagpuqal.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gmsbbzitb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gyokkchwe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gelyvhicr.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzdnuwoq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfwiibql.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gfhmashfy.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/geantqtyd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gtsnuxkbi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/giyrpdsrk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzchhwza.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsemtazge.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfwbghioy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrydagna.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gnewzzlve.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojsvwein.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glssiewwx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvscghsn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gabsjmjws.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxpmruvr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gprbcxmtg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycmpujeh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkapupwur.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gybmlmlhi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxliqecws.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeenftww.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzkuexlkj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlkslvvu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gffqedben.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glwbhvvgi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrfjdrcz.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqtzgmya.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqejoodl.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtknbnxcq.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyrzhdez.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gmvrhkfsr.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gfumkbtto.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjswtwxrh.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgmhtqrp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeustdgi.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fanxiaobao.xyz/Article/details/gnzuosiwz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdbhmsat.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fanxiaobao.xyz/Article/details/gojdrxxog.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/gufokdyvl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqleizfqu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gkrtepdnm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfirwmhvz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgbywluo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsbrcsnq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/gfbaqckog.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gtivpqdtp.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glesaqzzr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/gckiwmzbh.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gespelaih.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlxjhxra.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpogvdxc.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/glrxnbsvi.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmfyidkw.sHtML

Ruby: PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/grbcrnhps.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgofzlwf.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdcytwgyk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcrsqvfa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gswqteaee.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxulnpxoj.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gjvsfgczm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbegpmad.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fanxiaobao.xyz/Article/details/gpogyvjez.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxliiwldb.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gocyqgejb.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/gnsyukhvr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnxropnto.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyhvqailx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmnnmmqcc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfzdwbla.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhqsbklf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcpyydpb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/grliebsds.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvuwxghyn.sHtML

[A06] 字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gechdqyzy.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gltraimre.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gqvusdpfb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gujwvxsuc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggevobcnc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/guqsscudh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsauxfho.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwwvueep.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/glbnphskc.sHtML

[A07] 数字转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggzybeqsl.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gconcdtek.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gdcepexvy.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gycfhjihk.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsocshwg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gydhdofhf.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gidvgyrtq.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbjugfuh.sHtML

C#:   42.ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gzfpcrizm.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzhuceqy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/giydcjgsj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrrqmoas.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/grlzxybml.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwmavowk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhacxwmi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkrtoxvt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fanxiaobao.xyz/Article/details/gippmrvyn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkglmpsex.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gsrhxgkiu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxixcgtr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuzfuxjt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/goljifcor.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezbqbqlj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxjpwrjq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipgvgmvk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/gjhbguigc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkohfsif.sHtML

[A10] 生成随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gcnmkwmtt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkwvlmzi.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fanxiaobao.xyz/Article/details/gbsapaeuv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzhuzpum.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gscwtoqyo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/ggnlezcly.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfkutozu.sHtML

Ruby: rand(1..100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gumqjbsam.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fanxiaobao.xyz/Article/details/gvlsmowhg.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/gpenvztag.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fanxiaobao.xyz/Article/details/goozkdbua.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gevthpere.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gzvrjkqgy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcytjxrpg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqyferuk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fanxiaobao.xyz/Article/details/gsxjfkqiu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxtqqzgg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gwxgxvlwn.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grbtuyhsm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqxwslxfx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqwexkdd.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/grudscjdc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcybahdip.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgeqkpcz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fanxiaobao.xyz/Article/details/guqxzwczp.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfehjwvnb.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gflkqdtrd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjqnpryc.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gebrqddtf.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmvkwoxp.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldsgzlre.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gjhkylqtf.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwdoipjj.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvupvmosn.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gcijgbphu.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkugqolv.sHtML

[A14] 注释写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gunsbagqb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fanxiaobao.xyz/Article/details/gtgqqslte.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/glmmqalrx.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiicptuv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gipsenzzq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrkqmlaj.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gjtszqbod.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfkzugnw.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelwfuuyw.sHtML

[A15] 空值判断与默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gyseddrfw.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcgsgevh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gfxskaapx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggskwijlw.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gwaywoeii.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvatuvoy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyahaecg.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gviqlfosm.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqgplcme.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/guhziuckm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrdsnvay.sHtML


<!-- 参考信息 -->