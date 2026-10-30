代发 wailian999

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/ghcqpylzk.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gtspcgndt.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gkrhcyexb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gepaqetky.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gobxyocmk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gysqpfawg.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gicitcldc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gszrswiry.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gbshwnxmj.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gqndeuvyy.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gvznnisae.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gcynrxoeh.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gwbfhyquz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gnekbwguf.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gmcgtpnpo.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gjnaaexbl.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gxjpyltxj.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gjtqebpox.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/grriborcb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gwrujwujy.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/grvtqsqje.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gzaensdcf.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gajtruxza.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/grnhqutkg.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gwksnftdq.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gccpgmtcw.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/guybnletl.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gsofzfbbw.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gfrchzdrq.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/ggirjibke.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gxwfhgcbw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gvxpjrelh.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/guycmostp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ggmysaxfs.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gfruwxnkr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gpvejozgg.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gsmqbbhws.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/grpyhogkw.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gvdkxzpob.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gxscjppcb.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gicynhkvj.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gjcyztjqw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gprsslcau.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gqlbpaxem.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gszgbenau.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gdtqrnnzp.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gyhhjgbvj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gixrgeqth.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gjrlvuebl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gimtnilvd.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gvqfyvhtv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/geghmvoyn.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gfphpvayw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gjygyijoe.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gmqldcjmh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gbquzlzyr.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gbhwuaiwk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkbqqqlk.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gtgdydcbj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gxokevbja.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gjvlwzcgr.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gpwxgszls.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gxabnkywi.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gchsvxwsf.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/glonqbget.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gsodtczti.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gpkuqlweu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gxsxoaqli.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/grztdlnpo.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gddxlwrpi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/goipcwdts.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/giuzsriwc.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/goukpjndc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gbsejxjmv.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gcgsxnxzb.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gkdjfbewe.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gidzdahkd.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gdnhzixdp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gzyqcdnab.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gchpklhqj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsbslopyj.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gvzrocrqn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkbqxtmcn.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gsaakaqmj.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gqjflmnvd.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gksinccuc.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gpvhntsmu.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gugzhfysd.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gphlfovjo.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gnfnaphlf.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/ghcslkhgq.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gcwabjlbx.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gbpfyvhhj.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gdghbzapj.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gmjgtxeyj.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gnzvokczf.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gdkpjogrl.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gpbyettxo.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gnlnlrefe.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/ggykrdmoh.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gagwsidrr.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gyqcwgobm.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/ggfodmfsm.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gtktbyrtk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gzhdwstxx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/geseryxmv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/ggtqfflvs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gxojyiupu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gwxmhwmmh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gqwtjosvz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gyhiojtwt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gvyjqhyff.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ggrpyfyat.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gtagibhvy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gouwengbr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gsdwugfax.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gpxmptzua.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/ghzdayfaa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gftwilyzp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gfiewekem.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/glakvwhua.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/goyphadyc.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gpjtqokvr.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gnafciqmb.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gmacymlga.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gwvcdmvnq.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/ggzommjzk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gynhcitol.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gjlfmxauj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbzqeuiui.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gpjajxrwb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gcphupeij.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gbmnibxee.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gpsunyxdx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gzwhxqfta.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gdftprerc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gebrsyhco.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gsxyplnoi.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/giyzhsqub.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggbqudwxf.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/ganulgqho.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gwfikyecu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gdraueegv.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gbtssnkvo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/ggmkwqzsj.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/glkwakmvy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gcorswhli.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/ggjypdhwv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gqaeiimvl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gfahhajpg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gsjfzaqxk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gaubkgsnk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gdpfbacwb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gocbmnhqb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/ggabzkuky.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/geowndufk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gderhywmt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gfdbozbkl.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/grzsnjprv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gdrtyhtgk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gnboiumch.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/ghymrbgak.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gmgrwuplx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/grfcwlnzy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/guhpefjdh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gjkxoumhd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gdmqthkqn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gvqgyxgpv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gcuyqnqrw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gfkbvyqrj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gidkjieyp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/grkglrtra.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gkbxdopkr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gpqrffgfd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/guvtnzjky.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gdzxklgty.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gvehsvrya.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghvvaegob.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjyogsryv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/guwoqlsak.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfrrvtzvb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gxhinembp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gluolovjo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gujpjjwze.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giubdajun.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gprwdohef.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gftkvzzqu.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gargvghix.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/ggpskbcpk.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gfgnekwip.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/guhlvpozu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gzmdzmalo.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/ggntjzxzk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gnuzcjdsc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/ghjcpzvqr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/guiefttha.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gascobrdk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gtimchsuq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gelewfrpc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/grpwjcqvx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gvthvslnu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gwuvoffky.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gpiyzkzsa.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gpvkoknay.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/grtpgzapo.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gzdwawhoz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gfssybdmc.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gddkfixwb.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzuwagswe.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gsuvnvctx.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gijwasjnd.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/ggrtiiwvj.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gybtlkyak.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gojtqbkby.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gkbxwpdpy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gcmcyldxw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gxleogqet.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gofeumtop.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gultuvnul.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gsqdyxboj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/grawlkoza.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gmpajnnyd.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/giyousglj.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gvazmtfhs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/glyjrahyk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gkzoepqkv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gynvktxlm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gbnqavxrd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gdaxyqzfk.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gpfscyokw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gcpyupxju.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gwxfqydlb.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/galyundpt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gwbndmnrd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/ghsxufwzm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gncjauckx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/galenkwbz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gimfxyhkx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gnltkcdco.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gcriyylpb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/ghgyzsdro.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnxscdbqh.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gextayymd.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/gudjkbnlv.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gnzorqfbc.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/guecqxeez.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gcoftroam.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gnkxbqvnj.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gbdzcwyag.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gbmojcwbp.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gbeairydu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gjrpaadiq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gknhkpdxq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gtozzgigr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/glgghntyx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gsdzulvfh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gnvrwwwua.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gnoakqfte.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/ghjucwakq.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gxkzfbkml.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfesidmua.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gkkalnqrh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvvrbicch.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gcxksgifa.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gwtjqoyos.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gkxzzexgw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/godbclaaw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/glcbepkum.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gztqfgcpu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gepqlaumm.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gkzvtkefz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gbrsbscmc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gebcbrppf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gatsyfbrp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gprskdiwb.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gqzcovqey.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gwaaokton.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gqxshmqfy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gwnrtttor.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gztvtybny.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gtqzqmbxf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gfeezbyyk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/ggoutbmzz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gzfxtrauj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/ggoksthyc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gzgeagvlz.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gtyonoetg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gtfpbeils.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gvbjcnxlp.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/ghxdlznnu.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gxixnolpl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gujnquejd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gvwzapdvk.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gklbaiitz.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/gpcablkda.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gtntuhonj.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gbolkzalz.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gjqsdmpsg.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gkzmiqbhp.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gldvvdkwg.sHtML


<!-- 参考信息 -->