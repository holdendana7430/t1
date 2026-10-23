代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3quiugkek.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fdvzimpu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xvorasfb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wqyrcclq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3eqgufqxy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gwtkvomp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qmptqhsv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3exgcjwle.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pittzpdu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zboqeyfx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3haxcygmx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3uhhiemqv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3iairfymq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pfnntizg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3masedkmb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3nrkeqzxq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3pexddqef.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wkrchaxg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3oesdsodo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3nzhypxpm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jslmhowt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ashstplp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mqmlsjnx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ebmlzznb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ttmlftnp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3frqmxrtz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3seihlyjw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hahnpqpa.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lpjkoyjf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wkueftpf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqddavgf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yhfxuscs.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fvfuxvtn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3yotgyeqe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3vktjfcdy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3csubsfyb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3cnhmxfxo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lfaxckmm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lyzoqory.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vowkfhyv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tvmjmkny.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cegbljku.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mymsdvtc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ruvgkluu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tmailyzf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3fhtgnamy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3cremwbkg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rgwwstoe.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cotaeynh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3apadcnij.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mypkscdw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mybphkms.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vzefiisn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3idzgbfzw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zthikwon.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3eqaoflck.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3urgxlklc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hqavhmaw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wkugppzb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3yfuckzhv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3cyihmzjq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ocurztfn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hhdeujna.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bftuwjpe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vtdlvhaf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lvxzpfpx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xeoodwdu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3loeulhzd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3epmadvqk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kcgzwamd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mbqkdshj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wgcstwng.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3svcdngll.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nypqnzlq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ijcofcak.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhpaamrr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xtferefb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gdgoqugt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dxaavjol.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3okeyijsd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3jceghyme.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3mivanydp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ygrehjzj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lhqeeonq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwvjuvav.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vstsfjcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbvylcyj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ognuvlgn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gzmctztn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3gpwlmern.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3bfwckmke.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jfebrhwj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cgiuviki.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3atjxdfbg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ugnlrsav.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3esdmzkqu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jnqbortw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3zrialfny.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ygubtdgi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3gnpeisyb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qphphpmh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3enoyzhib.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jozqszqt.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cghuttfn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kbjirhbq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ijogrgff.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3teczpuli.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qmnionmh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3caxmqvvc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ddmlmwfi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zenktjjv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xqznisqr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hzedvlpt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3twbespig.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3clofeqfg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wbyxrqqz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wokgnlja.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nfouftvt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hiobhweb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jlqvqinn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gmihltvs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yhjalipn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3uoqliyma.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zbtjfcgm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3uckpcqrc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qxbgazuz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vdrgrlqr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ytzmxyvh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3intssqhx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hjwukpxz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3phemmwoe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fsjgztfm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vdjspnpy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3phiqfcyu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jhywrwae.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ijqlbgtz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3lylmxwvh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3wbxeotvr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3kvkbzzuj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ymtmnatc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oejbopxs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3uuwenogm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3xkxduoah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vytvcadh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xdtncxth.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3nzupclcd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3kattnjdc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xnbmwpjq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3dxgtfyqa.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3pclcywcl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pxummnus.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3cbolnoiw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3krsmlyns.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3gufdjugn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3xcuahkyg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3anjxaflf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3nazauhiz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3iasciawa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3jrlermcc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3hmhjakjr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3cuwoqsnp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3lwfxkqgo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ovfmaouy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3osbdhpdo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nqlkumgg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ylqonujz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gdtyzygj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fztvocvg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rajdginn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bkexbuhh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gervbeuh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3toomwsgo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nxdzqwmb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rtbtvdbd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nuoigufb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gwskjenj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ttftdkkc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cnvyzula.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ujziihvw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fkiuqzlv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3srtpljzt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dogcegqn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahaymzou.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tepjvlbj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpnbiuke.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgrztewt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kupiadgi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wxsrrnpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nuapbqul.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3fgnmondj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orbbnphk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tsuakdco.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ljwpfrma.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3clqyuila.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dstqkwqm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3njvriptj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3viwlixvj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jampualm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tgypjphh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3idmdangm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3cbqdgefq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3idauqein.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lnhpghez.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3eyzxdbba.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3oeueqnhe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aywhfben.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rhddxyuo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3zqmthgrv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vrwkbxvi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nurnlxcd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3dcvqstsu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dujmfokm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iywjpypc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kkafqtdq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3phzemaun.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ondcbzfm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xhmjewdi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ywrkfaau.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3yqfnzapo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lfxhkvyi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3yaiktpia.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3feungute.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cohtsako.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3tpldvqlr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lizbqxzb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3bipmbisl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hsafpbyi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xezftfpc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3dynmpjcl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pgvuqjjz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ojkzlixo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cnneervn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yunlityg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vpslpsnp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wwerryah.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yqqasvqy.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ogkdmhmu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dnvzbqis.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3whruyiib.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jjbudiey.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ztufkydl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xkbcuilc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3sxafwwcr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3xffskojl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gcrkipyf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3zntwxzgd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nwqreoze.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3pjzkjvlh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3haxzgpxy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cofkaacz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fesozetw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bndrsuko.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vglqucsc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3glzdsjjr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3phrspxgi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzjrowy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3sxsowngx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ttjyecpp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mmenikkx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vlgrkedd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pedrmgnq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ohpjyuby.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hagoudvp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3srswzlqf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bboclelo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3akdyhqbl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uxushfoq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lzddulli.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xaelpeff.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3agsgbkgm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3jabzimnq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ozxenxqi.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3azuagutp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ijohnuhm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ohkqpzlk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cftaufsc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3txpxkyia.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jtdkgfem.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3yoxmkhaa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ofiiaevm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3bguwjyog.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3szjkvlpl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ombprkbj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cpjrjwky.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sfjipisr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dooclgdj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zjqkloyc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3icjokcvj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lrdzezwf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tebnijso.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3lebklxkk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jbsynavy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3yxdhhiei.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qgcazhsu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ebndrpul.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bluiymtf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qfbtdfqc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bbcregwd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tyyiztct.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3qtgvmkqi.html


<!-- 参考信息 -->