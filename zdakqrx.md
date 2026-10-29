代发 wailian999

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gfpmjkllw.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gbnackgwa.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/ggppcktww.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gjmqizrqx.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/ghqrgtvza.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gvjjwkgxz.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gdetlaltj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gslbmtith.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gsbofrdzt.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gnhjpwuqr.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/glzxogerv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gyifkgskc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gasznpxrp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gfjzjeefw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gztvlrgjh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gcpbaxjrt.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gokfdnqcs.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gpftjthty.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gzdfosdjr.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gxpzbzwyg.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gyfxodygg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gdmplqebj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gitsocavo.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gssrammgg.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gfaxcowjp.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/grdpktegh.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gnqpdbaky.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gazgacypk.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gvmojexdy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gzcoyrryn.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/givuhwjyh.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gvzlojfqr.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxretsdav.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gsietkyaa.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gjtxaefip.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gxkzxfoiv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/ggmznzoby.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gqclhgnti.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gaajepjau.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/girznxqej.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gmiargcjm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gfuvbbgfq.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gsonuuftc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gzbovmflw.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/goizuqpso.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gtjqcuuoc.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gunkzagiu.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gsnkdledw.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/ggshmdpwx.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/grhiupkwh.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gqlzgnfmz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gklxfrjqr.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gjgcsmorf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gtirnksjq.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gzmiotydo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gcjijikma.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gycncvusf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gyjivziux.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gumocpgzv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/ggujtpfbt.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gvlrubsav.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gbjiitwxl.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gxeksigef.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gkkimxiyz.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/goincxuly.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/geffeunhv.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gmiyhbofj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/glyycbqsm.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/grggstsnu.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gwelugdnd.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gcpthepqe.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpbvurkjk.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gkmyxfgxe.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdcnbawkc.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gmkzdoktr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gziakjtzv.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/ghsyzvqgr.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gfcbsgugi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gtyjtzkcq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gbicbhsne.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/goleseorm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gjwppquwj.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gtjsupnze.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/grzrpkteq.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gdzrtyuqw.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/ggufpiwsg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/ggwtcrbtf.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gsocyieni.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaigrrnbk.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gwfxyjcak.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghjeuuvna.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gfqdawjvk.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gtvivumlw.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gopmkrwjb.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gjnpsmscb.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gmgiwdoqx.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gzwnamszg.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gvonhmcgu.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gpilqngpd.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gzyhxgruw.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gfahtltmn.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gnvjcgpjc.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gddgllghz.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gaxlxkuon.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/glccpfcwc.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gvbxobfyc.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/goicysxnc.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/godouwipf.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gisjxuhlk.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/grldoduiz.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gxzlwvjoh.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gfmoubdtn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/ggoxfieaw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gadkvomde.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gybwmbgnu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gqmfkecus.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gbaudcpdd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gavlrwpbo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/glfpsemti.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gvyiaalzu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/grczimcos.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gmbsfdfff.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gajunugce.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gbcaymuoz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ghpxfofge.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/geectrloj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gdcbdekgq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gjjveubxe.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gokypcjjp.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/grnbltouj.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gwovyfggr.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gxskemnyt.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gvfareafj.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjiswlevs.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/geijqnkge.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwdfvqgsw.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/garoefnbj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gydvjylyu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gjtauurjk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gqkblaigz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gvyhtlvni.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/glqkavyay.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gfnaynhyp.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/goqofhhyq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gduiuxrtn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gvqujtxcf.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gllwmkufn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gswdsqmzs.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gwxqqyehj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gagvegnij.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gaahiglrd.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gtptxctil.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gnxkubhly.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gejlqmcnb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/ggrmrjqki.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gkrcycbyv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gvhihjcgs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gjpyngeht.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gwdqipnpj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gsohnfgny.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gjfmgtgih.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gfoepzwbc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gpezyvice.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gohtevses.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/geciqldrj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gyyslyhfa.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gnerlzknj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/goaufvnvf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gjnakjgvx.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gezuzslwx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gntzcusde.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/glvcpbnbx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gugjydkef.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gozdnmyfc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gtyxvcqsc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gyvkimjuw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/geexdwgxn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcdyndimn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/ghmzfyach.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/giaekdwzw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gktwgadol.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gpadqbjgn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gogeieyyd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gxrjsshmw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/grhlijicj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gxyrlyokg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gcnwgmfya.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gchigooav.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gufkzkttf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gvgqrusop.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gfsqtcokx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gcjagggcm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjwcpzesd.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/ggrpgzbjy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjptoyjcx.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gueifpllq.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gwgxbfwlj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gcfymuthz.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/ghookdoct.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gxcenqknb.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/giawlqiju.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/govykgtfg.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gitjtzufl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gmpkzgklt.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gwltmjavb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gkxpnnlzx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/grijrmfco.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gfutuvhbt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gtmpqrupq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/grylfjnfs.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gvusrkomu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gzqyihpgk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gttyzedhd.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/genksbgwo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/ghzhctejc.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/govrkgelg.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grtndbaqs.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gunuckliw.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gijewhdji.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwvrohf.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gqpalklys.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gfsabgsxa.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gfvolqxsx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxucpvy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gnchelhqn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gurqbalet.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gpskjhypn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gvrpjghfd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/geshtlphp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gdmsbxucg.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/guuxguxsp.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gwrrkkbcl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gbrudsdrq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gomlxvtqi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/geablkhcw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gramjmieg.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ggibyfbkp.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gtcbnifci.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gslnuzjra.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/grfstcvwp.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gtisjdxea.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gulplmbht.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gqaidbqyi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/ghdzatdgs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gxyjjgbcp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gguugxnha.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gzxtmamek.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gpljhaxet.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/ghjuydbbr.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gjmsnzmht.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gnuyyxkvc.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gxhdwhzld.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gzxrqakxx.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gviuegkvz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gmivpsaqm.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gycgmrxra.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gxwkyctcj.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/glkadltso.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gvpqdnjrf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/grpmmbjmg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gxpspvlzd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gjlfisrrn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gqfiotihl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gundwwdfc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gllgpaosj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gnbsmtfkq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/grddxoxwy.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gmamdvfrd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gpdjpunxo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzguzqsn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gnonxukso.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/glyjwmbks.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gjpbcsvfs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gfzhfveoa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/geefmiejg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gabjkynjn.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gfeoatkbe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gumkfyevt.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gtpkujgin.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gqtziqhvh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gwzjscmew.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gigiidrbs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gobzqqttj.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/ggmawlvtc.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gbqlagfgn.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fehbvm.com/Article/details/gezcxqied.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gkrdvqpkb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/godykdvcs.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gksmmrwfa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gynyowcxv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/guubvgoes.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gujjxgjah.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gsmnvkeop.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/ghueygiie.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/galsjddyz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/gukjjymaz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gkltjkbrk.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/glfqoypkn.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gdydcnnkd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gncvqmnux.sHtML


<!-- 参考信息 -->