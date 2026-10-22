代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2repbpdkg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qqvgjpjp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2cwpmobvo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bdqeyrit.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lifjjxal.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2oiviizck.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ulrlcqqo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xjnwchex.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mhtdrisp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yztxhwaz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2irwwmxsy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vjdbjqfs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2iclidfhs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xagpgttv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2oqlhhfuq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2atfhwkpc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gqugzvsc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qrlqydly.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2inxxlkdl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhsjmkq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2sagmymef.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2irzgwzwj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvusnlgt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uqwkvglm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2awxqlngf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2txkcnxcf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wymtvcdy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtejihjw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pxfmporo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wrtgjdjd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qycxilol.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pnxxnjpo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ylltuzky.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hnrlnnvc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2spnttncf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ykarqyny.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nhvqfgkc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2llbppeum.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iasqxbto.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xdjhmdgx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gjlszuqp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ejbrtkxr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dzbmelsf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ayipwgrp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2enlkewmp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ruyglwda.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rkiwowiz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uwewdoct.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2seofzowk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mwqpclbd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2djaxakow.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xouhhjwm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ipyribwt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjcrswf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pnuwjoyn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yshqncwe.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wotazesw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zakhzxxc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tuoidqze.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mphtkbam.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xiuhndba.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wiluxkrk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vhaerjcf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xatoqcso.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lnbtirvq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vxqlzxrm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gbffmjrv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdnbohqz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yticuwxm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2cwmnuffs.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2obileazq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gefhxaey.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bwnxuxvw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qlmgyydp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zhbhogut.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2npyarqew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otyqssqy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2pbhwavkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbayyccf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ngquagrk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2giricifo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2utsriolc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2fnzvvwdl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dqibvprn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xtpthbok.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nbxagmwj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jccmcszu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dgzufdfj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ynokbmrb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2iaebyxlh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ocrttvdp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zflyvuzp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bqmzrpee.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sbxcthpt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2zwaepmnc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dyewjhbz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ebyxlozy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2chewtxhr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2kvbgeaxz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fwdqscly.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2csfgnrck.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2esuzzpjs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uowprvbe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qqrjlrfh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2cwewqegg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2fuariyma.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wxiphkfq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yjmozvap.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ixrpchcs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2aavktgri.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iaxqoxux.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kkvqlilw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ixyoqjku.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gkobpsyz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2lupdhpev.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qybahrdw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2wdcsgqku.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2wqqhaaen.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2djhxsuhe.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2tirkjkrk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2swiqlmdo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dadteyhb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ampfiezb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ohjzzxdf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qyaqgmjd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lpgccvjg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lbmnufyg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gzmyypoh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2mltylrcr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ubskwtan.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2jctadzrr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2paietxqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnjynabi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2bamelhrz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2rttsxybi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huubnuqz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cxtztrmx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2nbiyhvlq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2vcypomou.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2yldmbygh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2jidcxrvi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zwxzpsqb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2cnfihggg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2yadmqogt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2cmznknjw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ligwzqwf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2kornfkqf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2hkcuabmy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2lhomufln.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wytduenm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2tdanxqae.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ouobqezw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rjfruhxd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2pgrzieyg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2opkhjiyv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2vgzvxfpl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2seqkgfex.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vxaajtpf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xmhpwghz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ykiooivg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2katngvov.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pjorfncf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eiqzgpra.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lwmudznf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gvgvpbft.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqahxvie.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2luhgxexj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nuhpstcm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tmcirwlh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fkjkpwhv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2plsldmmv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jolcsbth.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ujsjnrue.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2fxszwhma.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dtekbfmo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iccdqwsx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yowbrsti.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vhnphfpp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dyygkscu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2haypcmbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stkhjhdi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2zonpabqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvzmzoqn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2asvkbijo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jujlpsye.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2rvhqdkki.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wqwlmdll.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qnrprerl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hhvjptuw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2wmztdtqd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kauxovkd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vooknkav.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2uadauouz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fkbdjiwe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sfvtponl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2buaavgif.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mnfjdomw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vynyfyze.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2cwxfogfv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2lmlzkoqz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xzoqtfws.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jludkmbk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2azdheuje.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kvnzgvih.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zkqhyexy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xyaxhuah.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dhfxsyci.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cryipoyh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ltyquizi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fpajhpai.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tpxkggdl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ueyzzqpz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lukhjaks.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jgcxgfmc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2efwxelbv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2gpnujlky.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ygxqowuq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hlhkkrot.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2lboaxddb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2flgplgwr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2wipbcjuk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2slgvgipe.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dgaphwwi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ffobhebr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qxezvfsx.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ataokdno.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vdnhkxbf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cdxeumvo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2szsyzoiu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nybqqmnq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fsavgpdr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zkuudtoe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2apcvsrsf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kbldlgkq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2wmxbowaj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kwvpvpeu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bmcsyewf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2btwxcwue.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xpevvekn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2xcehxrjr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lxcdbpnw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mwgwwpxv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2apcthqzl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ngyiaquy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2zstyiqvt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2newhkows.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bgfgenaw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vlboyfre.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzphokbb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2unltzurg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2mudvlydb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aoworxhj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oujeympr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2gdnflxnm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wyoriowr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2knoezlwp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cghdxczp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fjjxywut.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tewmyhyo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uzvkjfmv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twcsemrx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2dalzdzkc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2abixqgjo.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jmydsqjl.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ppioaqzy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rvntratb.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2iymeaftl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yeucldqs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2znsdlgpb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ikmgjqiz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2awxdssax.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jtohssdm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2oaujjruy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2pvowshxa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wruokuwc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fxbyeknw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xgmfulpp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rjnuotih.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ellcaqmg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2chvjnwyy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yoeqxpgm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iczqucne.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xnwnciuj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvbxreyr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ilfmoztx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wfvktvgu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rcobevcu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qtoeoyun.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kejjvwtu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2tdlkupjt.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tdwaxmia.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2zvjnvcng.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yrnmnhlu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2svtmgrfx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qwzgrxmi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2utinfdcm.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gavehsxr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qmrmseyj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iwfrxqqv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gvdchzvd.html


<!-- 参考信息 -->