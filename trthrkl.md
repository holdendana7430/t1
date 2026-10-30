代发 wailian999

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gcgextnjd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gxpxvczcj.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gpxjefnoa.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gngmeckng.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gkskiwmap.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqbcspsx.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gueiwsdkt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaabzienn.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwfiohxkd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/goysfnbpr.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gvcswyfgq.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ghpylsbbu.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gklyagslp.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gbpiazvyr.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/guwgynqbw.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gozusjjja.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjpylfus.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gpbmwjgdu.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gotruwsav.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/govdblnax.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gbzmcvkqc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwawznqws.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/ginybcadx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggufmuadj.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvjiesxk.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gdxdxmzue.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gtdajktvg.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqksvcmnq.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gnetweeaj.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnazdtjsx.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gfpbbrvyc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gguumyitl.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/ggpoifzrd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvevlmzhr.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfwakyek.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcaizuxq.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gmesnedfn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzalqpzv.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gerdeippt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/glcponytc.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexkmdjqw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gmqdmgaxo.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmxtzioo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoomxlux.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjudkqba.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gtvelnekn.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gdejdkffr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjelwobo.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gybiceqgt.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gdlwwvyzk.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltihxraf.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxgwrvrq.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gubzmftlr.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzaxtzrp.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gontfbhmm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/ggttwxdnk.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goabiyzun.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginvyfzhp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/greviktmx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gttuawubt.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gsfifviqy.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyonwgkg.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gljumgote.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guezzbdxd.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/ggygbbpcd.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzsvguyi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gljmziqwt.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gempduzoc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuitnlie.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gazjwhwhn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyirmlmws.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gpwsscggp.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gcalviskr.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gbqirgqeh.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gzeuczohs.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomahdsob.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/giyvjrogw.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gyutrlfcy.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkosjnwn.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gckvfcviy.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gvkvhxdyc.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/goyritexc.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvlxzrgd.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/glnsinitx.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/grkechtrl.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdddvikej.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelbsntmf.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gvdbdreuu.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/giufnpkjv.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gwuqpsbrr.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gbclvujqz.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gztrocoxl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmzeyrki.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplowkzkg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gucusztnr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gipujgxwf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gsuiaursr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gvsvjwrjl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gruxocjpo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkonpwes.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrnltsxy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gamxjkikf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuyqugzy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/grzwclpaj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlqfvlvz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbdbyuil.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzmuafvo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gnltfhvno.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gibowpezg.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyvdjxjw.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjuhrtt.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfdhlfxm.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxyyfbsv.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gszoygqly.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhdrurqm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnzbkqii.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gcwmnechc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpzochix.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhqaunlb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gvecukbaz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gnizfhpqc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgrgnwzo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gwpsglgup.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gciqmzwdc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gztybffhz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gchzwtlqb.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gkablnqlf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjqmtcaul.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/geddrukfa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/glblgpjlv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gyicppkgt.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gcbtmyfjj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmfycihg.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gemucxrrd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gkdlbbixw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaotrqbd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gdlqigzmb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/guccnkxwt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyciniiu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gfuzgxfca.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlmaerzm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/ghnwoqspj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiecutar.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaemntoh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gxgunotec.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiivwlqv.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdccvpyl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeuhoehw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gorwzvnhh.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxzowkqw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoeplhmi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzgdbcke.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gebmkuech.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbrjcvrx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkbidqcij.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/grrcwicli.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gqivoszvq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdsnjont.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdlsasoia.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gehsqmlpo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gimmkaris.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngnbbkjs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gygefmsrn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gdsnnotit.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glclqknsm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gligflbfh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxfemoew.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqdbtoea.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glymjevuc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gebwbtkqa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gjxamywdh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grvdmzptg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmcshycyo.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/gpeqokywd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gklctoehi.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtqvicudz.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqdiuadt.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gokcjzlge.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gwhlirdwp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fanxiaobao.xyz/Article/details/gwvvkocek.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniecsaod.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqmazgmr.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyptjikvn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghngozyrb.sHtML

[A02] 变量声明与赋值
来源：http://baike.fanxiaobao.xyz/Article/details/ghdekvedl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fanxiaobao.xyz/Article/details/giomiztrb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmcnlchr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfcscgzc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqimmgnlc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfclsgxtd.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gngmxnrtr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gbhqvfsus.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuhcpqxt.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gjzgrqpst.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhexkigz.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gykpgwudm.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrprpocj.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gkqqpgopn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqssexto.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gukmeylbu.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/govbpayox.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/guqiboogl.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/glmcxqkkd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gronkwunb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhpnsbpd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpqlzbcm.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/guphcuaez.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/gqtmubhmr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwqyslez.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngvtqnfj.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjfslfcs.sHtML

[A05] 整数除法与取模
来源：http://www.share.fanxiaobao.xyz/Article/details/gkipgwfdh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojiroxbk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gldkwokvg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glgeeqyrx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlvgaxnn.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gspghizix.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzplxyues.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gorxtmsti.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gclipjerh.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgudguuz.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/giiyqzauh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gusbnixmf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfbfufjw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gfzpufbnd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjqbsuty.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gojicjdhj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgjftvqb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/ghnwldevy.sHtML

[A07] 数字转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxycxnbde.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gonesafvo.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/guatmjdzg.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gejmitdtx.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjcrhwqo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqdacahm.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqfcnphc.sHtML

Ruby: 42.to_s
来源：http://blog.fanxiaobao.xyz/Article/details/gtgezrgfd.sHtML

C#:   42.ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnponslw.sHtML

[A08] 取整与四舍五入
来源：http://blog.fanxiaobao.xyz/Article/details/gslapqkua.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgpyzko.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwludmqvp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gehskfuuq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fanxiaobao.xyz/Article/details/gudttyama.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyzapzrm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmgovjgr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fanxiaobao.xyz/Article/details/ggyxhiqjw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gxdrkcxby.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gxekxkpjj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gddhbxddq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqkmeqwt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/geoumwmbf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkysnorbf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqxfnayp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fanxiaobao.xyz/Article/details/gxgzlvliz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fanxiaobao.xyz/Article/details/gacyutmem.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwvxucfh.sHtML

[A10] 生成随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gdsddqamh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fanxiaobao.xyz/Article/details/gvwxnihyd.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fanxiaobao.xyz/Article/details/gqewqpcdt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gijshainj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbbqiecy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnebxwex.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fanxiaobao.xyz/Article/details/gqjnkkily.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimxirzxh.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fanxiaobao.xyz/Article/details/gbwqjkbdh.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fanxiaobao.xyz/Article/details/grgugkfud.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gpfggiena.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkkgnkpj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gdnjxqmzs.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnubtfjlr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gosmydnsy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fanxiaobao.xyz/Article/details/gnsevydkj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gahzoovbx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gycifomrp.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gwvxzfzhe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grskakiur.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fanxiaobao.xyz/Article/details/guwahrbov.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoelmauw.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/ggbsteqsy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnozkkvxn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gskzjjhdp.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/gusdsayqu.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/glenwqnca.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvccwcqyj.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gyzoqhqeg.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/glhvxefgy.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkuacrxf.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gnnypacjf.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjevabxmh.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gixjvnpzy.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcespkgwm.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtenozofd.sHtML

[A14] 注释写法
来源：http://read.share.fanxiaobao.xyz/Article/details/guxiovbsd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fanxiaobao.xyz/Article/details/gejpqmjto.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gdllpkybd.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gqessibof.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gxvpydlyu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpziwfjy.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrzlbqsm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fanxiaobao.xyz/Article/details/gulvjnpqb.sHtML


<!-- 参考信息 -->