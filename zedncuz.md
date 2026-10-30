代发 wailian999

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gjiwuicxm.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/grfzcldaw.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gddkpqtvb.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gmfxkytur.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gwijrergz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gchfcgkom.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gvqddtwgt.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gibfjznet.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gujbqwuwg.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/goidvitvf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gbpkqmhqu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gohibobdf.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gjagvtbxn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gvhzhejer.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gfxjqvuse.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gqbjifffn.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gpynylbee.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gqhhtkhgk.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gdhzwfvib.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gzowksogp.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gctswedow.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gniblwqph.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gsczlvbve.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/grzlnkmbc.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gmdtplpct.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxmkirvzb.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gkpeyhprh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/ghkggbzcw.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gitbfmqbr.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gttzhkwen.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gwicuoyev.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gwmkdofnc.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gpafxeryn.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gyobdebne.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gjznnacav.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gcizizpvk.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gliyypbcv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gaqffrhsd.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gisrfskfe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/glpnueebn.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gctnjrclw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/ggtcpzcfu.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gmseekdbk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gjknbppzi.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gdglalriv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gojajqrev.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/goxvlqvnv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gilqhialz.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gasiqalnp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gbmasbrjk.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gynaykwnv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gmopeowtl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gdqswdcbq.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gmduzfeur.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gvjlwiley.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gdagfsxlc.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gdcqqedwt.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghoekallu.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gxkmsdlbc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gbjqmwjmi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gsxjgovju.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/guvceyjrm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/ghgcxwzon.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gqhtvaupk.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gynyymymb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gburopxdd.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gragtwdej.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gqrwxmgsx.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gmilkwcmf.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gbvlxxcmz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gygfcyfna.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/ghawnuyfq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdaccyqnu.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gmmidrdlr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtqadwhhp.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gvufftjum.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gjizmwlds.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gpudyhmuf.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gwzkbugip.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/guckyaxuj.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gamywwhwv.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gpwsesmdb.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/genkgsicr.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gkvmgtssb.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/glbmsvstm.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gjtiurwma.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gljqotrlu.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gpcrekbfj.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gallnfgjv.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gbmdcxewn.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gucgyhzlk.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gabimpvlz.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gmjwkgzmj.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gltcsgszm.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gwbgchywx.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gcuppkarw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/grmspinvc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gikijzgfg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gjibgipam.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/grzvyphed.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gqdfwtrpj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gyogzapev.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjeglknkm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/ggbbmqhve.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwdhtlgzu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gpfzwfwbi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gnlpxlveo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/glkrlmkyc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gajitwkiu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gpssoylky.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gbvsaheni.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gdclmfmuh.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gikyvozyj.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gdlpzbpjv.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/glkdstkoi.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gtpuccylj.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gzntupsdl.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/glnsgdnrw.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gjiyieajb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvwwchozb.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gtletewcb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gbvbqfdja.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/govtkftau.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gzkuypjda.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gehxkwsqy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gpraskeqo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gzvgkvfxg.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gzorlrrdb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfbxzdxhz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gwldkqhib.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gkcpcubgj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grbbgtuir.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gkofpxfqs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gbiousngy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gduwkkodi.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gkwxkywsa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gdmjzbdbr.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gkdcojuqn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/goqigmwfm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gecomxivg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gpbmreoyo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gqsfbvndv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gdwkchess.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/grdeigdds.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gfcmgqqvp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gxhgfuyye.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gaufmyfbu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gtsfoypcy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gkemedurv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gojnuoolt.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gwbrsqkti.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gaocvopyw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gnusqlkue.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gnfaisqex.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzaeysxuc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/giomsxhbp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gjbpqdwsu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gdsyaoyvj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gqkwkhinn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gryevukok.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gadlxzsfe.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gvfokxeou.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gzzslpkxk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gppfqhqco.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyzpgqrqx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ggrovlfuv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gcqvlvlqf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/ggcrfvudx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/givdckjtd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gvjmharmj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gibehqmvu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gatwwvasn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gaayeceki.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gzbklorxh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gfbudakid.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjbzspdlx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gufkmlocs.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gqcfsshrv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtchnsfnr.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gdbphruoi.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gbrmaudkf.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gvirodzze.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gvaymcsvb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gbtbtcgrr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gpygpplqv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gwyhibabx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gpwfjwrvg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gfkbmguzd.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/glnmgubfp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/guaedlwoh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/glivmraof.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gjcoopeig.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gmkkwqjnk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gufecyyuh.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gvdusqkoy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gqynewwcv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/glngwwkxh.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gjkcfluix.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gdsngjhfp.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/geriwthvi.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/geltnkkbe.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvpmodxim.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gnhuydewr.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gmsdnbkgj.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/grmfbelut.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmckgunmx.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/guvtlkgxq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gomxaproy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/ghqndkdhw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gnclumuwa.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gzbeldsjw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gwcpogsfw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gklgkydmq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gqvtllibe.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gkaqszwlh.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gajpkzdxb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gsaaeyhfb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ghcqvmovg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/grtydpeoo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ggioqznzi.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxepujjvg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/giwqicmtu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gctozjgod.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/geevqqazn.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gsffcudtt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gvedndnfv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gmgoxnhfk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/ghtdnencv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gswodjjwf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gmvhbctay.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gyrhwhuhg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gpaclqhjl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/guqxiulnr.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gvgwuadku.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/ghbcvodwr.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gdqoxoxav.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gnxqjdaie.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gpedophgy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.hesvh.cn/Article/details/gjbrsvhgw.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/giaasmnnu.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gphoyfgwl.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gtglbbfma.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gbulirphb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/golytgynb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/goskuwuly.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gnvecsvjy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gbqllcexk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gixwnbolh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gmdrzyymt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/gimrqzizy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gitdrjpwp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gkbcfjhdr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gcysyctur.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/glmljmdbl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gulfcyztb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gnckftmin.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gbodhcpjo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gxzboqmwd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gauqcrfbg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/geddxhxye.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/golbblekr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/galqfqxvc.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/ggtybgonn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gwvkumjtr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/ggxmlsdwj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gichgwdeo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fehbvm.com/Article/details/gtlxnaxiu.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gxplcnles.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gvmlqvgzo.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gtzeyreqe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gaezfvxsv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gmrstitju.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gorpccesl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gxblnxgnw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/godyhccol.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gfzmkazpu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gimizvtsy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/glbatylyc.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gabpikyvs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gahoyjllo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gfbadzxac.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gjszhgcwi.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gpsmobtvf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gofmdvyja.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gyvuajown.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/goihuvska.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gawghdbxr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gprhbtbqz.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/ghzprvcua.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gfbygwgel.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gnhilhblr.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/ggbdfnblg.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gbpxyedbx.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gepfefwap.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gzbmzvlno.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gsqqafbgt.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/guppjoeow.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/goaizrxee.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gkfokbasn.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/grjgvugkf.sHtML


<!-- 参考信息 -->