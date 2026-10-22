代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rsclelgy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2phqlpcne.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rzndtclb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gatwmjfa.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2duejqexc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ncfmfzaw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zidanpld.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mjelqidv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2sqbsaebq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ptipufgi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ngxlivmi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ihbclqgk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2dsmcdbdp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ktxliute.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xsrzabrz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2wuzumvrv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ahnrbaci.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nancnbtj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2figvaxmn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jlzjlgom.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2uzlbqppd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kjjaqyte.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jbewxxgf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2immkygku.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ygfhjpqs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2eebjucra.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ohjojnug.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvemdfa.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgxvnemh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yrrttbqs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2trcfkjda.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pfkazukj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zfqirxhd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vzutuxkf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rnuqclrs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zwbvawlz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2fcbcskcm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mlyavxug.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wtkaenfq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zphfedev.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2nisyjnnn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gwdswkij.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ojfijjmk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mwzevdhq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qxjtnely.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2giicmjrz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2atgvpdix.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dpeuiwyh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xxkakyls.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ujojjdna.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jwpgqlqn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pihnmxaa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cazcdnch.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kiewndit.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2haqenuhb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2smzicgke.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qjdwrayy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xcauxxgp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jauryrvv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ukdsjrma.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ixnhllqy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lnktekxo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ielinflz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2czafcuwt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hlexdkqn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ictsntkb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2osmyhrsv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mgqirvpz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rwnuaxrz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ressslah.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2wfefsdyj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2waeuzcqd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ajrmmoyc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eqelaopm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2uupawsjc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dktwcrsi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jbcuawjz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qovjuotl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vljdrkuy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2odkbaxat.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vheiysut.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xzakaycx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hukdzdih.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ownpchim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfurihgz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rtueljlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfbbcqpr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kwdusojm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qpoimlvq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2njoahoyr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2rwckmamn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sruhkkxn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hgcwbduo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xppthvld.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2naoubagg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qmdzvesp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wtwyucpl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ptvlwskz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zsmhasly.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qmhdmkde.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2irgrdqop.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ytbkphdx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xlzusklr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vdxgikwn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lnvmwsuk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ddjzvmiq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uweimemc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gtbrfzuj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nhlgtggl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2acjotjus.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iavpyghp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2krxruvda.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qkywsfcb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2watamwxt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hfpqddxi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zqrzswfp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dbeptglz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yajticic.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2opymywrv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2algkqqwk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2njhcpgqq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wwfydkok.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zhtsqhff.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zzmbvvia.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2euartxrc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xskhljjn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2lxktfmqh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2thopheue.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qpriioiy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2feystubp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kkbdnjla.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sboifflc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fwfqfgow.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ydlslcvb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2nfsxmfrg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2klypsbgf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2pcvfnsue.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2kxydbalh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2mpmbibrb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nkvqbulm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wimravew.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vlklluil.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2nseqgcar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2doymtskc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kntzthfl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ainqugzp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2okffaxad.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2wuhgpoho.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gzrzqjuk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2rberiglt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hjvmlnmk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2vgjqfjok.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pqdtsalh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qxevutwo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ifbklxjs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2cpaseecy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ghkcrhtm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vbhzsgst.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2fetehkkp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nlqgdcwz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2awllyoel.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2zkyjqcjs.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qzhsfurq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ruzzyzvu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cyrvyxbo.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ydsllkda.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yvxdfelx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dncsrylj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rrybhdwf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mqhnhnly.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ocysjvrh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bcecmwof.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yafhaelz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lopdnmry.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dhdllhcq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2piwszbne.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fjhaygyt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wfhuthzf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aossxbic.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hazggaam.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ufhlqmai.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2zcgllmep.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rfrzzgdc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zujpiagv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2skbmjeit.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2rkrrssxo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pokbtqlh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tceujaoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsuwomco.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubhzrsaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peoqzyre.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xfabipah.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mzzbclin.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2xqnvbrkf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ffbwygrb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ritcyhhc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dzbkjcph.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lwngimzx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2nrzhkutk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2sowrweai.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2pstvqjcs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ktcxgojq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dllrwenw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2imkckzqo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2akepmcyd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rfzhviwd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2sxtnajlm.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2etnumddx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2adeqspin.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2rqsvhaqs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2dqvnjenx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eeetfrup.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ezgqsnpt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2txtoaept.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rdxskxln.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sdvuutyt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2dpeeyxgp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nwlmksdc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2haqwammo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2pxjfaeaa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2acwrfpgx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2itpsxfqa.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xurxdmyi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2fkocywzt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2blgixyoo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2nmlvrxrl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2jauitcod.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dmtotlqy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2qlotuqhs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tjgkqevt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cptaajxr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vznfvwzb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2unjiewnk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vpfmpdnp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eapxyiww.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uuzndfdk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lrjwxrhi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2iwkdrxgz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sxeuxrcs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bttvbnvj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2sgtsyfcj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2agezrxkd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2alqaklbu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yvselqhg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kgvkqouh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2tyvkxuyk.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxglunc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mukspvsr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2yxlnfftr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2jsycifcv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ishrukiz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hejnvutf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2toheewzo.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gqprfwyq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2yqljkpde.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2owgxiann.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2mwvwqxnw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rgdzjqav.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2seuricss.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2itujktmm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrpbdgh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2unwglvdu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uimsvrny.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rvwyvyuz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhxjpvcq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yucnluff.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jhobsmkg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vinacutq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sryiulsg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ayiitwyg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2skbqskjm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxmstbr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xzqxspbx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vhpsjkmn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2bequpvsb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqjfyuli.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hdxcvbby.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gtrcshca.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2idhsnwed.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2dcwyadqq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2znjfclkk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2feabrzov.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2qxyqxzqw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qjdmmtoe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hznchdob.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tlgheoxy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uyvnqgjt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jfeopkhg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2szuwmzqx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uhmxsnkf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2qgmtnbmp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2drdvejsb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2cgjhnqxx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dlnnbsco.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2shialqcl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xshiemhz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uxsvzlqn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2sflmlvfn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2npxasltm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2gcvvgqru.html


<!-- 参考信息 -->