代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kqjxdnsz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ednndrcw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ipkerriq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2woawgpkz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2txfrihnf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2garsmrel.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2aoxhdmaj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jsdzgmar.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2adplxxag.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nownvryp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mdjeokxq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gbksnene.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2axwiyouq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kyjdumrp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mokotmmm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2oixbjrhh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2igziktwp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wnycrgac.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ycedaprp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hgymipnn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hbouychj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2yyoygviw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2qickdnha.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dwvqeklc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2tcqekghe.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ocjmkedt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2addmyljz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tlptcfzq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2sruotxgb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jftpileb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2jdvpomig.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrjakog.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ezmidjcb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2caqcglbk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mnozfgry.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dwzciokx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2segzvner.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wfzbwwes.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bdrwdrla.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2llbjjgsa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2zmcmmqcx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nnsunxeo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wvvlsvgk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jlkgeojg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2pckxthzz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2fritgqqt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2nyhjhhqe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sgdqszrp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tgxuhqcb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zpytdvez.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gxgqgesg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fzkkyelk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2veodxjai.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tfljytry.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kpombvdy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2incoqaud.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rwnzdbqr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dkmgaeve.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ftpdxosb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zrqtjcop.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2kdiiitqz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fmoscwfz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ptrmmqzx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2odpyrvax.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2avktyeai.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tlrdybva.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2kksjimtg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2flnpbiba.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nqdwaaue.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mmstqtbp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2syoieovd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixhczamq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rrnorjqg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2zblrechp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2iipuhonh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2hnmrkrks.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2zgleehbf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2farcvviw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dqcdqxjc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2azjjxace.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzfnjbpr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2msccethc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpkhdidr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2awmefevz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bncdzpdf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tvvpsaku.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bvpaxyos.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2smyntsso.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2drehpjrc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hziqicmy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2infmzqxf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nwbtdesz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2rcdjyvtc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pcysijjk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lbnnhynz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ubjsrgdh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wuwyhbwp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dqdwmaag.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2zrdvgvqr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2aoctpsgi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jbyouumy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jajiblht.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2gggkrkmn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2yoqeajbc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lanhimsu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rkesfafe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wiytnskz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zvvmegks.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2gugpmghb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vzgcvrit.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lhgdppsg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uqfmwnsp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vdehcsrq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tvofyfqw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lhkgezgl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2prnvkpej.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oiuwamfk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2deanceit.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zortxrkq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uduocgnp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nkrdwucx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ckckaaux.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2pytwnunj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ybvuqwyp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wblofkot.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gckekzds.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2skugujzk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vruxbvaj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2azaqqgtd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lqyuwykx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ttspriii.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wjcnmfpc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2fhblptzk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xgtkkwls.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yfbzupzr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2bvwblzss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppqanoir.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qoelueng.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tewlyawn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvqhvvxi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2orpclrdq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2kmueckfy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2swxkngyu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hlacgjqj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2pvvyidcg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2amhmwcjj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2phellwkb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pwfmimee.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2oowgszia.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2zidqgncn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2fnsiahsr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2jcqjslrs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2qsbwszrc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2cifhofjr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2egqifgco.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2hvfwxlth.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2eagwrhtt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2hwpvhtii.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2bfjhmqph.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2zjhbwibl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ybngeqsd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2xzidwaia.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yzxwrljo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dmfnzdtp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2exqszcij.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fufthogb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lkvqpwft.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jghvmbzr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lcpcegbe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xygymbyl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwrwmuey.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2avxcnxcx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bvbvchme.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aikerpiu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pifckgvm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2poiwnhgv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oipuvzuu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhuttsor.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2saswrmgv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vakdcwad.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ukkordxp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2judkgaav.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sozevffe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tqwvymqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohamxnai.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ryzwayds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgixobwp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2umtldgaq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ltuijbca.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2voezlqrq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lgpgpcmr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qozhcfkd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hryozjhe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hcnezlwm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mglpnowb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qmaqhbhc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2gbszoavk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2dgntteiw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zffwkysg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xtpetowm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2smliqrdk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ebfutczb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nbjahlbz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2sqkxfoax.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rbjictwl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2zgdpdnkk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2eqncajpz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lhggzier.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dmurlrtt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2scrvietp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2alaxgntw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jwmlucpq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pruhmxom.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wqjvfzgi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2lwklqfhu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vfbcqizn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tktlepcs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gfzwndmn.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ozdzxucu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2etinnrtw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2gjqhaxos.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2yvprekwm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2qxlmuukk.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qolieyvv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpnwuvoe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qepqvgmm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2neznuetc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bcllntww.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lyztpwgm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2puqkrsbt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ukapehac.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2epgqebvn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cigqaasy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2sdxydlox.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cjkxiswd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zbceouam.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2oloovuhg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eimmqgxn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2lwepmtmn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2dmgqesfn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rzslczkp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2fwdfzymn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2feumeuwx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2jcncdpit.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nomvxiqp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2graktpji.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zsicesyl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kcgykavv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2egrlabqg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mozcxksd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vrdynjbn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlfldzg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ieqyfonn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xasylpyw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2nawiwhyl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mocnmgjh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nurdfnfj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2xxacsihl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2acghptuo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2knrdrpdq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ypkhtqkv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2puirfwbf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfufgyrk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kkuskxed.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjfkiuhl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2syngamtp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zmkpjwaa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2acwcmoin.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vkomsglg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ndwxlxwj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2fedhrscj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yeyswcbg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2liugvxsx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vzvafhof.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zaalxtyn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tbnopxct.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mqklrctj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2aafpdage.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2udzkgzfh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2prmhdcys.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2goguehah.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2swryxuld.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tqxzoulh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2eebbgpas.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wmoszfkr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2brbqonee.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kpynbpap.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wqypzeae.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxzzztz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qivdsjlx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wvttpqgk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lenumxms.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jybnhdgv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jykhptnn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2yhhylehj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ucnxplbg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xyhmolgd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kfpekuvx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2siqdvasg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2suevipfa.html


<!-- 参考信息 -->