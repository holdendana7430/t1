代发 wailian999

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gnasxvoyz.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gzatageib.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gcbrhdlkj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gifuhmynw.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gxmovaeue.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gvknxwvzj.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gzwyoehdc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/ganukemcj.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gpqsneflv.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gfwyqqxkm.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/guctvcmwp.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gnmeydrfw.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gqgntletx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gycgtopbu.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gqfrsvfzi.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gsajbfajx.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gxboktdjc.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gumxclxzy.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gnfivyqay.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gtcrbwimj.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/ggogklnch.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gualfepzo.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gdjyiihnu.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/goxjhwahz.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gcvevmezo.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gpmuulxeq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnjkkxfvy.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gaanomcil.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gnrbqalqb.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gmvnjfrct.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gijmhwbvz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gnvsbfedm.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/glutgfxnn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gvzslzkjk.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gnmfvxzpq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gnowxzggc.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gbarqmkin.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gyepxrhdr.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gzowyowyh.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gvgtuorcv.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gvslulkiz.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gvufgbuzc.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gunqkwfnl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/grdbhxzmj.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gxrtnbuaa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gwzfqxwxe.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/glqbfthlj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gqopsjrdf.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/glmwuckqs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvhbkglwh.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gutnumjpo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gpzyzaaah.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/groqqwugt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gpkmgrkus.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gndzkipbw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gbnkddphg.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gmqjujcce.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/giluliqiv.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/goqczmhkg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gzvigvttp.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gmjyhbygx.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/guktfrycr.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gomcdqjxj.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gpoqxntpc.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gqygssuls.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gfthfndvh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gbkquyvvb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gjhaxbrpr.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gtzdeyyrd.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/guavyirjo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gelksykeo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/guwurcrmc.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gscpwvfby.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/glkwabins.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gnbnwbxys.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gboxybnkc.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gzalgaoyf.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gdikmehde.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/grjtylmza.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gfokhjgsu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwczqvbbm.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gebvclyqi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkjziuslf.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gtkfypesy.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gfpwillzn.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gjmkaqwru.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gmfgrnbjs.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gqzttdshz.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gurwwyfon.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gteeraghx.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/grxqtmiii.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gbzoxuvfb.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gmwwtwxim.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gcismpyrt.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/ggnajpfrm.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gkjtzhowp.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/glfjpsstn.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gszxlfnfz.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gbvvuzgwb.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/goklozpim.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/galogette.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gsxbgdcpm.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gskbdqhlr.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gmmaqvnkc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/goohyfbbi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gvjsnddxk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gwbtddfqk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gdrmpkonc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gdoihzcnh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gmxzlsiuq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gpzzgkiph.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gdjtdjmvt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gxubysufp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gykpffeos.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ggfmhqguz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gtxuiatjn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gpeagenrd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gfsooipqq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/ggtaceusn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwowonesd.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gfmfheene.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gvuvkwmyo.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gsqnlzfbo.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gngndksxa.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/guqcuptjf.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gcperzzsa.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gznqmgume.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gelimuuhh.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/glbvqrtcx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gbkbahgmm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/giajvdxbu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gbdeqcrdl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gopfsjxxw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gcvtjodsk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gbxiluenf.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gvlpqzefz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grlftebzb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gdgcbphyf.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gbgdetyyh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvqaegthb.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gdgiiwltm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gilmiebde.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gexmegnbs.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/guwsdhrgo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gfsthqmxj.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gbrosfdlf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gqngbuyou.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gfnjuqilv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gonshanan.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/ggfsfdqft.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gdttiprdt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gzvqexkpi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gmnpnrtsx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/grgocjgkl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gqkoqpvtr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/ghgmuhbxb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gsfdrldnb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/galxepmud.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/giwbpcwxa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gxnschnbd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/glkqpytbl.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gmorylqjz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gessypufc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/guozndqha.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gpoipjvqo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwpwrcgkv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/glrvtfnvj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/goyektofx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gsjybtjjd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxderqduy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/guybqqdlm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gkabfiqrc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gttnyhuwj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gtqzxrcgt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkmrwnetq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gefgdwwja.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxabladah.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gctcgsbke.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gxhfzksku.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/groitoepf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gqpilxcbu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxllilood.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gbtcewwqa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gxnkuwrtv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gskocmkkc.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/ggcmztqyf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtynnhccb.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvdhpqeat.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gcgnqgwua.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gqitkbuzj.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gsncujxww.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gzoanhdad.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gunikhqir.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gufgpeeww.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gaxkleprq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gxvgxdktv.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgfyhet.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gunmshxaf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gtzukwzus.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ghfoiqreq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gtsebmeuf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gamsbiojz.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gtlzjqdlv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/guyecnvvh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gxeijlkxr.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gswqnzsan.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gsoyoabuj.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gtvxmsfgs.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkreljmrc.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gbolvzsul.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gsjihbimw.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gusggryjs.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gdujrgnkd.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gimllzema.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/grobkjwov.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gkskgnivk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gwblrotzo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gmsfkmeok.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gywadojeo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gtmvyihde.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/giiljcosc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gzkulvzzc.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gatzvidqm.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gosyrklbm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gvxwhyclq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gksjkrwdz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gowjaiefd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/grcvqppjr.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gqpjfnucr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gcuscpvwl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gzhfqxtfr.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gfchbspwj.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gvzqiecie.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gekusgfja.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gshtizkzb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gfbcixcfo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gcszzhudj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gqmrngqye.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gamfsucep.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gnvbrsymo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gkncjjokm.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gugosawsp.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gnagnsoig.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gobvzkick.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gkrymrbnu.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gasntmqlp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gxjuqcfxl.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkxlaapd.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/glibrcxgk.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gfykywzod.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gqtepqcqi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gwginjusa.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gchhtsijk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gpvihcgjf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gzdqtipla.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gjsnunnum.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gdqkobykn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/guhnqghqd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gzonftvxn.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gukmccydh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gvwayszqt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/goadrifci.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsvgkbwav.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gekvnixlv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gushdvxmf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gxcboslmm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gcfavemeo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwvfblinv.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gsnxrmrez.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/grmoshvmm.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gfwrhcvgi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gikufdsjm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/glmoixmen.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gxycqleky.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gpihlacxa.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/glefyoxpq.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gptwobsif.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gkqxfkkcn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/gbofydqev.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gkcghnkxl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gkwihvilo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ganpvuatk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gqmhydifo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gztmezrux.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/glrxocwyu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ghqclxbbs.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/ggvpjjhsu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gevwqvagi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/geamphnyi.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/grpfvquug.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gkhkhthzs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.hesvh.cn/Article/details/gvnpvydhm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/gvlthiqbn.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gpzrlirrn.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gjuvngrfy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gtkrsqcvm.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gmxpxuiey.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gaipbeqki.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gumjqexim.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gusarlfmh.sHtML


<!-- 参考信息 -->