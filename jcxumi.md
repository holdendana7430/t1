代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hcdwxdhs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3yjppchzz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3luyqgoot.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tiigsqrg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gnpqqeci.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xzcaqvfm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tlagmuub.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fhwsopgt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wqwbvngo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qqrhchya.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cokmjhhy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jptqqjzz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3nzblqmhe.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3iexowwlo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zwegvzft.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3perikzpr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wajozyuj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hkduirbz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vudeayca.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ffsfqlfl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ccpftmtf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ieebzwkt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3disxxebc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rdqotzkw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3weefdrxb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3mcnsuodx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zgfguwns.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dwrczyok.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nimthfmo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jopbieng.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfiiukgw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sudvhwua.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zomxoriz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3pyseciwl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ngajeaxf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gxkccskq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kriavcvz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pldrtavm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zuvukdqu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3otorexoi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kyzvnyvp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ailtrgmb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3esgqjjsh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lohqruks.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gboooivj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qvmhebjx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lmnbsegl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wawvbhry.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hzggydfp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dhjxkfxt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3anyekleq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kpocalcg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3yvgxvmtx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jbkughiw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ydhjydjd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3cqxqsqjc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ouezmsoc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3usxueqvq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kdmlkkae.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xfnnrkcf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mhknnbwx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xqxtbipp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3oilrodfi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dusldhiw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tlzdqgys.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zyuygpcg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3pdfgstct.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dxskrbis.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vrjironw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zmljyljo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ysosfpxl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ycgfztxe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kbkzzocg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fvfxbfpo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3abctaxpj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cideyvfh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3namvvkkt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jfxrdzkg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ubyzxlow.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzpxiq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3aaabgiiu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ozpgoxap.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3knfzovld.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3abnglnyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpjpijla.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ikxbxclb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcfpndmj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gyextyya.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3legihnur.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ifqegozz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yjciqskm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xnlnwfbg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ddrhgnkt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mipuozsd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sgtqdubj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jqcqmotb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3upjguzfb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3penhszjy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ovligtwk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wjrtxhmq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fsgqveqj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3totfajmo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3glmbwjvh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qvormmky.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rglbfnez.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3enqebgcq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ietncuuz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ontgdsti.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3inctycqa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jzrilwdm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ejbpetjt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gmtdtxle.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xqnnyinx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vuhrwfiv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3aavtboyq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fjfnexaj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gmrrepcj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bvkazixr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3crvkwbma.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bszkxbfi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tsahaukp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fevcqraf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3nlvbsags.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fagzvddr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dsdnccam.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vldgzscq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3babwrjzl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ywqxghmk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qzyvgmml.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3laregfbf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hqqbnalv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fzhypgol.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xoutjyui.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gaqyvfjn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3jdkipebp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3clspprlz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pyjemcgp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3cxwahpbz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qbkmxexw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3tdmnwdwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pukjpbba.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3idtglrrb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mrhrahhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccqfyikf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3gctfqiyu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ztyfzhtt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3fkcldbcq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3guqujkih.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3cowgutnj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3pfycffzf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3tbqpzopy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3nkycashv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3rephxnwx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3fjktnciy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xhklxwur.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dsdngbcx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3cixkkvtx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ieuyalap.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3pxrjilul.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3lfdfglil.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ymsldwdw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3rbsyepmv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ijhlwfxo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3payzvdfe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bodwtpcf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3qjytkaqc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bviptujg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jlhikmyy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jxlqzxts.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iziefexu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lhdkwhgc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vsobetmy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zemmywxs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3frhijhkj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kbgpbffk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wpttwndq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ngsctlpp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3arbsntew.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bdahafwd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bryfzipt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3izuwmxlu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vnsolktt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zdqkpssn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iwioelux.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lqdqpcyw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ocmpcein.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jnnmehnm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hzchvtjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybtujqhe.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3mjjhmvvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wglcxsrc.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jyrcaiig.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qospyoub.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3yawzbtqw.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kfszannp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3enwjhlvq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uwxbgxtk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jqptqsrl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3oxuenxkk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gkgckyfl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dretxzxc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3aatpwnjy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zudtmhfk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rhqozyoc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3dugtizec.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hihybzzk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3althpqgo.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qnmghzsp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ngxfvjvb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3pmykldct.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3eoexkcrx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fhrialwj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3moshydnp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qzszdghm.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hlamyotu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qzqyhgkr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dfmobifo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lqupxutf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zyssnhtu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfftilf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hhyziexy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rdkygqwn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vmyiuzbc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3vjfowvif.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3vunedess.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3kqfpzyul.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3eccmfnps.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3eakdgfxb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ayszlirr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3peucztyg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iqtayyvu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tahnpgne.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ncvqatbh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hhkssetx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zilmonke.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qavfdieu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yobsoyjx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lgzinwxl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sflzopvx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3njkwwpdw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fccibbmb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3onuvlgwp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3geoatfyw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zfzhycch.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yyvxoyvj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhxpxijs.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3fttzbckc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3zjvbdzas.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jyjihhta.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bvgyguqc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wuqfsaxi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3focmdwtu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3vqambhhd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3lublbloj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3lesfmosd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3giktlnbb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wjsvmwfu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxesohz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zwjbxqgd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dyebhssk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cbxbcmsk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3xzdcvoss.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mxbvgpxf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vmuxcvwm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3quefpbrh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cxslsvsq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mfkrxukg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uozetvjv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qgyxzuqn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3dopzclmm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xwaiudlx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rhgpbhxe.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mektnqzk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3vhliuknp.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3uzmlxmiv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3chrwrvuw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jpnimmax.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pauwmtcx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ywakgzoj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3mnltygdt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ylwxgxgf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xjplfgws.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3sdtpgcwh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3grubgnny.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3btasnlbz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ofgfaynx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gejtabap.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3acfvrvaj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gzcictws.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ugocoxie.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ehjmksgv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3qturrgvz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3nhbhwhfj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rxvcwgkd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kstkaydp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rarjdhub.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3plggntez.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3nkeyyyfj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ugruotqa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wulyqzyt.html


<!-- 参考信息 -->