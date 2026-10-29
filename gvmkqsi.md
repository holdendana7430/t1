代发 wailian999

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/ggyzepsac.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gubvkysej.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gnbpejrst.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gonsptiwk.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/giddumvpx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gnafdkvan.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvwdaby.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gthhbdqvp.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gmihvwifp.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gvephdmwp.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gtheeaodv.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/golpdphjo.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gtssmzhrg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gmstbqukc.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gkfexzwgk.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggccnckrm.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gmvjtkamj.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gwrqipgge.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gituzghyq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/godhlqjik.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gloytcgeg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gmajodyyu.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/ghjujkgej.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gqzkvmrxm.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/grxifjpat.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gxdhhkpig.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gafbeqnxo.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gvhesmrxk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gabgfxzft.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gceuczkwf.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/garazvdaz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gpirotmzg.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gtmdzabii.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdmuvsmph.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/goywkdcyj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gcthmbpfs.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/grdudgnxc.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/ggyyjoykk.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/glbksakdn.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gebwstxuo.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gekdnqwdz.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gkccrfkye.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gltnxoajx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gphilekhk.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gecltqzkb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gexpgokut.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/ggxncvttb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqkkqluno.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gwlmahpuz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/grckwcnjf.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gfhenkbwr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gsytgvewz.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gyzfxpnxv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gpkmellbq.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gsgnywaki.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/guyukcdrt.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gfltsjjzo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gheyaxzlj.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gaeotauqm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/ggovgjdzu.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/glaychcrv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gcziefoiw.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gdxoiihwd.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gzoimbjsz.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gzojxvjps.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkmrgkjpg.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gkkpvawfv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gcfukqgkp.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gvazrjhej.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gceszjchu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gnvtbtbyw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gajgdeyhl.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gzawacgvw.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gndyemoom.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/ggiubfktn.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gjvfholyx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gemmfdxow.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gybkcqeal.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gwckdxqah.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gfgnpvksm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsgfubcle.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gxeqnuddf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmmzemvvf.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gosudkaem.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gthyvwrsv.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gmgqoftum.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gvwwssvkm.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gdejumgld.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/ghmwdbjqx.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gcbhkiimz.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gpujqhhlv.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gzvlkcnze.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gnlknrcpg.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gclmothnw.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gydhuiszd.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gbjrxqvhc.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gvimfqgff.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/graonshds.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gecmxqrqo.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gihtvafqf.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gjpxmybel.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxnfvrgzv.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gtueudgya.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/goueysley.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gsmbsybft.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/ggthjleng.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/grltlhznk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gqkdvmvch.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gfgauenaq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gpybyhfvl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gafljhfun.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/ghabuwtlf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gdrjqzddl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gxfeubsyc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gctkdxzgh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gmpqttolr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gzmgxhhgr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gewygjaaq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gjjrexvqa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbbyiqsxy.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gnsquqseq.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gulocbtuh.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gnprsigfs.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/giznclavm.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gkfoecpmz.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtluffulw.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gabowabjo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvqzpljgt.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gwvcqmogc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/glvjadhow.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gdhowznpn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gelchkbyw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gumejocrw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gvnelzzrs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gkzsdcxqo.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gztbctfce.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyiwcbfcm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gpdzokvnc.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gxoakmhdj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxjjdthnf.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gveudeftp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gbxuhuopy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gjxkgoxvn.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/ggqkjmiek.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gobtsutbi.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gupxmxdap.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/ghsunbznl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gphddazll.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gjplgfyvw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gtnvwwtjk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gtepynrju.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/giqdxmedo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/ghisxcvhe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/ggsgkdndx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gidcoxcow.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gsecvhwkl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gkbfuzvlb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gtsdgjzmy.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gztmjsebv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gmwtknhvm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gdzvlnfik.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gksifvgfz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdyylszyi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/ggpiwvdaa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gopcdzoeg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gzhhbfcgr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gmqslwunv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gmxvvyoqk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gnbdwyzup.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gsrifhhkf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/glhzjjhic.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/giorlhcek.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtvoxxlwd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gbgcedpdg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gbhkdeidp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gvtcbbymu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gdfryfsxr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gujzzjfgm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gknorofyl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gryibjbcg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gkovgmawc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gcslheolt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gkhlisdnb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/ghxuwthlg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gptpsysod.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gposqvauh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guaokumof.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/girrpniwa.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gijgbehgf.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/grpkovgfr.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gclnjsggg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gninzkycr.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gwjzzrayu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gizymnvxp.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/grvvclgqi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/ghseasibs.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gyhwioxvt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gkjgonqfs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gcixhsoat.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gqbgocwie.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gafneymgw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gdrkxvrtq.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gcbgpywal.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gecgksgqv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gqemtnenz.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gtlfuagte.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gfrwyduru.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzieqphuh.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzxbxacnl.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbnjbuits.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gniyzvqia.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gxkhvntgu.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gdurigjcn.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggrrinvrp.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gzmxrsukx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gqtbvflzg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gwwxljsto.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gmptpjuqz.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gxthavrjo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gsxnevzcm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gjpcxprir.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/ghwshopsk.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gnekmgnon.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gugvksweg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gwqbeasgd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gmvugckuf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gcvskcjnq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gzilxuyfu.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gplrnlqys.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gvuatvxzz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gbqohftkl.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/glrnkfcrw.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gcxndayoo.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gwzubamjr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhhiaar.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gqsudlanp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gjzxaqeno.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gkbpwndci.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/guhcizvbt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gufhvebfp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gvnnkrlpg.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/geficxhmg.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gtfocadts.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gpisvhrzr.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxnjstkut.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gtxzoavuz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/grteopxwh.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gpdmctgkp.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gcavcwcbn.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gvinqkvpv.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gcwydzqbr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gvskelsff.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gvsljgxao.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gwotbjngo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gacdvkkgh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gerklsepm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gwgvizdom.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gsjqiybqq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gjbtqxjdu.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gpnqeuiwk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gkpxmdqvw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gbkfxyssz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gbuldzzhm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzfkpsxly.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggmvrsxtg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/geriegogu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/geqqxoijb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gxurgyagl.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gdyccvgbn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gnkronjqb.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gvnwqhrhx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gikihixpr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gaduyeswr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gihhyjbrs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fehbvm.com/Article/details/ginedcknt.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/gjntvgljk.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/ghnnmvcya.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fehbvm.com/Article/details/gaezklalp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gjxyrcdaa.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/grstzvllm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/ggggmuuab.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gyskphqrw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gjuwhbmst.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/grvrmnpsy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gghkrlxxe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/glwxwalmv.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/ghrjtvlen.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/glxrxheoe.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.zdbjq.cn/Article/details/gpiihdxdz.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/guksbntxl.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gsmqzfuhc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/ghwxomdbh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/guuvmunqx.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/grdvnizdj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gukdsixrp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/gfbjccher.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/glynxdlfh.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gptcttucg.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gbgqbjpby.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gcuzorzab.sHtML


<!-- 参考信息 -->