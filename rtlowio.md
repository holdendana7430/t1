代发 wailian999

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gcjouwlrr.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gpssyvjdn.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyqhqedj.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbnnhlfk.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwyxcntr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvoukykl.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcoopwxg.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbklifnqs.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gwxcrxoxp.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyvdvwcn.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/givkskpzs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/glkqgtzoi.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvlwwtbq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gnsrlvbue.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gvpaayltm.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrxypsjq.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdugyspzy.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaeqlluh.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmnzuxpy.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gbvbhjttt.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnrhhvt.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gtglawtow.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwfkyach.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvqchrjgy.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxhrzkif.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbyhmjyr.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gryhyooys.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxzygzyf.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gexsuoqji.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gxuvyzrzi.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjveljbxj.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/geyoxolot.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gansiattc.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/geajsqnsf.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/ggjavqxko.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/ggiwtsuei.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcualruf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gawrfegpf.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/ggkgpsmbd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicptpqtr.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gggozgrnt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gifdkgsrj.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gxpmnmwef.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gabvaflmo.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxozkvwt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvxpwpts.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiuwjcle.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gafbxljhr.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gcdunxnkq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gplcpqvzj.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gonxtggyg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqbdasme.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gvggfltgq.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gdynhkfva.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkpohzsw.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gbpiorvjx.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gqzboddrw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnzlffmm.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpbuyxzws.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gemzdkgip.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/geafpnkle.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrisoffw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpozrjqa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/grekekvzo.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gbiaxbjlp.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gcavrmyuf.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbtlqlnm.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqonfinc.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmomunqf.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gvoskxglx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/ggsvkrbdx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypeyqhut.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzltikec.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gkefuoefy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gydhvgehy.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqlelwy.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcpsuznv.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfwmvvxq.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gqfnqxumg.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gvgkhkwif.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbigoldr.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gfmkoivqb.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gsavdgddu.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gwppjprwn.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gbzbhsxda.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gihwwibkz.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gptosixui.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbaenire.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoxypcam.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gpyiruypd.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gkqmbhrbr.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/govwndyzr.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gyizompjb.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ghprdjqql.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/genfymxic.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/guwropngf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvykgkvdc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbqfutov.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnsfhzwa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgvavdqz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmvqnldl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyrvvvzs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopkwvoji.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/galzaodpi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gsegzelqi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkywjsai.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaewedrhz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gatmgkdku.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdukkshsn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gxekmmnyf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gujxbnbfm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhczemgj.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gadnobhwx.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheogdjmc.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbffhikoq.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/grservwdg.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxjmmqpl.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gooztfzjr.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gnblrlmps.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gpndpfxpc.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdyfrqi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/giptvghwz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/goeareeot.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaswtsqn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gsawigucy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gclcplajv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/geooyrtzk.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyhuopkd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpyglojwu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/grnssufqd.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gqewsdufg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhufbmmf.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/ghduylhuw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/guppscmnh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeincsyb.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gqhrqesce.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gnpjnmtrl.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnageozo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/ghllaaqdu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/ghjymxoey.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gcectgtxd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwutdhoe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gybrsxnxn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/glrodsfdh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gksezvpyx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gmhzifblq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfcuials.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncgswzza.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gulyvmswo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gmronozrb.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtsxytig.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/guzhzwdqt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhceihuw.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzobfrfd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpmwpiux.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzrsokmfs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrnzvhvs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteucndtl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqqeaaws.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnendnhvk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gidbacnqm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvvypahub.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffricbcb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/glkxjdgzw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpccihva.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glwkyjqtx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxpfopow.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzyikiomw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxicxkak.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gdcogwaxp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gaekhgsws.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxuzfcubh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gknlyxcaz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gyxzuwnlf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gatggpxyc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gijepktac.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqxvehni.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhpepixy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gewewetdc.sHtML

[A01] Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdmldbeja.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/goqurrawq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndleqcto.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gqoyjxdtv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fanxiaobao.xyz/Article/details/gmjugrfzc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwihbqkd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwkfhcok.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazexgaxe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/grhiksose.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/gexiuftop.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/gsobujjjt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnjlpqsp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gvvfpwkts.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gawphxwjx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gtzefvyco.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvfgzhwt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrqaphlp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmrgbxgv.sHtML

[A03] 常量定义
来源：http://3g.fanxiaobao.xyz/Article/details/gxxupvgme.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/garxqvhnn.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtrniiik.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gmgvjhtax.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwclnnlsq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvttkbvob.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvfsqdpl.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gksldbmsc.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghedbeohb.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gefvoebbo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gtvtwtwlz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcisxygvt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrnevfrb.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/glumdtwts.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gisodxqrd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslyoqbla.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/gayxjgipf.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/gzgbrpjni.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gdmidzdxe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gqdbxwknn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gagwwxsua.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/goebwulzv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfxpmktk.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gewzycuce.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gozkkyorf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/geedfmxxv.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecfnnvcy.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gnjgfikgn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmaodahp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gcyzmauti.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/ghwjzuddp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/guwphylcp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gghwpwaka.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/glknhmwxh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/gcryhxciy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gsrvcdoas.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhpqtzoa.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqnrwbzs.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fanxiaobao.xyz/Article/details/guzmismgk.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbwjmrpe.sHtML

TS:   String(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpqdrpor.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fanxiaobao.xyz/Article/details/guvawowxx.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlucukks.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/grmquorul.sHtML

C#:   42.ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyjhqmdu.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbgbbwat.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfyxvzcm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpslwyjeb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpfdqbbi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzfyqmnt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcpeftpx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gsmnfwtsl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbkgjlym.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gxcncxlah.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gmbuojgpy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggzyixnx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrpzctiv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvclvjso.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuvbzsvo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gulwbmhcu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkvlsvaa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbphkoxp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/geqneoygg.sHtML

[A10] 生成随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyfilxns.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fanxiaobao.xyz/Article/details/gvculpgab.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fanxiaobao.xyz/Article/details/gqtouajat.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnutedfwt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gjficxvvn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/ggavbcamf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fanxiaobao.xyz/Article/details/gcwtevpeb.sHtML

Ruby: rand(1..100)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfovjwep.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fanxiaobao.xyz/Article/details/gerszegqo.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjppbqgm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gscwkwdtq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwdxziwf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcpomimm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdyqklta.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gfdkbpspw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbvhxjeh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcbgjkyp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzxncwgt.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gwsooqpsd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gampchrac.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwmztflg.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoxgfzby.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/gcezkluwo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtawyedaa.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwnsxfog.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/gdsbyfysq.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghouhrgit.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwlrrhbh.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/goxhtjaso.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gyizpcopl.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcegnzlt.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbjxvgej.sHtML

Java: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gsezoiybv.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/ggrhiwnsi.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gkdcshydq.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gyoggrmmo.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdufzqr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fanxiaobao.xyz/Article/details/gkguwawee.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/ghzdmfgnz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmqdfnlu.sHtML


<!-- 参考信息 -->