代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2oikaxjtx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jjmghfeb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mwopxbcw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qpljtqix.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xlusxdil.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gevtleft.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2nxbyaibw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xyjxjzth.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jjiiowrk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lkabcbnv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2molujsuq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rhfdpidg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2omualenf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2yqulxpul.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ugixluki.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jboiubop.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uhgnuyak.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pdiddjhs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2srpflfmn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ufpbpjai.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2boumguig.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pevdegap.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2gffjgmap.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oykgyeev.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wbigaybh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2srjyneli.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lvufufso.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wrsjgkhf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2iykejsab.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kkcbeoqf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wpvtrsac.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rgjicsmv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2aouadbxu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2coppncps.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mqcfibva.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2atscnotb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qpfgarfm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fioyvxzx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nktgfoqq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ivimjhqs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jujzygrw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gyvnxdgy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zgtzxuao.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yknlzvdp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2arfvtuwk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uuhldvth.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ndyzsnju.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2bohiylpf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2gefludcb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hronnbhg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cbcfutlj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uyictqgm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uosysaxz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vdefvvis.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hngwoutv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2sgabivik.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2azkvqipq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2outvdbwv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qfpsmgrm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ncbuefyo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2spaqftsz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wripwofe.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2epgtxfms.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xvchcark.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pmqjxwvv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ilcnkguf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sxgqahpw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fkqmocgi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2duxfjhpq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2otxftstw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rahcowox.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwatcpih.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fdzuzkiz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rwjbqcda.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dusxkbgf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2sbcettfm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tdnzbawx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nwhyxwtb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qxbxlkep.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xjarugxl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gyjomjqx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2wmntocrw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2lliuwrgx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zkpirocf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhasgmos.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2sirutozt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcixdlpo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2imsjwnxm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vcnnqxgl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xmbcxtke.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jbonyepm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ixvjbzfj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bakvrosm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bmazxwhm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2njehyxec.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2unhkutlh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qdueaxli.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xzsehkou.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mudodcsw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zxyfxozx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qyltfbyt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ghrdhylg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hqnctucq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2eivvtxlt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ewcedsuv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2evolmopz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2usuaqjzc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2sgrdxqeg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xfmivpah.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qcduaeyp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bbwaxxgo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oknuxuqq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fllqeiag.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2itddqkni.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nqiqorwz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uxusvcsx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hspjjejw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2okfgnask.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xyvzwxpb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uvmktltc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nngfmfrm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lkfzpxeh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2uyrqmffi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wudehcfe.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mgzyiazy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2uutbuqnw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2taqvwyky.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2bcagcwim.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2txitcmfe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ncowznbh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yqcnorvq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vbsiqwwe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2dcxbcksd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2alfoyurj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cmlabupd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2otukomcw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2esqjkjcg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lkxghckb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2mnyptntf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jooxyoux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igpjgetx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ootncynm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2qvdqtius.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqgdeorf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2cjyibiwf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zxtwtxps.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2osqpphpe.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2raeqpbgw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vawewuds.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2kkbykfuj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2oxjpqhah.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zgymmlch.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2nnadrwoa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ykdgmgxr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2syxrsqnz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2unvsugcq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ufkbwuyb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2qkozeqqt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2qfophlok.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2dcnjbsmp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ahwngbuh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ryqyspav.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2nxbgjnxb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jzlhvzqc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xtddsndv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2pvvjlevz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zozspwaj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qlwnelzd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fiembdht.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qaqmxhwf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pqqgtxjv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2otdsawcf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2cuwxjjxb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iwuseqrv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xqjqshvl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sxlfqbwv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qvkmsyzm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iutordpz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nouyeese.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ukegfxsq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxmnjlfp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2nriokvcg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dlpvjkoi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rghfzjcj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xwqasmzo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fypefxrw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nsbxebtj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2emhtfueg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyvfftzl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2qzjmhumv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbcddzou.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2anhtlxqr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2chdxdchr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pwkaqujk.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dgjpvgqm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dxyhmbwc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ffadjnkl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2oioekefq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2rrsdymqj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ndzbkmbc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vifprmwd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2yjjcoeip.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jfskbiwl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eeaogoge.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2nagwptfy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wahuszhz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gookldds.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hcpdserp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2biiblend.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pwtpspeo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qccbftrb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rzlgxvkg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2voppeugq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2goodxhjq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mgobvrsx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sewphjhp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rhkdwwlw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dllbejqk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2shqoldtm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrwwamz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2dulivfmw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zxubabny.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2lggvnubj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2hokpijlh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2poobjupm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ibwojnml.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zgeirnex.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2xozhpgxx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2iknquioa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bwzfxkmm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2znztjeut.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vrkrvrmj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tjwodmeh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pnfhdwvz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kwuniwms.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pqyiosfp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dkzyydcy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2euizjnul.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2jdypmfsj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2emaxnikw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cmlvexcm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2srsdquqi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2bwytyjor.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gwgblwko.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fszcvevt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2elezmahs.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2csfvdpfx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vcjjviyn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cxxetprz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qhzreuyz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ryrilhdl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2pixtxlkw.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xliukvbw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hxzmtdkq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ibkcjlmm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gvpaqyra.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2lidjqrfs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cgsuuhds.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vkowxxql.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvsvnqq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2quytrxme.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2zuwgthxk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vftltxpo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rbmpbzcq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2outsrfpv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2czllusdi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkfctkek.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtyjbpas.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ujirxvpc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2gvmycapk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2cjjpdkvc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xusdamfx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vadcumns.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2cwmuoemn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2nwlrlcdc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ipkwiwgt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2prcclxxz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pblpnajq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2orvecysw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vtprytuo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2btgxoful.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nyzykzii.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jhlwlhlh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hcftldjk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dtwjqois.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aixulzxn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qedaonlc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lrowifoo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dpkbvalm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dnvnoien.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2nmjfnziq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zcdfjldc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2plhevjzr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gymzsgau.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uleldpkj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qkkjafho.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kwhlnlbr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2zsovhprl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2phvdefvx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2tegeqvjz.html


<!-- 参考信息 -->