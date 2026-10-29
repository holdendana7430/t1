代发 wailian999

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/ggsxstcee.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gjwrgfzom.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gizyakpad.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gihxmdzan.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gjfzqgdnc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gihkdiuvl.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gmeknccmt.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gshwqxpbp.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gkfwkusvj.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ggxumymxu.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gjizygdzm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gxnantjkc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gnzmxnlts.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gtcpvzbnt.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gomqvefxr.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/grgkmsbot.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gsklwirnd.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gshtuytsr.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/ghjzeqvcj.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gjkohgwpb.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gtdqupbnl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/ghapjhvei.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/giavffruq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gpmrdzqpx.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/giubwktyk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gsnmcjecw.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gptdgaaiu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gnxhqbtiv.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/glrjkuunh.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gohyfznvw.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gqiroqfcc.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gljcktcuh.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gdpgwtsdl.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gkkbkdewc.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gylmqwazl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gwjdubhpu.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gpdsaiwtz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/glniatnhv.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/grasqnmjs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gtuuiegsp.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gptxetrwm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/glczgjdhv.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gglirvhiv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gjuwgesqk.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gvhgvihwp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gzufnbmfm.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gznwaslpd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gybaijopx.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/giqkymqgf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/goxlbzbrh.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/geslzglyu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gtaktrvbm.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gefanljng.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/ggxqvfcrc.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gjzlliqbt.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/giyjfcsbu.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gdueotjuk.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gddfwtupr.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gsswkevql.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gwgaokxxd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/ghislzzbi.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gcfyfmdjg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/glzyntffn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gkliriqbs.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gzrbfuwiq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gefmtionb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gzgzvyvpr.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gyrikiebv.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/ghohrjegs.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gktpygljn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gjihjybrn.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gvupyqein.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbzwqzwjl.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/ghwjqnlhc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfzemwthq.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gyhncrgpj.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gujjomyea.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gibmbtzkk.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gnplsexzd.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gcfttqolg.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/ghhqotfeb.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gsmzntxjh.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gzgvgcswy.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gpvxrikah.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gxfbrpbzk.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gtvkogmws.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gaxjmeikx.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gvdgnxnyn.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/grjipiomp.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gtndajzdn.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/ghvfhsghg.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gszgqhujf.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gxlmhnefx.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/glddcbvjr.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/glwmaxovb.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gdqxegwbz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gisloyybm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwrrigfba.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gjlgofzun.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gkvgleggp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/ghxsaszac.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gjmhociao.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gizkaxygj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gkhjvmcbf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gbqjatpmk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gqvmqqcvn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gykipxfpr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gcsocndhv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gtttwmcww.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/grvxahpoo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gquoounhx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gyttqwwdt.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/glwunegxd.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gqanxezlc.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gdzkeiitz.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gecgzjemf.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gquvxvrnx.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gfgctozcw.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gpenpghek.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvixgzhmv.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gimqgulfz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gvfdlapyg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gkcvwufcg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gcuynammd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/glaevsufo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gsxqsxgng.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gakmmtgmc.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gdnpfcdop.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtpmrcxpq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gbshqrbya.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gukfrotnq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbfoawhga.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gxfknlqfz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gckwrgaqs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gmtqvgchf.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gdmwjlghe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gjbadrbke.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gbfipumpl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gztiwctdj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gqetbgjgz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gyaaclcca.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/ggukmmlgy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gjuppkndl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gnrehlmou.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gjumoyriu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gldkuawwl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gmowxlhys.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gupfviqag.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gcmjcqzby.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/geqreepcz.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/glpkelolr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/glhcuurqp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/geicrsjhl.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gibczceld.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grevqnmgf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gwkjvmznr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gtglscxbg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gadqeueuf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gdiewktbz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gvsumeysv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gtywytrdo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/giikdetmo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gwwjizjbg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gsjzshjgs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gsdedodbx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gpwracijj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gbnyqhepz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gfzpeayla.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtylowvul.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gccozrucn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gzeyrdhic.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/guivsmayo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gpwpeidvj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbiskuqpn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gktxaazsa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gsapmxwol.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnweglltu.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gcuqdlzeq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gojwboqjw.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gincqbuba.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/ghgioyzti.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gwrquayqe.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ggzghnxmt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gcxyfgzix.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/glzunxwok.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gfhickshe.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gazquzhad.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gaxklecxd.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gubtyzdiv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gbbgzblyy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/ggqhygaug.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gcsgtvawc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gqmsuuzmq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/ghtribgpz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gtfkguqvz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gnefyljwr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gpmndopfo.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gzyflklyc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/giwomkepc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxanjnlri.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmlzqmuhv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gtjbgruho.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggfnemhtk.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gjfepqdwv.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/ghmwvmdtw.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjqnygfcj.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gamwylmip.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gmvuextgi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gdzjuxbpl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gsjayxkdr.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/guyzmsndt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gzmbuaxoa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/goltvmhuz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gnocqbxjh.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/ggxkrdylv.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gwtxvxbps.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gcgqvdahe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gxoamhzcl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gvyuvdbwo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gmkpfaett.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gazpbrftc.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gfajzazwp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ghkbmijph.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/godkeuqwp.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gtaiwjacv.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gwozzwacn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gapnfrckc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/ghbsispxm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/grerhfogn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gphmsnhym.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gtspphyoj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gkrzhgdvs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gsoqauxqe.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gnmqmveyu.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gteilrnvt.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/girejvdir.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmrvvzhbr.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/gfphwtgoi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gcwtidepw.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/giaqlflcl.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gqxvoorgu.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/grgugdjax.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gayqgpuif.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gejsgeoij.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gamaiqzdt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gfgqveuoo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gobenhamk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gdohdwxvw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gynertbiq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gdkqtegha.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gpnsndvua.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gsizhdylo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gxsyzewhg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gnifgpzpz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcbvfeaey.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gbxfcvcqb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gdaqkrdjm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/glmrtggxi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gbamspigf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnthuohng.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gzatyyrxh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gfcewpjco.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gwmscvyef.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gssatdaep.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/ghgdbrfct.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/gdrcgoevq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gjxznvduv.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gcdsrgobg.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gsyfqdyen.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/guhivdwlo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/guosxvnqy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gmsthxmqv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gswpysqzm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/grvujljmd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ghryajhcf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gqvzavxgh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gieqghukv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gxyiieqzh.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/gvorntrbm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gzjkhhesx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/giycxyhkx.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gssypnhcm.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gojgzrzwa.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gfjkgexvi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gavvsaind.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/ghlvqeslc.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/glambbujy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/ggvoiwzso.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gjngtdvne.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gczzdwdjc.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gfuzpmtyb.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gksvkmskz.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/glgelxjhz.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gubvsdcxy.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gdmzmclsm.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gdbyvpyhu.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gfreczeaw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/giwditvke.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gzuiqmdmt.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gptdoyamt.sHtML


<!-- 参考信息 -->