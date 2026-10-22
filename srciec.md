代发 wailian999

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2etfwihok.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hkmvgxbu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qausjbrv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xuyatgak.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cuslvjof.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lmohpezy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jpmjtxng.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tjryyxne.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vkgolffu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xqytampe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pbfxylqu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2vtgfshsc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fuaykenm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bqylqvai.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wbihgekz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rywaojht.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2fmkezzel.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bcoqvzex.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ydwjufre.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wwcckpzo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tgiyrmrq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gfpwukex.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ignitlxv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fuypuroe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxhqsnfq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2umquxicw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rforlfxh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vuqrhqlm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2emzyzmzy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2bxnmibgx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2axvycrgd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2plurqelc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ixygqfpn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2renikceu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2yrmqxkhf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ukatvsrl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ghiyxawt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2limzxfoi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2fobzhcvl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2nnujyjzl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rtbbcczi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ocrhcxqk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zlonzxnn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2pefvivnd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2szhbuggk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2odvgbnky.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ohiipcwd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ywilrxbz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gkxserty.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yzhyqsea.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pkecyias.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2moslxgiw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2erobmtrf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qeotgprt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2hqsiqeeu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bnqyicfq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2czcnscjs.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fipikblj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2hwqozkwi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rlsrzfza.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zxnjvusb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rfbkderg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2oepentea.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fqpokrky.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2biuygjdt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kydyttai.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yosixhsi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjfosfmg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sxhhhgec.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qqknldop.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ydpioorr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfrynkua.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zdubjdng.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2yferdsdu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zjbauglk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mwiqmktu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qywvaidy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2txiczgbb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mawlrkfw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jytocujo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijpuwyiq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2btkjqiri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltlpsbwh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2cqprstum.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2egaqozmx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2sobusgij.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2yexiygye.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hersxkgm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2miwpwdhn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ijmxyxht.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ypxrwpwf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wmdvebsa.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dawymows.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2nzkrmzue.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zemvaglf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wctlzmjp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pxyucurs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pomjewkt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jmxtszal.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2malatgqm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2iujkltek.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2stzpiajl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2eaxvrgyz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2athracwl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fhedduta.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lsfifzcx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rjbkyhez.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mvaqpqcg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2satkkoog.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2etqyqslg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iqozfqlw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jfjtamth.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aoitnbde.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xhbqlfnl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nvnumtnc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ikiytaxg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fektdhwl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2aturuadr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2beibryqo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vwrnsadv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mmxqkjsd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hjzrfmjr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kujihwyk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2abggpuvo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2reavplsv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2obsqhzmd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wsdvafbv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qanfiwrw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2pdwopych.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mohrksls.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2tawftwol.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ejvvwszn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2apxwglxp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2irpafvtb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hrdiiwod.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2kehrkrri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpizrgdn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rqgecrbe.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2bmxufpgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvlwlxzc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2tkpzorix.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2zurtlbyt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gurwsgcc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2wrzchusf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2wzxtgfbo.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ffwwhmmb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2uxdykecq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2dyvxdfhd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2zwvurcem.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2tbylswjh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2bxcwwzqo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2cjyqgwdy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2uhzoarmq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2sjmwsrmo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bankoftt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wxutsbaj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xohcwylj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2affepgpf.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2djeicmmo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2itheyniq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dzyoaauz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2smhvdacw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2catisvvz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pmxjzqhs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dlmbdbka.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nfbjddqi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ujlfhioe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wfzsuyqh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ubckbegj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ygbhvbms.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vcqixirb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ijgdgwda.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvmxwnzl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jaylfvag.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lvjdwaiu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dtsdvqkm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2cfkyzotq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kwxaqwws.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rwyftpsu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrdmojkw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rjetluro.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yarlrgqu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uwsnvsjw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iiwskorc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohojrlqg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2gnszhccz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kndkijfx.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gwaktjuu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nvxapmio.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2pmizvikm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2intusnlz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2nixmxrrl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tjpoyjuv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2msdegfvc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2cfosleaz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mjhbyefl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qqmscpnt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gzsdrmim.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zwqdiyow.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hxkwvmho.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vjgmyhik.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2frkbtgpe.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2cqvatojg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ypqwydmm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fjoogdkw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jujepgat.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2llptleqo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bdornsfa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dyfmwbhc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xxhiizhy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2crrgtfwh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2boqtamwb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2otilgqph.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zdfqhszf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sgtlxiod.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2lvfoevpe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2brqmrqkz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mhfmisfu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qowntwwj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mlrrgspd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2gwkqmmvv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ihppfqgq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2uqdnssiq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dordxwyt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2rbycojme.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lugicenb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nnudjern.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2arxhwxiy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2icehpfdn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cekbihfp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xpusrwra.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dycqsazm.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hkglylpz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ejzuclwe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ntnhpizp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lffcgmua.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2srqoqejb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ibdejkqx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzwausp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kkzomjey.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rscnlagz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2vtfoairt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fxdotixy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tgeiebgi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2tgveyogu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2frljigtc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pphmduks.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2tuxwyeai.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2apbkhfbd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pnvstdrc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2xwmvplfo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sfubkvdy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dfntclvd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lqugszae.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vuzeyfbw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zmbvpopw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kjzvrdxm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lxyapqoj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gdslwmlg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2chsvxtkt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utfxqtwl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qulkkwnx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zvvzuusv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvccoavg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aheaxdmn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2atupysaf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2bigdcsmm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xbukftek.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2yopdcwza.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rhiuojeu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2bhxzcbgp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oakpngfa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwzhwapp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rfmgcblb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2kwrrxwhc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vlscganp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2lyfuehmc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2zsurtbpu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lxgtkasf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gonezdiv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fbqllpne.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mrjiirsk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tmsxikyt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2kjdajoro.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gpnfwgue.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kukczttf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hwuwbjbm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ujgzdnry.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2bjirlogi.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hgaiyuki.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ltmpqbso.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xavzghgw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuxzako.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hwudzffc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fwynjftx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2tpigfyge.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bgeeuhgh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cugeiljl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dxgfzcsf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pcqwaypl.html


<!-- 参考信息 -->