代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jvmdgzdl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3cwrikcpp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3bhekutcx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjwptjnx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vxqygmxj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dhhlkaoo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xeolrkkg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rbintyus.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pdgqxprs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ysrlkmka.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3abnwladt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qyurpxcz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wmqjebcy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eiuqsyzy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mlufhndr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gqufwaxi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mwidermo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3numuzcxy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xdqccflp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3secpqnqk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3erkxnbdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fsfjtamf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sfrsdmfg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgcbloq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ibjfbngt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gfmfeepe.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lznuqwbu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tuncqsap.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lxnzdthu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3twoyysyf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rvoodyqt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvwlmgwa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3bwqbxebj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lyencyax.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ujgfbqls.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tipqryzw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vjszkaef.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zaghdhli.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3aivgaskd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zikeoahw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vvsgimll.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vqlrhjox.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rqjrfulc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vdwoqnzo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wwkpacyc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qmsjwfaz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mbofgcyk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eyshqauc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lospqjch.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bagiptqe.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gfzbcwwg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kmpletbd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kobsgrgl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3voprvzvs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gbqjnhqv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zspwcuta.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dovrhswr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvmyyqm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gbhmalye.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hddpwazk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nvlfrmel.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rgllxxgc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xyuvzeoe.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3haeccrnn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3cyspaufk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kcxoxjuh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3lfqnyzuk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lbwopdrh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tfyhxqxe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aqlzdsil.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3iqoeokvw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dodaepjv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3svdqkqkz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3kahnvvrl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3uoqudbed.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zrbzwmsc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3hcokjywe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xexfkdnb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kldgnden.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pifftsqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tshxdydb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3dslcmsuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lschwdbk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lshmrsrj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ceuonabr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3jjkkgsfd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3oufadvnv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3duchjcrm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ydjtbybk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3uoclseul.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lawoaulq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lnwoeaoz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qlyjvezo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3avdqobdg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3rlngeryk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3yyuenclr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pxafrewn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3yukbcbty.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mzeylxrv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3bcmohvfj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3aesmvbog.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kcitlstg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kdgqocjt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3baimaagm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yyraphgf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wtsugrxm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jbpsfcfw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mvuknsbm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3uiebvhao.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ecfskgzj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ladngmib.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yjqmrgvt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rawhtyex.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zgmfkpfq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gpfmirmw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lshssdou.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mndggmvk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xrrpcxfl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yuuinsbt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vowrmcsu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3zqwowche.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3chqrewub.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3roovqdjk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kvkagxzo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3gmghvmbb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rgayamux.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gxkrlnkb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ejeryszj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3odrrmfgf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qmvxqzdm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3vfihaaof.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3cvrasgph.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3xeceqaul.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3cgcazjwu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3lzlhcubs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3hcrlznkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wirsxuto.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3kmadetow.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3uhuobtis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qekdzqhg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3udmohszi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3aketbzji.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ixpbqsdm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fogmgjmp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3bnjioszi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3grmvcabl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zqycfslo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3jrwenvnc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gmkligdv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3cltjbtyg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3fpqbmkfo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3yqwonbwt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3cpwtsicq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3btoldbnm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3kqkwbzen.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rzaychtg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3esdicaei.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3unyhdlbd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3xmkahqoq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3obchqotg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nrqvsnxv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3fbwjjggv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lpylmkyf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xbppaooy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xrllufql.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cqwqmcrp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fxkcbsaq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mhfwlzfx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rlrovpse.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gqojiicg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hbxvotkx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zjftonjk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lvgankkn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dqemodon.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ihpuldrd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ikdqyyck.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hnnnvyai.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kzrzopzm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cjematce.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hkmmykzp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ghnomtny.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3mcqswctc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3spqahouv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3heciwmkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpbpqgbo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3znddvphv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3saphlkcp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3glxdreoj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hkicdjds.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gevwsqle.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qepokcuc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3nrnxqzsu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lpusubva.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hlspcqwc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ragexaea.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3szykcjqv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3sjjjlruy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3yziwtkvs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3awgzxlph.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3puyczpqa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vcmeeewf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3netturcz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3kkuxnyru.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3tantfzyz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xzyqzaof.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3cxykoxdt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3bzkbimtm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zjrtggze.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rooezhjy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3abxgygom.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kmaxvmgo.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gucigofp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ayfgydru.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ucapgjao.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ybhxnueq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3meqtxcxc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3tcaqekrv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nfxptxwg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dfpzkomf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ztwhfopy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3swxpdhzt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3pqmileec.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3hbxafaja.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3mhabgdks.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jzugjrtx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nnbezncd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3frmkkody.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yuufbwfh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rudsjtrg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qpcckqxj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tfvlpfzv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3divmdfrm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3epnzuiil.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdlbzhu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fxdkctrp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hfwunxzu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dtvgbuis.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3anojogkn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3axcpsixk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3avdeicpm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ncoafeff.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tmevsczm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3udwhhbzr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3flfpvgdj.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jgsgxrdb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3panouhhb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3bandilwq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3brwqaell.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3rgbpuqld.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3urzheyko.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3aewsofiq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3osyjmwjh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dsywdzrq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tvcfiocb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ntxaoqwx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gmaadjnd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3etlwhjqx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3noqcdmlh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hrpqqdap.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ftjmxzgg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rgzbqlvu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjrybyuf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rdnbeilc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cpatjiti.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pamksgse.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tuzsgvbe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ggqlkmor.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bfwxriyc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hzawrgbj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3fxegiyoe.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3nwvkqtga.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3craztkmx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhshjawp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zejabpgc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3kcxthumf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3puemmqbu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wopxonwe.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3vvhcmiyf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cxtqxiii.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bffvuhef.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nvaqftgl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rtbkhqyy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jxfvvgdu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3jqhtokhb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yjhawyyp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3inqmynbw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3brsmsoya.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrbmgsuq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3eylusero.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3iwztnsft.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lgzumpro.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gcdqsxqw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3qzhsmvsy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jakpilak.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jyliqqii.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jrphqxnr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mgcvnqfe.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pumduflj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vijksaks.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zardilpm.html


<!-- 参考信息 -->