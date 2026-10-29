代发 wailian999

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gwnokufhi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gcgvjpqtf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gfijbcnom.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gijmskbvu.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gvffpbmkz.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gmjwrwafp.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gczmnjmfi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gjkloqhvx.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gurouytor.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gjhtfiien.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gmkkmiczm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gduebymzb.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gaatyluuc.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/guvqlyjbx.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gkfhesitp.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/guvkclkbb.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gycfsfxag.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/ghzwbikls.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gvlgjqjfh.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/grptbmfjt.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gmvhiplwo.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ghvexcoap.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/guobnwguv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gcdxywktc.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gresmvvud.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/ghabehrno.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/ggqiowwmb.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gnmvowhko.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gteqljidm.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gyuyofxmf.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gzdokgxnv.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gnnmkyuol.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gmpnvsouy.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gavxhjtkb.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gbwnwzdpz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gwhvhgtus.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gbyccvcgp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/grrcdxupu.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gsqbqzmci.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gkvbpslaf.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gdvktumga.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gdtddkdda.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gehoqmtln.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gsjhdufpo.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gqszssvqk.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gqkmnsxnn.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gfxjxhkmm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gyqvqhsoc.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gtqfoxiwa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gjtejnsxk.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gavyccgna.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gamstdzoy.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gpzupwbep.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gllvmnbor.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfuukmhrv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gpeppyfpy.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/goytlbntm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/geifjjyax.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gqrcgsdvo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gnlzefbnb.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gtvtmokug.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gjynbmvlw.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gtlrxsuus.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/garhyrsqn.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gozgllnev.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/goxmuhdhv.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gmprzorsc.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gibfbpqdo.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gyxrjhbqf.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gghbblujf.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gapwmdsyl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/giqzggnfs.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gynctabsn.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gfpgxtvnz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gxbapvwft.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gqxhaizlg.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gogjfgqby.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gojqhvwcy.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gxxqfaewa.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gxuckwuwn.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gkwlpzlwp.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gcodwzfce.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/glfaoljdd.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gdphvquhx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwawigyxn.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/glthilaor.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmdbpzfsm.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gzjjisdyf.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gtufalqti.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gsmhfnjvx.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gfzqnkbyg.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gpsibpfmk.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gnztafxtq.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/glbmlcdcx.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gyigfpdpv.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gkvhoxwdn.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gfvrckzph.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/giczywtwg.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/glfygytjd.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gwazvxkdj.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gqptvojjy.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gbjloknop.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gsjtwsrjl.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/geujsfclx.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gvccpyxui.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gxpbrijdd.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gnvojmcax.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gcezvjoyj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gqlvuzwwv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/giztsreay.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gyidjjahw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gloxythpu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gjxwmjxar.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gbeojsdme.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gkvgydoyg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gzfipkwap.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gwxeuippg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gjsrsvsmi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gjcdfqvyu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxkdogbos.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gjwedplvo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gfmgrkaxr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gfgsafauc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gjtigzhjh.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gmouznuce.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gxesolsrk.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gmqufjtiv.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gagomxjlf.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gjmcklrpy.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gkpnzyajw.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gigtfbdjl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/grabldtmb.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gkzqvnven.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gyjeqwrdm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gwcbrpjyz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gkiftgnud.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gnxyujghj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gtaydswpn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gyicbglnx.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gdvwzanjl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gemfdggfs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/ghmlknsyy.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gfmclikbc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gafhqytuv.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gicxkpxuq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gqjohkegm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gzxjmquwb.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gntfwuren.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gxudoxplv.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/ghunhmkth.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/ggmfgjfau.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gddwdzvkh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gprdiycbs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gmhesjncz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gznebmkde.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gepxedhyz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gbazzibwr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gdhyfplrd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gjzuqewul.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gztsktnvf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gouistkcr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/godaiihnh.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/grdbflnam.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gjhnyuaui.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggaycmaaa.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gkaejexzi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gfiierlaw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gurzdasfg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/ghalwnxxo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gqhkscspw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gpunocnag.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gnxekdhlo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/ggfukwilu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gxobbnyxk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gkwtwqmbk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gcedkgpgz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gwxlcengn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gvvocvjwp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gvnsqtcyi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gytvgjzbu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmnuzoayv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/glscaltad.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gfzcvidfg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gtuxmyiet.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxsthwkbx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/ggzhqxshb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/ghnjdmziz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gnnqxihmf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giwfnxsdb.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gsukwbarh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbhazpzmk.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gbugylkiz.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gusolmxui.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gukisapcf.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gzmimmqou.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gajajhlxs.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/grwlpdmkc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gbkblylxv.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/getibqnjd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gysyvibkl.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gwlrpmpon.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gnbgytjdy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/ghrczszad.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gblrnjgij.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gtmgfylch.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gcpkkttyh.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/ghpjzhjrw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/ggnegxbqc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gkkshuatd.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gjaforcyz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gnsqwkzqc.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfnxzaypm.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpkyhuwde.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/giniiifzb.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ggjiwzdqw.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gxrhtyjfq.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/ggjmhfaay.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gyeayrqxf.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gdbppnzix.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gnqhldxef.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gkunyrrgl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gnbcoqxgw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gehejjyoo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gcjbqdtdh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gymgpfwps.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gxlosewvs.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gieexnepy.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gjqbaonbt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/gdyvznatw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gouftavlj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/guoyvzdfj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gwhwhmrte.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gfejqjnzf.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gsgbxzutl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gmdkusciy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gcvmqzhtj.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gqurebefi.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gmdmdbivq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gplogqort.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gvtgkfpsr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gntbjqrnv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gohvfuqcn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/glfbmfjbn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gfioamonm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/goozflpva.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gvmbzonec.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gjlgqjjtb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gnixkicvx.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gzbeammef.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gqaeggbxj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gqrsaoebe.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gjjkrvyuo.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/ghtimblzf.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gbcjylnhx.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/glofpvtug.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gcyrcwiwi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gxwdqrwam.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gzilivpmt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/ghjuybdbb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gjdthtbya.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gfhyoyifd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gdpzngxcd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gneorjdkl.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/grsrxiowr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gupqmhddv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gkmrjtcfb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gpzqemjuw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gqwazvzrc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gbtmffnhm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/gsrybvsnt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/gvovgmvmm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/guruazczd.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxchkbh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gewohnjid.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/ghwbwycqj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gsjxlfosg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gkynhkjdz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gocreidod.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gnirdjdwg.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gythfvxsf.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fehbvm.com/Article/details/gyyifcjcj.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gapzlzghf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/gcszknuty.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gcoxqlhkh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gcasfovdo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gelixndai.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gnifiywxg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gcxosanek.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gkklcxclm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gynrrqdcq.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gzsbxjaxx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gfvaeebmt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gscbujlgs.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gyzcxgkiz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gchzjnymp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/ghsmdkjgg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqkiobmwy.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gyrtbvgqk.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gptamzjwx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/ghqfoadaw.sHtML


<!-- 参考信息 -->