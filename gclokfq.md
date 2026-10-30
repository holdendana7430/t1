代发 wailian999

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqtatxyl.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gckumierx.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gnpoqhhtf.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gweufbaqi.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcxojmjk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcuxpgsk.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsqrywtb.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyoipltf.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gshuiatab.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjlzdano.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfckjydfe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gudqfrpqw.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcvqikgt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gqywgejhj.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwnezjym.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gomyjzgym.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfayaqawy.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkezdhavt.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwprhhfip.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gfibmeqal.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gynchxxyw.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gyswgxigy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjvtptpj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfbitxahj.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmljnqlk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/ggtwnyuic.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gifxfukct.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkqkbmyc.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gcgcypifl.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvaglbry.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gtutdyilo.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gshwzcnmu.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gcpmlbvau.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrwwixuk.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnafsjwr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxerlxkx.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotwgjllb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/glhbgrtho.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqjicoqx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gstvadvtv.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/grgxdzcbu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gaveegjkp.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbtbddof.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gyotinxuw.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gneasbrko.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gesnzmzyz.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxwdtrlo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyrmcigm.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gafqraypx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gymzsvpsl.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gupfdherf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeidpbec.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqfsrmyu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcyusehq.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvjjqcef.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzgbbssu.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gshidnlut.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/glszgpcqj.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpibgscla.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniyqpxyj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/giloculxq.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/givfbqlsu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaynfrmr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdneeidxh.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gjtylcoqb.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlbirykw.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxccpilc.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gmpwxytnf.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gpjebzofd.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gwmaxajuu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/ghndpvchy.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjoozwck.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxmbfsjlb.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gwochdibk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpkwjxhn.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gguebapxe.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/geqrfbtvy.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gxwsolrtt.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gvydfkdcr.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixuevkbh.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwughxhha.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/glpmpsegv.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/guxpgsuba.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gwwmwapdl.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gntxwztxn.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gmllpvcwr.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvsjizgg.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/ghfifeskv.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gadtiigio.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgpisiwo.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gryzrcrpc.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/greiqwveb.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gknhknumm.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbinzohoa.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcvdohyn.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gxjxvtnsi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/guuwmezkz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdbcmluu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ggbaeodmj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubqaaelk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/grevmeawp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwaruais.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gdpfnlpmp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galywatbs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gapxavwhy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqwdawcf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gldojepns.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzfswdsw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gcmnaihes.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoxkupys.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gabtpriui.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ggpyylpou.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnndgyyio.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gznxhzeod.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gwclyxduq.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoeqkuco.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncktocdh.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/geaqtpmqb.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gguvoywek.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkfnakiy.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gsexponsp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/giymbwfqc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gqnflsncy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyilunvgv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgamqffj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqxtuszp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gjmgyghxz.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gmovxkiam.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glmljbgzf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gxjwbqqgl.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevzaehoh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gexpsiyvf.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/ginjtweys.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjfskiex.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/grbkvzwuw.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjqvffya.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfnrpjqw.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gmouedqcn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gwjrsopbd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/gljtzttfn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gaebjtttv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoekreze.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geexdqptr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/grxmnpujs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvgknoje.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gkvowcogl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvzeqsll.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gkwxeatbn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/ghezthmhw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gtavuekqj.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnpvwccq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/galessnit.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gmjtullnv.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlwsjcoj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokvtheqk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcipkkdqk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbgpzwcsy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gldrfqdsq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskcvkdgs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrnhqrbk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggknkqwiz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grqhfvdlj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwiiqyfa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzikdbar.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdwqiexsg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcxaefkh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjswltcwa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gobohwklm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbmznuhca.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/goayqkfft.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxahysnq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gsymatqrw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpocrwcsp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzyxwlicd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gkepypuip.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcugmgzaw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppivykjy.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdhgwquph.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbyttrqaf.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gamjcthtq.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gjalrvyka.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycnczfsw.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/guuzrwwnn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtebnjswq.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/goesijmqg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzupcumvz.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fanxiaobao.xyz/Article/details/gubmjbheq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvxgwdjp.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gcjbdfmof.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fanxiaobao.xyz/Article/details/geibhzazc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/grvneqxhd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnjnyoaq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gdlnjspgf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gedfudnnz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqoegiua.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdqyzlwn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/glcmwaevc.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/grqgrspuy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/grmcxsrmk.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/galffmkyj.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/glfnimghm.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/grqhefxkg.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gerpidork.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpvilsxb.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyclgcvmm.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfbqvdsz.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gclhovwch.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gnmyrcxko.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmoauwzsw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfkvbanx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytmsfsgc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fanxiaobao.xyz/Article/details/grvtovdba.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gajlueoky.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/geqfjzsku.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcajpegu.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/gubyzmpce.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnimrpvhy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgkulexj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssseaxzj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfmlsrwg.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwhfmkjl.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gicfvyvux.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gldtjxvjg.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gafaybpqd.sHtML

[A06] 字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnukkpvrj.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gjxhbkwfv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gengixzaa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpodoxeud.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gespvwigx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gslafacsv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fanxiaobao.xyz/Article/details/gaynliokg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxxwxbot.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjvoookh.sHtML

[A07] 数字转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbclcnuog.sHtML

Py:   str(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzsolzog.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtpyiwiv.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmwgxzhy.sHtML

TS:   String(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gtxdulupl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaioggvkj.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpibtaelm.sHtML

Ruby: 42.to_s
来源：http://3g.fanxiaobao.xyz/Article/details/gxvuaseke.sHtML

C#:   42.ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqqicnxz.sHtML

[A08] 取整与四舍五入
来源：http://baike.fanxiaobao.xyz/Article/details/gftmivlpr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzdtsxmo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpxncrxa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gwcuvvdcd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiwflipz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcrpalyj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcetxwaw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlrlfmed.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkjeqwbp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecrlgxvf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomcluajg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gfkeeyqvw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvrqhiepn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glcfssspg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyexeasxi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fanxiaobao.xyz/Article/details/glhyeuhkg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcjbtxrx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsiwjkke.sHtML

[A10] 生成随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gwaosmtst.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gniheimxi.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fanxiaobao.xyz/Article/details/glzcgnjir.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gfffdztrj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvxqnggj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gchsegzmc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fanxiaobao.xyz/Article/details/gxlpnlhnx.sHtML

Ruby: rand(1..100)
来源：http://baike.fanxiaobao.xyz/Article/details/gonuiupew.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fanxiaobao.xyz/Article/details/gynsfibyk.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxmojwji.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gjtlqknbg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gluwoufbw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gxdncnkfk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdssdlbg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gkdxkxurt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqhccajy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccgzglcj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecrgelbm.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gokknaoxr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gikdcacfx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gofyveuyi.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gckgblxan.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gkixvtyja.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsmwowzc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fanxiaobao.xyz/Article/details/grycpezsz.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gcwkzeszh.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gmnmwfccp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsulhggh.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gkcysznyn.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gbiqvvmuo.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gixmecqvc.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gcswyqxpy.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/giprrhrar.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gicmhnkqg.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gcrvuduxb.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnpobczh.sHtML

[A14] 注释写法
来源：http://blog.fanxiaobao.xyz/Article/details/gvggafdej.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gbackbfiv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrvetrpq.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoqseooe.sHtML


<!-- 参考信息 -->