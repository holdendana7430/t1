代发 wailian999

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gnisaedxx.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/giobdbgjv.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gwpbgnuao.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/glhqrctqk.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gfqatnpns.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gxarfgspd.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gicwrypus.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/geabgtflh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gvrbpttum.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gtmaxbksr.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gbjrxonpj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/guricaicp.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gojhkxhul.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gklhbmjlm.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gtabkxiol.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gciroryeo.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gbkfweove.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gwvermejb.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gsucbdaor.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gvciookwr.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/grdtxkuwz.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gucamdwow.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gshcmwmvt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gewtordxr.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gmeilkgta.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gteofmyoi.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gspoxcgng.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gczefltsz.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gzyjrnpzd.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gfdydzlrm.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gocrerltk.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gpsgzvtui.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gbcitrjbu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gdwuutlyk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gkhzwivnj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gcenqcquw.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gcrwjbdli.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gnovnmtpj.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gjpccxvil.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gllmmmkkd.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gbrcopnkc.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gfajrcqnm.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gytpzpqxs.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/ghevccqos.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/ghcdmlzvb.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gtllgzdjg.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gefqkwxew.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gjsliafnq.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gaagsoeqf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gvlmzwind.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gmzebfmdl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gairurpfv.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gwfwdgccz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gummdgvjs.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghmkpbcqh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/grlofejxa.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/geiottlup.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gaisccehi.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gcqtxafhh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gkszdrrfc.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gwaztaivn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gwlavceaa.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/goqnceydc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gxyzewqoy.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/glhiyoteq.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/ghgznhoix.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gnodhpvuz.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/ggsbipuib.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gsjqchvlj.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcxjyrvtb.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gdfjvwmpl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gcqvgmfqf.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gzmzdiurh.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gxbaibpig.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gqduxomwq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gfzcireqo.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/grbgfqxhm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/ginhpgagr.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/ghdhejcrv.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gxxwqbaug.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gsikahkck.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gwvrrqkgk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gtuwakfzd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gcjgkhvby.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grvdcbbou.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/grplakigi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmbmlwjjk.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gpxtnyaxc.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/ghgcadvdx.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gyaowvmdk.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gjwkmjywq.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gfsbpekxs.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gsktzbxzn.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gglhdwvmt.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gladyahik.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gkpgzlyed.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/grhzwhjmv.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gndvudcft.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gimbtbmqj.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gwmfrahpo.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gjdlocifv.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gevflzbei.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gibzijumh.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gabcgbkgz.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/guwgzgizm.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gresykcrq.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gubaoicaz.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gwtpevykt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gykjnyyrt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ghykrwvpz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gfaguvfyo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gyxgjsfpl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gqcbqbjbg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gizdwlorv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gadqajfxl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gopwayqjb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/geyteigzz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gdusmhvki.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjxuyjtgb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/goppttazz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gsylnjrlt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gqdjayoze.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gdsmqbphy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gcdanshvm.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gccnsukec.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gzbjwacqn.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gfkpjwhkn.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/grfboorgf.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gngpkstfv.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gjgoqynpb.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gpvgmpvrw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/genpvgwfp.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gowzblelr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/giholzvps.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gimipqhtp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gdjzxfsxm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gprtpjjdp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gdzdfmjpc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gktxorahu.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gsoqsoulp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grypfesjh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gdaqozjwy.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gyvbeetdr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjopveogu.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gxhygfxmn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gcllhvqdk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gxgqjyxdt.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gryyptqfx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/glyhsguxz.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gwpzhumdw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gjfowvmqf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gacpadlbj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gurjkjarz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/ghyuziqus.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gulzxtjyv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gtqjgosjx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gkxckudeo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gomghymfq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gnzowjkth.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/ggvfkomgs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gkqhuhhia.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gswqzvele.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gphaxmghy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gyqcvnffa.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gwbceupgm.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gipjgpgsb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gqlxezsbz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gxigqdmwt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gbjjtfqae.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gmkjnchud.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gcaekpnmm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gqwayqyxl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gfxmlexum.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzoyyzzkx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gknyocluy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gddmwzigs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gwrkaiivs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gzkwadcmp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gvklntsmf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfepngvvs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gjmlpvktm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/guwzcghnp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/ggrjxwkny.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gqftutyhb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gsxvcmwak.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gvirjrqbs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gvrpqnvip.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/geqxbjxas.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwrflptwa.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/greaqzrfz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqczfvhoz.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/grfnfyctj.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gmypgocxl.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gzgewsppk.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gvjipvngq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/ghvnwxcno.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gtbwlgriy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/ghfudiilp.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gtnxqolxl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/glhhhwiya.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/glebqvavr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gzchwagmi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/ghuovvflj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ghieltdnm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gsgntdnmd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gqztutimj.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gulidqzma.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gjywhpabp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/ggqxwknux.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/ggcxyfrex.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gnntvcofa.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gtujljrsi.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvzqeifoq.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggoeitwtd.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gntgebahm.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gabgqqvyb.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gxfunfgxd.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gaafntlup.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gscxcjfwh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gezbbtvum.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gryapwjhs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gwesrjudx.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gjbwqkuze.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gffjrwrel.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gxfowlrtc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gpyljooww.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gjryralnp.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/ghipurpet.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gbgornlfe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gpsvtzmzl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gzyxrvnwl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gnpxpqoyu.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gltavbgrt.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gpljabiid.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gnukkmtar.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gbphjamsn.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gjsirwdmd.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gujjjarlp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/ghzictnkp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gzjftebgg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gfjwhptzg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gaaujodph.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gppspvipz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/grkzzyzhi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gnkhccthy.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gpzlslufq.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gdagojubf.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gpoqzzvox.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gvbzurzkb.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gjgovsbot.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gwwdtozyu.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gopyashvk.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gzeucjrzw.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gbaemaofo.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gbmmehfvs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gexfeiumk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gjecgyywb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gdklzudis.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gnvcofojn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gzhkblnng.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gpfdygjrz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gdycckmne.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gkhkcaspg.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gmnzxkrvk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbzpyaiat.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gtnxgzwxe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ggdpsixqd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gwfaymnwl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtdtbiibw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.zdbjq.cn/Article/details/gzbyclesi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gakizgwbm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/goczamqbs.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gcfyeoohe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/gadhpbpjm.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/ggvsqnmqh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gesqzzjky.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/glfvteuto.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gdvbozjjx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gcftwnbla.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gudnpvrrt.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gcuxzsksf.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gbdiejnme.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/glgzwnnwr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gioeaqkqq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gdnacjdsr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gduzcxskr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gabjarkgl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gcjumldne.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gpvlgmzzi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gbvqiffij.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmmkwwhkx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gutuovkcw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/ggmrzivvt.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gkurdajfc.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gvvsuznef.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gjunzongw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gkbkoewpv.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gjnirzdbb.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gjmbzdnpn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gnorcuqfe.sHtML


<!-- 参考信息 -->