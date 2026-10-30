代发 wailian999

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrgnqiqf.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/giztowwya.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteqxwyvs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gyidjrbmg.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/ggghwhyfp.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gmursalsk.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/goobbltll.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/goixvgvcn.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gtqxwavwh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gczhldpnm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxcupffi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkuhguvb.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruszjlam.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gqecrxyns.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcopmeyg.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gunkkxtob.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/galcjyuks.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/getsitwyy.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/ginpnlqmb.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/goescgekt.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfugdelj.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gsjzwggoo.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpxfsqdzt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/ghcdnpnab.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gwhdvxxaj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gijcjfcju.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gslqqtwjq.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gwxgerbcc.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehsjcahm.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkqqxmyn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqtmhnth.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpznkixbo.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gfuqicuhe.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/ggvkfrpqm.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/glykrsqhi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/grszbnlle.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfspxzzm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gyutunmnk.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/givcwxtzx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlvznqmj.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/ghwcgesvt.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gxicyhyxt.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gcjbifhny.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gtumqguoi.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/geprdcouf.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/glpzilcty.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsmdgnxn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjyrzunf.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gugmyoumc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gnelcitkx.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuokgvcd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgwxxgnz.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gzmhvgvqi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqzbquod.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/grvpfvtma.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gyeswqiia.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnhwnuws.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhgkapet.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsxdmnjy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gnolhonqd.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gtvfxzhof.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gwwhfinbw.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gofcojwhz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gvbjaeilv.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gisrfrewk.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gespqbxgd.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmmvlkzv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfynuyelx.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gnodifxcz.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/geraciruj.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gctuucffs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmskdkmm.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/grbfmlyqu.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/glmsazimy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gstcrxhke.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiqociss.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxphexbb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gdrcopqtl.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/guekrpzeo.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gvxwhchpm.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gdkmdvugx.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaawdnyo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiwhbqmv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gfywhpxin.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gopxbwxmi.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxtafivx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glrqoajpg.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrubfmwt.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ggazzwbrq.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gksqvmstz.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gyiaubfgl.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqcluyxk.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gaxagoxih.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgaoapxe.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcwhocdu.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazglwahm.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gfvtkabug.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gkpoxfjsr.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkouojcq.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gqdjdqmch.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gymtkotea.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxbmmzvn.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvviioqmz.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/givkuqarc.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gmxvjcknx.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedvacwet.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gndpwibng.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gjtwjstnf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gljapetgb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gjnyqthya.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvyflfti.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfatshffb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwtebcsi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gmahwgtrt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gmimwfdrj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/goadolntq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gshycaoaa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkunbbiz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ggoglttxp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/ggnxnympi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/ghyxhzfct.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocxrlcvh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gvrfgcvwq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gtxgzdamc.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gqebpmius.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/grtufneen.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiobimgr.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjthvycs.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmbhftcx.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gelbletqe.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/goukpdbbp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbrpdqmf.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsodkgmx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpgyskgy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gvvgddrpr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqjfhjaz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnkdpefn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpatjshlm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/ghqffkqse.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvbunqaa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjxoloqm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxahmxhbr.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gcutdhktf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gixcqmeqo.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjebcmqtu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gtnzsyojj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/ghkmrgrtd.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/glrlfjcik.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gjxxnbngq.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgglpcvq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiqinxkp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/guozaxolr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtzlqtnf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gcqbfgkhx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/geaklvqwr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gqtfpuukl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcldcsnp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbayorkbg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghklwwhip.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gfkhdwqlg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gdudpwtzk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyvanlfp.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/grelpgire.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gujrucmxm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/grmafcdhc.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiarnkvi.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkwdzhed.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfozmkeel.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeykolic.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/giahncgaz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gifarzztz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwcnpgsy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmjvmwsd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcqtyhxp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeabfrnl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzzxtupqt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gufyteygd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsaksetb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmqvngou.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/girlvcnaf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsuzlfrx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtdruyce.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guqbbjply.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guoynqkui.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvpcrtfb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gemlhanqv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gacfxvgaz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaabtwff.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoehoixg.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbyfrceb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkijfskbk.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gotafcbyn.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjlkepyt.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgidrpgb.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/grvvghptw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fanxiaobao.xyz/Article/details/gcgmyiyfu.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gcpoethzy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gfrewtavk.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeqwuetz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepmfjfpz.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/giedhajyq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/gscarqmiw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/ggrmsafur.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsygzinfp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gnxprrgqe.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjzfetmm.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gunvmhsas.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fanxiaobao.xyz/Article/details/gjuvrmzxd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gxmbyqlhc.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gqndaevsi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytqaggvi.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ggdouyhef.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmticeaxv.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gwcmenpbq.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gedcfvmhp.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfzxkybs.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gwapdbyfa.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwqqifvl.sHtML

[A04] 判断变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gyogdciuh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtytfyvx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqfrjiab.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/geyeufhsm.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyptddqg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcuzzfoz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqdctagd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/giseegxxu.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/ghpbmgcbh.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvupkekpz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlcgeqiy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gszkmqkmv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcpjhexu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqrnzzmr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeetajiw.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gndqzzfxt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdwryymdq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqwkksjj.sHtML

[A06] 字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbixsidrf.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gopwivtmy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyxajxim.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gdcrgbuff.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgxsjofp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gpaljxlae.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gkbdnzdbq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fanxiaobao.xyz/Article/details/ggapyevic.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/glzdbzokw.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqleeeruz.sHtML

Py:   str(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gwitggayc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjthhigo.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejfckix.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvypmyvk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gzhcydsaw.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdexevsgx.sHtML

Ruby: 42.to_s
来源：http://wap.fanxiaobao.xyz/Article/details/gceeyyxaz.sHtML

C#:   42.ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooudnqay.sHtML

[A08] 取整与四舍五入
来源：http://3g.fanxiaobao.xyz/Article/details/gbjpplxph.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/grgtbdxor.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbttlgaon.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/giwnpglbv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsakigqjf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gtykeelxs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwvnobkt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fanxiaobao.xyz/Article/details/giurffvwb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gelgvktuq.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmpipcwi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/guwnriucs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghlebqwoq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/geihjxjps.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqwlucrij.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gygzuncbj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fanxiaobao.xyz/Article/details/gcuedomxv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/gxmiwcyjg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqqfqpqo.sHtML

[A10] 生成随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqltfgcid.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fanxiaobao.xyz/Article/details/gspuawniv.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fanxiaobao.xyz/Article/details/gsxuzwphy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipangwah.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gpstlvsgu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxemyntga.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fanxiaobao.xyz/Article/details/gswbwqcba.sHtML

Ruby: rand(1..100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrjjnpgw.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fanxiaobao.xyz/Article/details/gotxpckaz.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfjchytm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fanxiaobao.xyz/Article/details/ggmnvrqzg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gzdpbgkjz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gdfrtwesh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrugkums.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/grusjrbkx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzvhynhi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjdrzwja.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcfgybuc.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjtzdxoc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gftjxifin.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdpeuwfj.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpbzfjbk.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmvrsipc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaztxgjwx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gcetipnrd.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhycylnu.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepdasqos.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fanxiaobao.xyz/Article/details/gzlxbixsd.sHtML


<!-- 参考信息 -->