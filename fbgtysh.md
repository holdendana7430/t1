代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gyubzfqqr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/giudvviex.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gneexytlr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gavhugsbg.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gbopkfbuz.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gyybdhyfj.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gaigfqcrk.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gwhyfmttm.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gasqszegy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gcgzttokf.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/glxuzfsfe.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gcvbwdyks.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/ggzlpogih.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gawohnlpf.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gwagdsajq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/geomumbqj.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gllntbbzp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gfwtnrvag.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/guvqvmesl.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gyiorceqx.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gaxdrjdib.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gceebhfrk.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gctluogty.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gdpuypmoc.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gcvqnurwe.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gkdjuvgxa.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/grdhxmhjs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gwspyxnpi.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gjayxmaxk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gtkouhght.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gvjwllgrr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gqbnkwgmv.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gcraevqqy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gzjslflxz.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/ghnpjamea.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/ggqjlwnxp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/geraixmsc.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gcoeivqzc.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gthweeetb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gxjvvmphx.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gqjbzxcbn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/ggkjqlqgo.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gnaakdyba.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gmejyedfi.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gdknbawzu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/grlzogtyl.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/geoqgfztz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/ghchpubxg.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gqpjxixhr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ghhqvemnt.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gwueqcwpy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gtrvvcttt.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gyndquaah.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gdimxztev.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gtulslerc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gqielswtr.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gmvdmcbih.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gbofmunwd.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/guytbaxwo.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gybxmmbfy.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gkhxdkrqa.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/giazitrpi.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gmifiuqhx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gioadyszk.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gdpjnfcqj.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gogzsupqw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gamassrbe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkinahejq.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gtbwmzcbk.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gosakubhp.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gijoqjmth.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gketdrqlw.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gojjzbvof.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gphnrigmk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gfqzynibu.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/geuyzdfyb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyhbyercp.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gymsxytzh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzphxqrtz.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gbvdtboes.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gjrqkhlza.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gsrwhjbbr.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gnqguzptw.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gzymiwwte.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gijtgqjgb.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gvxoobddb.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gbupnqznc.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gqawxtvtf.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gvsjjqxqn.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gngchrhdx.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gtjgbaupc.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gjweuvlcn.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gnjigssae.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gqyjsrrlu.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwwqxhd.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gthvddjoa.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gfvrvxjcx.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ggzkpbmhi.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gyagnwpvc.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gtqrrcusi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gaxptvvfy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gwcspgwtb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gogtsuoxe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gabflsupf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gdcjefkqq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/grgrviziz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gpijvvfrf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gqdtllwcp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gkvlptabe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/grkorzbdy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gcthjmydd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/glybgpiap.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/geelqzxvp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gljmxbwud.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gycyfbvvh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gszmuiiri.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gfnigquub.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gqkepkbkg.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gnprzwssa.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gyqclndde.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gdrxfperd.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gucdhdclx.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/ghrtexurc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzczttytg.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gswpyouno.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gvcdytigs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gjhzjqojv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/godvmnagi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/godyobagi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/grftaezpg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/ginslctep.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gotzdyszs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdcvambvn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gmuxxhvrj.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gzrcdjvlf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzxgohifv.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gehqvmiji.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gswwnarde.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gntytrtvy.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gijqpqdha.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/ghcsrmkxh.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gygbnxbns.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gafijnwgk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/guvtdgufz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/glhityveu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gysqhuvvm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gtooatzpg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gbkmbtssq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/glaifhwan.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/geuecaxbc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/ghworitil.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gqvegqvlr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gilfqnohw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gxwyikqdv.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gytzynqot.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gapsdshup.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gthxgtyem.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gpmhdpitf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gdmcexddb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/goraixrtz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gyjauvksh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/goiycyzui.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gdsgvsaom.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gnzkywwxi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gxtpaxelt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gkoyklkvw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gixzldmrz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gfgaimxoa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gtihhcxfc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gzgnlooyu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gstooricd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwtyogvdf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gomtbmurc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gknqcuxfl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gevyuxrzb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gryjtijuj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/glsyugemm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gckaqihlo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gzwvpjyuq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gakcjgyzt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkunkokpb.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/ghdwhsckz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsqbdnkxo.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gwlkcutmd.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gsipdckvg.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gvnbhclzz.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/ghiejbdrs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gilerkqrb.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gxqwpjyjg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gltsulfis.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gknhhuhez.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gpvoqmhyj.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/ghbsghknl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gnsqthcfo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gzqhebxcw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gkauiudmg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gscmyzmvq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/ggjxvrzny.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gfhagtraq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/grvnimpnn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/geflyeyvr.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gbahoqqec.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/ggytfiuwp.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gdgfqdqxr.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ghquywxin.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggvdofxbi.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gchiyhdpz.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gcafzadpf.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gqtkwhzcv.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtaeumgny.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gxolgqyjy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gpoqvnogi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gbkclmfcy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gsfdmnqjo.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gnjxffcdo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gogsvnjnh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gtebmxwpo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gnesppxhd.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gilqavsnk.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gavknfdov.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gmxudfhme.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/ggxvdnwdm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/glfatmept.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbuwalono.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gwgrgsuku.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkosovnkj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/ggkbutpph.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gpuzouxys.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gzgoblhmf.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gkqywcqmr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gpvaegjpw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/geludinke.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gvtbrxdlx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/goscalxbb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gsfzgfbgo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gdkqiiefi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gqmrqdzeg.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gptkweedt.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/ggdnktywy.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gbxtyicfw.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gtilfzxrh.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gvafphlip.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/grjiqxjgh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/geuotkqfx.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gldsemiwa.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gtanrrzbx.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gnnicqotx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/ggiyxfovf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/geahmbeog.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gpmokfdpr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gjjuzmxqp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gdsfmktqa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gukahicrc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gzwyceziq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/ghdakoibp.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gpmcxmfdr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyrefwnnn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdhwifiwk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/grrtwatxu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/giksyvnsz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gnmweqatb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gstxnczjd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gypfrpdqn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxgsgszuk.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gbuvsxocc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/giuudazkn.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gexbbxocx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gchfodrey.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gcihfihki.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gzwflexst.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gnmbqpmne.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/ghiqflyaa.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gmxfgxbwt.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/ghahriiak.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gjgypehup.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ggxbnfxzk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/givvfqdxa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gftrhneuh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gtozyhyoj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gnluxahkl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gwmxuvste.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gsiufscnf.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gbhuuwkqm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gsvakoyry.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gkbxsitri.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/grjbgrmrr.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/glavtqzsu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gemhnnwoa.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/gbybqingg.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gdemdpzvq.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/ghmiibvuk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gpbpolfxl.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/giwpxhxcz.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gzlgdnxoe.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/glvzyelys.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gihdkmggu.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gmyvcyudh.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gtqwbefpu.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gerkyzbzr.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gcudlyysb.sHtML


<!-- 参考信息 -->