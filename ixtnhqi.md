代发 wailian999

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/ghplzazfv.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/ggebdhrgl.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gaxcbqdeb.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gvhkpvzro.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gqrducauh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gtzoobjks.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gssfjflpy.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gcdkxxmqu.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gwdwjsnbr.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gtueqbtwr.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gzgfunmin.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ggiyuttvz.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gwnibiiew.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gykknsvsu.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gknbzkjgt.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gfemfycrn.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gxxenrezm.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gaphleboc.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gnezuxpay.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gqlnypmrj.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gmwgyjnvu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/geieedcqi.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gogvennoi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gdntwvrgn.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/ghnadlwdm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gmiznabgn.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gguufeium.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gyrqvqarw.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gcjkyomfc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gluhsktfb.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gadvcvxru.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gmmaffpll.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gbvkpwxiy.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gwlaescjl.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/guinqymto.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gumyhigxx.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gqprpcbgq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gwoeyrskd.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gyricnreu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmuooolxg.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gqubyyeoq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/geoezswjw.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/geaonmnbv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gssexsjsd.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gllfxdkit.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gfttffmwk.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gmkhuvhmo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gckddrcqm.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gpozvwzft.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gclixopqo.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gzanhtqag.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gkhzdsjso.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gvlzotzvf.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gkuqxxibp.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gvrqceytq.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/giflgmcpu.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gkmqsaaro.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gytdadwnw.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gcjacjdtk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gbzbbxjzp.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gftzstuer.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/grqlosjjj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gejogtwcz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/guinqseop.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gxecooyaw.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/glhhdcsyg.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gejfswaty.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gjxqastlo.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gazsxgwmt.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gmdkcccbp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gmjrjikmf.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gdqcixfmf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbbwuqbqj.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gktccxpej.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdkqnhxzz.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gihojqyub.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gxxlwztny.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gtrrrkita.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwdkzdj.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gekdjfmhh.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/ggzheghlm.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gkaymufkh.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gsskrbgxx.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gofyarlyr.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gugowpyks.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gtyikpmtv.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gpetrxaou.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/ghixexjon.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gedslnzxk.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gmymwybic.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gofylejcg.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gfyctcevv.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gzbiwlssb.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gcadwuyeh.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gvfmyugkn.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gwdftieyy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gsymdhqxb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gvmtbnekn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gyckmyrjr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gcjkpmnko.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gimklrvev.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gfqozhzct.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gclaxjyhd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gmdoznabx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gftomnjtd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gjcypahax.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gzzcakiol.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gbbkcczti.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gevgogwvn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/galqiohzf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/ghzxvfoap.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/grpmlpjpf.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/grkkvdtmb.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/goeyarpam.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gzkgmhvvh.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gllospmho.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gkiguctop.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gebfzgefn.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gqwdlnien.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gabtmgghc.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gabmvnvhc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvhclvooc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gxvesgali.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gtqgpqxpy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gscxewght.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/grlhwguiu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gabdfpdjg.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gyxdrswun.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdwgcnazt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gqmphggsi.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gnwqubiul.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpslqhkke.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gwsolwkqv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gxafpzdxc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gvjlbdyka.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/ghkdguvbq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gkierbbra.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gfzhzokdb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/geffnynsr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/guimxdpuq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gnfpfffvm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gluoxmret.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gxbyaexpc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gimeeyxgt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gvbkynplq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gkhuathqq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gtqcxsouy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gtmglspdv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gtbpuozhm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gkewgtqhb.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gqgbtskig.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gmemwrook.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/grlhjingk.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gxodpzzgd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gnbrsorjn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/ghppgcnia.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvjhimala.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/garhodrap.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gyxwefjaj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/goxzcpykg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gqirimojk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gojxeevmv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gxpkhwwpx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gudfhhykp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gfaotfgch.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gjvawpriw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gjwaradrl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gzqivwwad.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/grpfbhrpu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gyqxvedcw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gsnqlrznw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gliirrggl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gutjozcrn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gukqjwers.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/geieaylhz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gaepoosce.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcdpduzxg.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/ggnqllidm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcpupkfxm.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjnybthdh.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gnbreidbq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gpsunjwnw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gsaiervct.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gmlxpeqjh.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gztfateym.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gfatuprcz.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gqzoaoxem.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gkatxjqhs.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gnjahyyov.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gtlhkhfin.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gvfefudhh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gfbibqghi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gsxgdqovq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gwvedizqz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gzppozpio.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/glwactvue.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gugqmntky.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gtsmaeyin.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gbtcgpsbp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkjuseqev.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtjrulmyu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/guhgvaeoc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gldgesljz.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gqcgwrxjy.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gfcyarpym.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gvqjfffkg.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gxvqgcrnp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gbyfyggdj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/gpznvwdkk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gubnkpbgt.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gjaqcdhhd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/ghkcqbmhk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gmautstng.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gsocxmzjp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gbdpbiajw.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gpbertwwx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gyamcxsad.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gkmgbmbpm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/grhduijfx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gbxnbmevp.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gociydxtr.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwrgitihr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/geufktltn.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gbsxpoegv.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gfnqniuvx.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/ghoosomvo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gixfashii.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/grvhdheoi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gfvfucdyz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gqnmfiwkh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gboqronle.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gawgmixxy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gprrdxius.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gfarmjfmb.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/ggbdogfza.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gkqsdjpes.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gudjmmqco.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/grtgcodfo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gunykxogb.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gjwqlbxxb.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gshgplvbs.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/gdpuuzdir.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/grinaqfpr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gcszyjzvy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gcywjopaz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gsthzjsyc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/giqibwtrg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gppqrsguv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gleoljjld.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gjtnevqxy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gjpecromc.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gveuhfzva.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gehfsquki.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gqcnbrnoq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gackcvvyl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gqlzyybhf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gsjqmailz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/geqxnpnyp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gcapgyncn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gcqburldd.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gfyxwgajl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gdakunkrx.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/gkwxqlkvi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gfqvaovkz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gtvqfdfkl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gvmwzzqwc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/gyotlsszi.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/glpragzpb.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gqlzndmmv.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gqmnwtqgo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gwgqlajvj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gbimrelby.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gqymofyyq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gvtujoufx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gtkkqdjvx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gypkgixme.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gipbfsjkc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gdzhsifvk.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/ghzobjsyf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fehbvm.com/Article/details/gatuwjfzs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/gzyqycaew.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gyxqskypv.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gjrhkmuli.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gsqogioai.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfvgcginr.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gnkcxeexc.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gvxgpwvkr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gsdnvmtqx.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gcfkkrshs.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gffbglhzv.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gssowppup.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/galhkdcvj.sHtML

Java: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gwjrzywnl.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gryqiiorr.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gnjmcpegb.sHtML

C#:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/guwjxbqhb.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/gbdxfoeuy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/giseywilw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gbvynhdxy.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gzldmkrhk.sHtML


<!-- 参考信息 -->