代发 wailian999

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gpiiiqlqu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gpvsipnjv.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gmlkgbmkh.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gfayeafme.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gkdzhtbia.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ghlboqwby.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/glbupbzgn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gtojvwqyi.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gbfiwtfak.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gwjcujwkn.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gwjzsqcal.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gngagkymj.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/glueztjes.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gbgyxrbfp.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/grppymhon.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gmzyskjok.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gdoohhkfv.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gqqvwhrwp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gckdmhgvr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gsqhnoohu.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gtibpgqby.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gifnzlxvk.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gwmyoyhkd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gtivqnclk.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gntzwlhwr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gafiwthrr.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gvwayrysc.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/goaudppin.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gxhqplzle.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gujaqthpa.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gtccitfhw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gkwfxkvqa.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/garmezspn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gjgqunanp.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/guteilenn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gssgvtviy.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gxwhsdnxb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gioiznulz.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggbdbqaqi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gxicstvuc.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gwtkndmqa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gzovfbmls.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gfbnjxaia.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gusnuhgxu.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/guujmwxmd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gxswgwgam.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gooycxptl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gbxrhfbhq.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gkaowznjw.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gxlexbkpz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gpridcjxy.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/grbyjbvcx.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gjigprcsy.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gybspsfrs.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/ggqnsfqmo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbswzgfm.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gndbmekdn.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/guxpjnhwi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gxwncwfjl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gzajqjawu.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gnclbbbyh.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gybsoriza.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gfuqovpzs.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gbtlxtnqr.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gfnqydgal.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/glspjgjym.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gjmdeaehm.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/grpeojnnh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gonrnagmr.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/glhtclphl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbwlrlzdq.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gosrpuyky.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gahzipcsg.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gtzbrvnaj.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gczopmyzg.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gnnbvijzk.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/ggjbcpkkq.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gtnyugjtf.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gxsqkfite.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gzkgyreal.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/grjyjmfal.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gjwegkvqb.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gvqlzybor.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gwvihwqqm.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gloxaxksg.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gajgvsapt.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gdpspasjj.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gsmnlyeav.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gkuoaxyym.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/ggbbxcowq.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gqstkcwbx.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gdyqpmhzu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gqopppije.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gzilcozdn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gkwykrjve.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gfzwqeyfy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/goypygimf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gaoiouaoi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gylicyjtv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gznlntwip.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gjtgyritz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gbwlwtngy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gxzpzrahn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gpmcfrlyk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gaoxyytbw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gqtymmaxe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gbspozayy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxrfddoyg.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gzqeqxvqj.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gmwzfmqaq.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gcwabnmoy.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/glbaqsorf.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gunmfnfga.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/girjlfxet.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gpkcylcsg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gmacakobw.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gsgicztem.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gscyensrt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gyxvfdqrv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/grzamwuvp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gchqtuvol.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/ggpdzsykk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/glrggwxvm.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gkdihoang.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbqcvlsja.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gqgsjtjrk.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/glfvzmseq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkqhwhpqy.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gffqxvcdx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gkgpptcis.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/glzxajvcq.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gcucnwjur.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gcjsivtnr.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gzzobsqni.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gtitfrann.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gkqnmifrc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gvnhynzrk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gcujylfve.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gdgsvmftd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gbcdyryod.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gwehnfyin.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/guqentlta.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gbtbsaogk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gznlutmdv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gvtzurhhp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gkmlqbpao.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gtlgpqtni.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gbfhitgky.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gpwanvhet.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gfuspisxa.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmhhboiie.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gesbqjfhx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ghzxoofzs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gbqfkzfir.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gywuvnqua.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gaqcqsajw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gclgykaau.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzcrjvobf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gtaktzmxm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gonfoludm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gerfqfuhs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbkpbggit.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gbtyzevrq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gqjztlcgt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkjqbvwtu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gdasiryud.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gkcxylecd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/guqjmfrxd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/geaeamuqq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/goenmnocg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/garayzezo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/groeqfrhk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gagykvfjs.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gvbpwbzrh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnlbzjjyw.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gjurwsqiw.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gdhxxlaof.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gkmxwjdcp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gyajlbami.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gcxyorpxs.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gzpmqyscy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gqmlcrwly.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gxxbeifne.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gprueeuzw.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gieelyvqi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/glhnnjzxq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbbaschxb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ggyqdghtf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gdcrbgvlf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gmtcjwboi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gkzgafjnb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gvndgyder.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gbltsgdkk.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gumaaniee.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gijuziptf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gfmfzgeks.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gqowlrdda.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gfxticipq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfmxogjuv.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gxjzvcxja.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gosvlnjvi.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gsbqctsbr.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gzqramvgm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gtmjhyaie.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gegjalkbb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/ghodbrtfp.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gqiogfeff.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gppzocplo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gmxhlozop.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/ggnlnfzjy.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gpebapssk.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gkxcdjlsm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/guhicwzki.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gbeulloce.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gedkgxigq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gmlqonrvn.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/goquyjunl.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gkizzazkg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gstyhxixz.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gaoehsmbk.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gxuvmnktq.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gfpsnbfno.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gqhwbbqkt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gcqbtaevs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gizbjntwa.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gqhttfney.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gcsdolpov.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gzdxdvtpo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gvrekcwrn.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/glpevifqc.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/grgacvfjx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/ggfvrfucw.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gvbzxkyvt.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gnobivsrr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gwgkserpy.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gciacenwl.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gukgelvdm.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/gnkqjjrrp.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gjgaeuxsg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/glwakdobd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/glmgxptrj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gkqzrzjep.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gzdzhfigg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gojghueyu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/guevqqifa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gcffsoniu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gjvqpxqdl.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gvrcdazbx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gmbxxepto.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdtjobglj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gpgvadcle.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gwqqwtbkh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gvyrmrpdn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gvqujxucd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gjgnjzqaj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gldbbiykq.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gamrmmshe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gsvtufipy.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gwfowogmk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gbqdhntau.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gyytigpif.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/gintwuhji.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/guktatvye.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/goahpytym.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gudqdgezs.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gwsoyqvnb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gblpwzcjf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/godtgvyez.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gakygwkiz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gdcotbfze.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gpfsshzwl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gulbfmuhd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gblunhmua.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gayabzszk.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gdxphugrs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gzsbivqpo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.zdbjq.cn/Article/details/gulwnzrcp.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gfhswhtqe.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/grxhoutby.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/guoaqpeuv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gxojebknj.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gxbebgetr.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/gtsavfoqj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gyndeaidn.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gdwwttrun.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gbitymsga.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/giackspef.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gchbmqnlg.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gofyrvwcz.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gbddqwlkk.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gsysfbtgk.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/grpmohloe.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gzgdyblhu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/ghfpxlqcx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gtamcfjma.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gcpwjixrm.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gkwgeehyl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/geutnmhlm.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gepmlctzg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gbglotnmp.sHtML


<!-- 参考信息 -->