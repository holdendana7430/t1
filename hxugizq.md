代发 wailian999

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaslktvo.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gersqekli.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfwxoapl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/ghezffwlf.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfywwshly.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvhhhrma.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gjlrzukjz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfkfkmxd.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/grxgceivq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdivflpz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnzrcfpr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejsvputl.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gjukhlzdu.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gtazvwelm.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gitvzkbiz.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoyeishc.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gplttrdzp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpanyjdz.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfypbhwe.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gertawcdc.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/grmwpmdhs.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gbzmnvcmw.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjstvtrto.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gzxpyqjcw.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghdfxcrjk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gpfcebtwf.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgsunpmi.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gfrnluthx.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztctyhxz.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjneokfu.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxhmulyx.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gnioakeox.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrfpftlq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnyudmba.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjkqzyyr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gntlvuuuy.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gpdhlfxrr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gntjpycae.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/giqldpwfb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqirzcig.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gegxqygnv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gkxizckkl.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gxfiajqmq.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gmghamebw.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyihmytg.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsrhkbaz.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gjilqumri.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gmxlpciku.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsgfwccx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgzblrry.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gauhvgzih.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtfkwxzqy.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxjjkyhk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqevhpaf.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvernknfe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gowazgjhb.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/grluvhyxu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gkpejdqhg.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfshwxefe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gtcxxnqog.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxhnhkpn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjemfjrp.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gitrsycsv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuwbgjci.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/glabhbocx.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gpqpjnsop.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gykirqcwj.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gwzttcwrf.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqdkzctp.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gubkhrinc.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwskdmuyu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmtgwjkf.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gvezzlbad.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gntlaxwue.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gznepdlbz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdrkyinqr.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gwymrxsxl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhvzjmid.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzmrxbjl.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gynmvgvxl.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gflxzsrvc.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gigxnqwpo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gumfzdepb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/glzafddiu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgsqplxl.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/ghublnqhz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guhptjhqr.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gogipxcyq.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gfiziixly.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/ghnyblpoo.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzozlmtt.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcikoief.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gwneoflgj.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopxmbdur.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gckoyfrjy.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzabubji.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gvynxnixv.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/goutuccab.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gjwqbehvx.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gzfqjmnjv.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gakeoebtq.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjijzbnr.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/giuhcxfal.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gfebrwuzj.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcopbkdxc.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyjfmxed.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiunpdme.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjehmgfju.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/goqtdlbgm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxtqychr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxhmqygu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkapkvixs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcxwuxdd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqfcaawo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gvdizpuma.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfwtwezw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/glieqcgju.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbgibbdq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbheojhqw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gakzorums.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gwjajjzsi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gaevmxzci.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gejlndrww.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgxfgbfd.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/ggldsjivw.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gvihnvelx.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gcptcipqc.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaxpbwtz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxavzoci.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gcqqdnukp.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyrmbihq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrardgju.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gkurmaihd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gckeiyvnu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmzamtak.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/grvagchxa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxczgndq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvqedfyo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gszekwtno.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuzkqkxl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtqpdhbjb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gwtfpfsgz.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/grsxkeuvi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghgyluvvo.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteukjxsm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gedpoewrq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gabmylqgr.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gttwlfmyg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgprupgs.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/grvskypen.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gzuqspzrb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruwcjgth.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gqyygojka.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmlpedbl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpxzsbvq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdasiflqz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gjpwtgxjb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwowbwlo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/grkqdkfxj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gnrnyysdz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynjxobpr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdykzbcve.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohfrtlcn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gncwlowsz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gsfwbksag.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjkubjdc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/grpnglfgb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpjzgpvm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/giogbjsir.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjytyeqf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmhlmvkt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glplagyed.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhopvxvh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gxqadmsgp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczlwftcy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmeuhawm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwzwdpne.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gxzuyzeum.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcgqaten.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrktdpgw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlrclegk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhsxvraz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndouwbyh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzffuisy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/guuyxgpqo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gothsiljp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gfzdrugfv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivprbrp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjtlzyaf.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/grpxvneeb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getwdkiem.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goenayxze.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfmpoghq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gmilpeydp.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gtlubkouw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfikxljix.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvpmbrha.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gykunvgfj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmswnrogz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gbcgkxyfl.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjjmkaew.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/gqevsojrx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrhtfnlj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/geqmhzpsj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzqmownz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gumuikero.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gzewblspz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/gbosjwree.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqvgdpfc.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gysyqqjkb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/gtelplhbd.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmkimtno.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhwnqvkh.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqupbbjqk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrwpavfl.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoxbwxok.sHtML

Ruby: PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gaklbcqnm.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwpshnmbh.sHtML

[A04] 判断变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzxjgqzo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fanxiaobao.xyz/Article/details/gqhweevqx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhkuqrhg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gpigyxzxu.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gyzyotndy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzrzgize.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fanxiaobao.xyz/Article/details/gyiehdqkj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/gntmzifrt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwacmpnqm.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/gdlwlpvqm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbctvbacu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/glmggttue.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzokymoad.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/guyoxgnnl.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgfqpgkf.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gksmyollb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpsadxhl.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gicptqamf.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqdzaubl.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/geexpauuq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/ginvvwriz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gyxpqryng.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujgwvte.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrvqlbsf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwaztrst.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gfaqxilwj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcmhxfyg.sHtML

[A07] 数字转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzimyacrk.sHtML

Py:   str(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gealfdwno.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/geikgiqty.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwesyuop.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghckaltsx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gnfqgsxly.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fanxiaobao.xyz/Article/details/grnieyfqw.sHtML

Ruby: 42.to_s
来源：http://mobile.fanxiaobao.xyz/Article/details/gehxjhyph.sHtML

C#:   42.ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/gnrolknks.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcxbmcjk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/geawdckim.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fanxiaobao.xyz/Article/details/gknwoudws.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqjzbrvt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieothokr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozqnliyg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gtobyqvrp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoiisgam.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gclnfisjp.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gygeyoosm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gywwwxmox.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmatvtnzu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gkjqvvkko.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gaesdyvfq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgvwowgi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fanxiaobao.xyz/Article/details/gsncrgpkc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoaewqvu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/grgailpvu.sHtML

[A10] 生成随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfpwxgvv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggquhcgae.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjuwnlrw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotdbwxed.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayveokgt.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gknrulkxs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfjydppw.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtktosqe.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnviulbn.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fanxiaobao.xyz/Article/details/gaaznbylr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqnsrfgo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsopcynin.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouuwpumt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixytqdek.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gsspebnga.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmgygtvy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gnspklogo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtriruwt.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gunofkurt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgpuezoh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwbgvgml.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fanxiaobao.xyz/Article/details/gslmvfwkt.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/gzovqlmrv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpexultfs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggouftrft.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gitfcezop.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzphnqqbj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fanxiaobao.xyz/Article/details/gppeksdwe.sHtML


<!-- 参考信息 -->