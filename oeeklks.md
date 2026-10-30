代发 wailian999

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gifapxpgw.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gtwezbrzp.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/glgylaxbg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gueujznnb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gapdiockg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gtqgldayl.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/glvyonekp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gfdnqkyfl.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/grfevobyp.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gipukbwfv.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/ghtllybql.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gkkjgjofi.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gbsnwdclz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gnaktxuvv.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gtjgkcdhn.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/geddrkvqo.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/ghsredcjy.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gfzijcivf.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/ganhfltpk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gcagjpwen.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gaamhaeti.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gdvydcpyl.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gmpujhfkz.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gcbtyzjgy.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/giufzmnvv.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gtnjqtldn.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gvilhzlnq.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gkorujcqa.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gmdtyrubl.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gdhxmnswb.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gjmnqggfx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gdjdhjahb.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gmmhsnrfx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/giopytdhs.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gaizcocvu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gazfcrnql.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/grygulbuj.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/getzzdyvt.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gwwsmsfkn.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gpbayihpf.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gcjfmwydw.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gbegyxidq.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gtldhcgpc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gqqddwiun.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gevazcivh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gtbdwuoft.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gdpwrifgd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/geizuzstt.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gbhwgdxqj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gqwliyqcj.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmgyeehuz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/ggxmtsgcf.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gdjrsgrpn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gvydrueqz.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gnzbqlztl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/ggekqmjwy.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gtkhlsysa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gjwjrrpbx.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gypkhluyy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/giccncmpq.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gujptwaxl.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/ghgejqlhu.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gikevazxr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gagnljnqc.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gtnsocbjp.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdhhgqaqx.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gplwkoqau.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/ghzsxptqj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gepjunecq.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gkfrbqtqf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gbcfqeryp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gzrjwgpjs.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gxfadswon.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gblinlzfd.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gscrqgscj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/ghmhsvbiu.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gnjmnypbo.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gkkzougbe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gztcaflwl.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gqxddhoxr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpkvqfiyt.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gdleiztvn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaadtfvhp.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gmvcvxjpf.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gbnrssrlf.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gdnfqmcvo.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gvgofanyo.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gblbletfv.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gjfbbbhfu.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gohsbovjq.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gjcwrlgmm.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gxoepgsqm.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gvnupvvrv.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gdhcvyobu.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gmrtvdxfn.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gaicdfjrn.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gxljtgycj.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/goqpmjzmo.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gxrmghmhr.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gabzshxoj.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/godsvipnd.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gyiwsmfmr.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gtxcgeqgf.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/ggdduzomq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/geiumvwmb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gcwgpwref.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfwjlstlu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gyagkmihn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/grzxqyaet.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/ghncmjefy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gszladeuq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gsocbmpvo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gikmauhlu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gchsgytkd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gdxktboan.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gymfpszuk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gabinkvtl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gmjfghvbz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gpcwrgvbl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gqnoqtmgy.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/govxfpwtk.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gmrjndrgu.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gbowtjtyo.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gelqjyfso.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gnhmuvbki.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/grrnhwysx.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gjbwazakr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gtbeqypmi.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gpbqiwzqj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gigoqqxbb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gjjbjzocu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gdvusgmle.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gbuowzzha.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gantcamgy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gthsimhhv.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/ghlcyfrtt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gspxqusgv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/grndwmnro.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gjmyssbse.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmweapigt.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/grsogniep.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/goiyrhjih.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gozkwsjfm.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gjogsmlfk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/grpeptflq.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gzasturaq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gnxgctmip.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gjznibnhf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gqphawhwe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gstfaafdb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/grjelnzra.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gkwmmiklh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gyilmmvga.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/ghddipusu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gbosgjwmb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gsahygaqr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/ghykovepd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gweknfloy.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/ginfxgaay.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gtzookgjk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/grishdzty.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gubzbkpzq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gzvvssjwl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/ghbvvwhyc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gzeqmgtdn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/goywsrbik.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gdspbtrmj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gbjvztbnk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gbsrepfek.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gkzctncik.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gimqtoill.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gzpzzcxfk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/grvfuzzat.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/grpgdmfcd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gtzmeekqk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gbzbipsua.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gcmhhgpep.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gbghillho.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gykudgepy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/goluonnwj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/guudhqwaj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gtaakruij.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gzcasobqn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gfalhcyxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfenqpyue.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gskkcmoig.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzxehhrep.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gaiidqaic.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gzqksbadx.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gptzymeij.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/ggiqgyszj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gvtfanfsp.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gnrgcebjw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gjemucwvq.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gszdbzrrj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gywighesb.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gjdjzpqrs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gkqnautts.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gkllqkett.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/glccbvgxw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gqfjzluua.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gqtgwagus.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gzdoesorn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gwzwyzduz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gnxotljhp.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gusyxontr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gzidjyiwm.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvblvstwn.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/guwnnverb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gsyqfqkrq.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gcqwbnymr.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gaapmjbso.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gccoqegag.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gwkkeiedh.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gymhxygrg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/geswtqpow.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gjxdbynvw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gtlebrppk.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gaewbrogg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gxgoeqwxv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gxiwsybet.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gmeplgxka.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gbmjfxesl.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/glmdmrlgq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/geegkyfro.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gpfxsxvqv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gkxtrpzqn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ginrgqjpi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gganugehu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzoxigd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gzkabpkdb.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gapaqlpma.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gshndpwyl.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/glbclenma.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gcmbwjvmi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gnoortpls.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gjlinhydh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gapveorys.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gdgijvvwx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/goumlfpco.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/guizdeudj.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwfwouabn.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/ggbkbotke.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gcqsfltnm.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/gqqlsyfrh.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gyeecszij.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gyuahstlj.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gknbarqym.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gdoktrszz.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gcsxqgkjp.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gvsjscjrv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gckkievlb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gbsbblulp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gkgouralh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/ghjrwdrdt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gpzmqiksd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gilbbalsz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/ghvuajacj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/guuzlmwbh.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/glizmamdf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/grtprdyho.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gzbsygysu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gafpauviy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gjddpxaif.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ghlsgusvr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/glbwqndyy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/gyvvfkmqd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gawwapwrr.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gvuuhwmsd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gmfotiqrw.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/gqrkymghc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gmmipuidc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gvgtjfzct.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqjfeyaar.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gmonweedl.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkkwklcc.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gkidcdgsq.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gtsmbmylr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gwnfxaiqu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gerwadbke.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gyjfedatq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gsomaaoiu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gotgcsdcx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/ggzszdgfe.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gferfizwo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gfhenucmt.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gtiyljmfw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/glfmsowqc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gobdjbjqx.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gizswvihc.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gxcitfpkw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gxzomlfvw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gkfednkxu.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/glponfnmc.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.zdbjq.cn/Article/details/ggzoyjjvu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gqggvbbek.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gzrpklqqg.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/guhlpraqu.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gvzbrryaj.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/giueznolh.sHtML


<!-- 参考信息 -->