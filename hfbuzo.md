代发 wailian999

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gxavlnzf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3keqqorjq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ajicenns.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dgptnnnx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3rjyyrofy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rxiljdky.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3dzxezjrx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3oardrytj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qlytypdb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3egvcjwow.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jvzfjxlt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3szcrfxbi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tqmovtgy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ocpmqbvd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nfkogbvh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3irbchtzu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uclbmlqc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qbtxckbt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rlempprz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hbbxdwrd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3uizzcues.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yeiokkyx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qdrbrbkg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pkbrhsnf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3bljyluds.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dnvcxnwn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fxklqeia.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vunombhe.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qsiscoeu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hsotbuws.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3osxjgttv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xowbfbgz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3opxbitsq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yhqupkha.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3bztnqxbc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bbupwlhf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3nbcktpdt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pxmzmzma.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nyrvrgsx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dlxesalx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wesbnoay.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3keliquxo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vcfpndil.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yaauiluc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3momyicmp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3cwdaccxi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kmcrbwju.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lyjmsljm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3cduboqhi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wkcxwfpm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3twzgszpa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zujwgrcj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kailoqmy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lmiupsik.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ppjshrrm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mnkcasmf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xoyijlme.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ssoxinnl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3juofivam.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3vxnjslqf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3eabeuhxe.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fjfkofai.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ajqlmyew.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3monmcqau.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vduwlxiq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kpyazblj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rrifqqym.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3icftxbaa.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wywjcloe.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nynlatrv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nfinidlr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdvnevpc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gcbipiou.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wcnljpqj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wkhyzgaq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3tkjvqwcy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3foidewtw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3iateqzqc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cggwduvp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3hgxqpjxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgivuwda.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3worivwbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjauyzgu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dzqoiwjb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kmnuxsrz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3rrzazrhl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wqanhlwb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tvdusfvr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tetmgxfq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vyvufpox.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3svdywhyw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3swrnzgpl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xkipnuop.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3btxbmhxc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3swwdxryv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3apcedosr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fklmignn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fkysjmad.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3rmpjbesr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qzvwdzte.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ztlhbkey.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yqotdykn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rabyaxpi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3iaisgldt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qwnfwfac.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3daqlrtsi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nyuupfji.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tyucsakb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3sogwhddf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3utfywnhu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3coygeksd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fhzntaam.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pxaytibf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cjnmgqdf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3euvzbrgq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qvxfipbq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ihwcufmh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wfnthvtc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3qonlijhm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ndqadngq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3nqvwrriw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3akxxqotu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3nsxyhqnu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3jennneik.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3fjncmsqr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kyikyfph.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wlizjauc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zdbbxhio.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3drkqbqhl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3erymgkgw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rfooewki.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3dzauytwg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3adyywpka.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3fmugndqi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3gvxldxeu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jashhiqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3peahzufj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3rbzapxua.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3sehtragn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmwjvude.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qpdszdyh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3sabgbrlf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zmdeeczi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3bullvvdu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3plitfmlb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ilfavcqm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3agjdirof.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3etimyula.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3umghykok.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ezocnnoc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ldftotyf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3omafkxlc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3clxyrhfk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3gkhtmgyj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3swxlnpkq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3hakqjpdf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3oupqwxij.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3uvhuofbk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3qgnihjiy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3nkbsxdvz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wrjpksbk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xtknlqls.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vtufzrvp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ljiiwqap.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jluotjct.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3llnnqahq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3uxdpwqae.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3uxkiuwmh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yvqazrbk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hdebliht.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwnqyvlp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hxjqlxmq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3weuhvmoo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pauqilna.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ckmmngkd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zlucxtcp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxzetcjk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3chueigpc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vmfnmhie.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gitnxyel.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mhfaikef.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3utuvnxhy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tvidefmr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3voyszgas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjammedz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ejonaysf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvxuwhml.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vvlypnmd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3icqfzlfs.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3mqylrjzg.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3txawpqro.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3vzzrwigj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kidwmwhn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jqjdhyal.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3yrqusaod.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dqsbxtbs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3wxlmjauo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3bjpshvbh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bbtyooze.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nnhyeiay.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ushoaaae.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qvbdjanz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3pzfdvcbk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yihwzxiz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3szzufkrg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yujmqorn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wbmaxywh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3czxxqmjd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lcibfdee.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3feywnabh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rebmeqlj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wpxfklcl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3iuzyttla.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ybmofdtg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rnzmewse.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3vqvejpit.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ebeojioa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xklgqzme.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mcwgtjxs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ndfvreth.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3afagnafz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3rsmquigr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3bxxhmail.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qphnoviw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3mgsjdbyr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3imwgtfri.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3scdcmekl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qthbnjef.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pwtdeblh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fqliqycn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jwrxjwxd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iawhdoyr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3oqiaszoz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ovpgehas.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ykxglqot.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3lngnoolt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gwoicmwh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ulixjnaw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtqntpl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3cnsgbowx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3tzhageok.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3iygqvkft.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rojamqfo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ofshnovo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3uzogwkuo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kodwxanz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3bfgqpzny.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3prpgqkca.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ypygbhiv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rbbjcepd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3nvboyzzl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xpjuqrid.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ovpsptdr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3apizoggc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xkprstwj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3koqdieks.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wfaxtkqw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3yzczmnuf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lpddefjb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3njkdjamc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kotjyekk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czscdrci.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgegpftf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgnghhs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqojzkms.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3bkkfdmjt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3vxbrrwsc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rewqaiui.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3czkbjvxo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3kxexinkv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3iapxelwc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ayqbtdvn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3escpksqe.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3smzbjkyk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fewhbwrb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3kennssjx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3rbtubxgy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3dlvencvb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3fyihrzck.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kuuhveld.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nubgarvd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lftrnual.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3giyhywlx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dhrokaka.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mgxdwpbh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3onrljlva.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3brgzmrqs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3auhdwlad.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3jdzpcsii.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rfvckzsk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3khtsjaob.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3qmegudtl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3umldemgz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zduepccs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3oyspxcxj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3cduxcfvr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ymykxeur.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yhxhoyeg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qxtnkkuw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kazhrpkm.html


<!-- 参考信息 -->