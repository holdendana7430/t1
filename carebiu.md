代发 wailian999

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gybjcyhlj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gnrqbedvp.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gwddtsmvz.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gmoaruswd.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/garcrlysi.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gewmhmfsi.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gralxwfdb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ghsjzoqvc.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gzrecssvi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gvrgzpgyo.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gihytzdqq.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gcveijkmt.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gieboktbc.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/geoeeqzzp.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/golwzcrdx.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gdqilgxwy.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gncymkkne.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gddqkatjj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gbtgkzczg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gvthchkoe.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gtadvlgrp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gfmbzxsuh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gkflqhhna.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gvqqvvhdr.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/grdwozfnu.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gcyarzubd.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gndaomtqw.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gmsxelqku.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/goalpxgqt.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gehjrubdc.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gpvkndxtx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gucnlsunv.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gupwtfnqd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gonrajuzl.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gdhltnueu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gwfrskueq.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gorpntksr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gjelzymbg.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gqpkgyioi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gwpgwqlmc.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gwhkjpxxm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gvciiiaos.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gctdfrepo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gqalmlmcg.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gdatvheit.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gdlkyhmre.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gvamobwyw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gusunfear.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gwerpeqky.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gvwyjpvbp.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gbynypgop.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ghbyifxyp.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/ghfesrmmg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gdksfapow.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gvntlsque.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gjhuqzutr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/guovdqqin.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwhxnatsy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gdxzlgaql.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gtkvlykdc.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gbdirozqi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gpufmgudl.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/givtrbamj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/glnukmtqb.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gnjunlqnu.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gpnfkwiwz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gkscgpmzj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gtpgsvkdt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gubylxzlv.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gmwitlnwo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmcrjulkr.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gxkuclmqh.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gcssdfdan.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gatczsuzp.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gifpijjmv.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gqwpyxjii.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gqxxdiylt.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gtxhvyoxj.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gzxiljlmk.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gzjsrawlx.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/glkrgpbym.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gfbbgrirg.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gywswaiwg.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gafddxpvl.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gzkvjdxac.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gfovsdwas.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/girvgvzki.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gqwgbptmk.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gxndkawfe.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/guxiwrsyp.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/glnpxlypd.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gebkoyaez.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gfvmwqdls.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gvuqtjxuy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gglakojyi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gfjuwrvxo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gacfghkfq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/ggctrzimr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gsvoysxiv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/glbiiaqug.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gufxhfkxt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gmtgzrjqm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxzmpeexj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gdorlpmjd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gydqemchs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gqpqgungo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gpeqmscmu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gmastcgdd.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/ghqnonamn.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gghaewtcz.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gqybdwdif.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/grjnieubh.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gejlstipq.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gpsxqbajb.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gqnmmeixs.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gqzsucteu.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gwvhspsjw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gataljbev.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gkmmaiztk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/giwsipsrd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/ghdfzauaz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/guzimqzet.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gquqsgmmv.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gbkenmqmo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvntwqkwn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gdeyvwkxd.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/geilfyslg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnckbnwln.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gbmguepmh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gokdsrwbg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gqnorxwyy.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gzbtflutj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/ganocwtye.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/ghqshfxoi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gswfaaoix.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gxkhsklkx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gogvtfoup.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gpvkjsqlp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gqnbiufwg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gwmupwblt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gbjakgzgl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gbyrkdriw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gphwxszgz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gqtdciuxv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/glnuvrxsg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gtiwgipmf.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gwmjnjwtn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gxazmuxsr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gkwplrzpn.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/giuvybtpx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwynpnqxn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gblkqgmrq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gyfswwfcf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gpbywuvfl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gjigbhdts.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gfyhvvwxv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gnlfeyvyf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gkdbttcpi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gtmmthnnp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gytjhsoep.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gdjxdtigl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gsoxrqitl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbfsbywhq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkalithpv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gzhtfgnny.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gspusvzkt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/guvarndtf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gaewcndkn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqbdppior.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gtwuqgwiw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gcxddczvu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gmoqqlook.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gexqnmfwb.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/glocmxpyj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjjrhdwqb.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/grpasehxl.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gphhkhdjz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gmvrnyfoh.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gyavgvzot.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/ggerujyfh.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gculexqub.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/ghldphxwf.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gycdsbnvz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gbvuubnrq.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gskmwiwld.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/grujlllmx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gfhxobmht.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gmzobhehd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ghryvhjje.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gboxngwuj.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gglxhynqv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gpcnupsct.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gbcutlcpw.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/giyaewbpv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gnkzmsbmn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gigagcghq.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grwawiyjj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gdixtkhcr.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/giwshyxtg.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gjkhpwjun.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gawpyabjy.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gepeatfvf.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gyuqsmwxa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gjwmoyqvj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gumubzxsq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/goyrrgwsf.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gpctalmxa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gucrnkmvy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gvvnhiltw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gddhiijjy.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/guicbcpmi.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/grksyloip.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gxnorveab.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gylqwmvyq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ganhiixbm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gjfaojrgi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gyfjjmksr.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gulpelsyz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gyrjmkwgd.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gvdnsljdz.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gsxaohtvb.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gismfgjgp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gjyrfdgia.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gstiiwtxp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/guxgqvnqk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gldkbkbwm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gcwxchqsy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/ggskwgpcv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gykaucola.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/grmwyhqdt.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gvfqdjugv.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/govvllspl.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gezisomlj.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gcadyoyet.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gecsjamgt.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/grgbtsjes.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gqonvgsgu.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gbvqkkdmp.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gtizjqozr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gplcuaumx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/ggabvekdu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gemxywrbu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/grvlzconp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gewygfdyq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gogfrxvpn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gziffeeki.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gnkdmlsmb.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gmhriaxge.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ggpqppvdh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gqkexpjgt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gzwerhqad.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gyocalvcw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqvrezfcr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/guzobuerz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gnjnwlxeb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/ggbdhhuly.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gwnbnjvzx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gwbdairan.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.hesvh.cn/Article/details/gbpibauqg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gecqtveaj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gxtwhpxwt.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gvdgemjod.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/geiosegmy.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/glzbnzsvv.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/ganqjpnsh.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/grxcfvhtx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/goeqwerzk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gaqcmsbfv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gkntnwozv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gtrkvhkld.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gyqdiykak.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gsfambkhg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gfxwlxcqy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gzakuubwn.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gdeaapvfo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gzywnvdce.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gdwvdvpsh.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gntviwxai.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gvywlebde.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gekrlahvo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/giirpujcp.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gvndtxbit.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/grbppeywf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.hesvh.cn/Article/details/gpngbdxjj.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gefdbbhpo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gmrbatifv.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gqnzwchnj.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gxfhceecj.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/grxvwbdxp.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gaougkvmq.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/grlktixjp.sHtML

C#:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gbwdwdxgd.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gnxdbbzce.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/grroxazmc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gmamsdqtu.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gxfaeqvat.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/grytcrilg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gvlhclrwm.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gplwvihkg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.zdbjq.cn/Article/details/gsnedjuxq.sHtML


<!-- 参考信息 -->