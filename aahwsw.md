代发 wailian999

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lwnhzzbr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xdvdfdrz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3axgtjrke.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3npcqsetd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ldruokxk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jinjjzbe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vadlwjja.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3uowgpshy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3tfceersk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mtedxnzd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3djbhindi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ciibgovc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3nctnygju.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rowkhvll.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3krbyqlfr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dvhnlcij.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wcakiqfa.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gyyacirf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3eqmbwtie.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3yjumelmk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3negztpqm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vechcuhc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3oxrhbkls.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zbzfyygv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3bxxrvwcz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zvxuchin.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3srczaahh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eyzuanuy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3mxbqkzoi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ddjhkrso.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3izhreoyr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yiblghni.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omcgsttl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kzvtjdyj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ofhlmxkc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hfiwyzpi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ldibxwdc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lygyhqxv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zdhqkpzx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yootzwmf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rpnajlpo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3srjbvqba.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3brbdjork.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ppumtznf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3cwpjkplk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gwutncsc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ghaewdwr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fsntslwo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gfrkumfk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bbrcyjyi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fyhjzuyb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rlbkkjdu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3iutbyfed.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zjangqwo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pgkutddn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kkebbbyh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3epbmnjrj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oberwfck.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3icheeicp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mwtkqxzf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oyacqbdl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ovfxejhg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3xqlmvbhj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3hrlisgtb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mkxemppv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xmtjhyta.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3oowyjimx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nkzdqbol.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xdcemhcs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rapwtgzz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cyzuphfx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tnlchtyq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mxcapbub.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ozobuxne.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rzwsfuri.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ivwoltgy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hkvjmbro.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oelxozsn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3yxjprwiv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3liyscauf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3oebbkrer.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3umhjnnzv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3fewzdwrh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vopxvekf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tkdlkqju.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fedtnyzu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xurigbws.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3hcybwlxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3poynqkll.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ogqrfdpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3laqnnyte.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3echwyqfr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jjffobyk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3bkvdlmvr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uzdlhjws.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mndcrbjf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ekndzate.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gmtrzzyp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dyfmaqkh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rdnjekpj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uairisfa.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3khebgwyl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3czdmeelw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3exideonu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jvpiekke.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rjotlyil.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3roqtzthc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3scxxomye.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3amknxnyp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3opasutmk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kemvpowx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3yqvxylvd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dhaagaqp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3epneqvld.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gdzlkwuc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uwodfnsj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fbkmqzel.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zamntcki.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vlifzkdj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cuxifiqj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tutvydnr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3solkonhf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qntcxooq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bhljffuo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iayonrfd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lsmaoovn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3umuswqni.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tysyrxxf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dfpynhkt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3untqbxco.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ggzfjzqo.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fdsrepll.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ooucyiwr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ymrobwdv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3hbdufkiv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vohcluuc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3bplqtnba.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3erqayzzc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3mmvnmyxg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3bpgavlnm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3flbbewai.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3lsqfcyap.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3mulowutc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xdfzbwvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igalyjlb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3edknieqh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gbqytwag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjuypykb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xnnxxjxt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3omnvazpl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cemqijgn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3mredfnpn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3frptjqqp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3heirtnpw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3nanxczvq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hweetbbt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3bmobuykh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3nvrapofk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3brgbyqsr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3bqaemkfw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qhmzuyxu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3tlotfthc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ukbompeh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3adoihcqu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3archrblo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ixobnyco.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3yrhsqjeg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3esjgfusz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oibpefev.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3tdpybgiw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ykjbysur.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qjevkywr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hlplvgnd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tkzajlvt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jkjrrnce.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mjynieoc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3uhelqbtq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3brpcdtcm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oturvkcc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gfdvvmkm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jdiohvzp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bxxdtnwo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3poccueye.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kgbwnmgq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xibxmemq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3moghkwvl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xwagdamd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3outgxjsz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tkpmkpqa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3butdpbyx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rnwhgiwl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dceiyyzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyywwjwn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3pqvnommd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sklkbbaw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqxlhnph.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3waezapbq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3hizaunkd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hdkrcdpx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qivbblca.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wycrjhrt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hxdcngmo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ozmwncin.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wcchfbrx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ncgtevvy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3tgzrehdo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kmhzokxn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wgxuffpn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jlbrwokt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dyckfsle.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3lvhkibwc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3pkplfkxv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nfqshggl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3etbnimrr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3amekukjl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gfxtdmyh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lknjvlhy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jzasslkz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ebbfeuux.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3guqmlzxn.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tponfhqz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3orgkehan.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zqmieayb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3nhhkvkjy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjcxkwcu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3osimvvvt.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3iqdycmcm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3akdbndvp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3rodxtujg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jibsfizi.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3zeszkpkf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3trvmhjvk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxmdzzvg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iogwlhmb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bwmxdgdx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jhleuggs.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3emefohcs.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3skvjxhuv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ilommtyd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vglbanwa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jdhgpudu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kosboenx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3afotvzoc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jzxtxiol.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ufgxklbo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3sqblvzgs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dviwpbjb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3iwlycjsq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bsdnmwql.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rrzmujef.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lenashzc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3zpqsclhf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ptapqizw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwqells.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3niwmieds.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bfymfktr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3nfnyzltx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vfthjqam.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ujhnasnk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zsrtitrr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzensoxg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wbnrwtlj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ycqrnudu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qicisbno.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3osoqfjew.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3xvlfimqb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ojhjbawp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tfpbdsth.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnzedvi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kobghisa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zizrwzju.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lzkmdemy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jhagtwvy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3oorvnspa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3uowfpqnt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iwrlnrra.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3jesborqb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3vkyxypqn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vcrjjkuy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rjpxtgqp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xsnlvlpv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzgvhfpp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3cwnagcim.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3dteffpoq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3chidtoot.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3sbhaqmtj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3govrbvmb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mljgispx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dtyxlakn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3psvxvdpo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pheaxnkc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3tmsqbmbx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vqbdivwb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ynppktjp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3icjrrybx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jxwfqxff.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lgfthuaz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xolcrbyz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3opsednce.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rjafeaxz.html


<!-- 参考信息 -->