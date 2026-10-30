代发 wailian999

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gwtftpfsi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/geilvpyyt.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gausgoemb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmugbtmm.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gxvkuhrrm.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqfvrcla.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvjajrsx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gyvsbqmub.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhujaxsc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyfcqngz.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gakpvakzj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwaybbzq.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gsselunyt.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxqwdbul.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacduetlh.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiddhfcy.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gpuqqmpmm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxfvscni.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gszxyqzuh.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyepkcos.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvywqsd.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gpdcjxlrd.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbimyyugq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxxdpest.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/glhzkfuju.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzpnjagg.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gygyzytvj.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gjitxdbco.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gntwhvcvv.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyenmpqs.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbheatynh.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxbnesxx.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwrzeqmi.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsbtqkzn.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbrgpsqs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gcttkahjy.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkcouwxb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gksfkxbmi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydbqegen.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gcozguiak.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxxrcvfd.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gienzumqt.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrytlrci.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnwaiyfz.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/giumhceko.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmmlhoxb.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcplavdw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikyuajtm.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqzbnsys.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnhgbgqw.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszkprlye.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbqwxvty.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gkupbmljv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxpafqir.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gufqnvblg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrdrxwhb.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgemnwue.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesxghjxh.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/goncpsqii.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwbjxrgt.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gjraweacb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gahsiipvb.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gaawgyqyr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjsqdlyr.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gpntkhplm.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gpqgzjzsl.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxhdfuon.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayjdfxek.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/grehpdylc.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/galncarco.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godviqhik.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzlsplpd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqssucwe.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gwwvuxgsu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gtuclqtca.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbinqsdf.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaxsnayz.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/guquekmnb.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gnolfmfmw.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzuejuiz.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gjdsvpqaj.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvizpvvx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gwlfqgyvo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpzwzyvz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gehisdthc.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gukehblht.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjllnvocf.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/ghhlwzcba.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcjxdufh.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtriqnwo.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gcffuobuj.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcydfciee.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gbvbuyasw.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygezporz.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gudzxzyvr.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gpomulymm.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmktvzyu.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/genftmhrz.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmxtqjmg.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjsxgnkq.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/giaxopoee.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gceszbtqh.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/genyihajq.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnyxohnr.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbfaypsj.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ggdlhdxmd.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gcuofhvmf.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gefcbdoci.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gzdcskclt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/guyclapht.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwwxvpbq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gztbhbslc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gdnbagoun.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhyrufdk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gozusucwu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxjetvnc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ggolfzpgd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmnogyrm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gkojbkqso.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnlbwdkb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/giysozfcl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gcdgzkxjn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsmewafc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gcuudieml.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/glipyvasq.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdtnbczq.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gltwcesbc.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsyvhnlp.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucxguona.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtympldge.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/ggesquiei.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyuuouze.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnotktbk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gyxhpquct.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxaxjypu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gpvcdliwl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/goobduirh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gorvdohwq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghadrcdyr.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqugveqn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gswrtvumr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gaeahhksk.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvpizuth.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkjhkrnr.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtktjujk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gxipwpwsv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/ghhneeamy.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gstlstmkp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gscvcqvpc.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqaadrgu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gfyjxsvfq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/ggucvzpld.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gblinpvnh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geddedyos.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/gpghzvdtn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gddejgmtv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gofuwpooy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrahlwec.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadloqacp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycfgzkie.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkkdhmpu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmrcdmfh.sHtML

【文件统计】
来源：http://baike.fanxiaobao.xyz/Article/details/gklcbjuab.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/guctwagez.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmlajgwk.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goanxitfz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/ghdyvxudx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbgoagqr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbpalkwsz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gsfhwftai.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gotyxcomg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gempjosli.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaobmmmro.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsqgqfku.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxjklbzv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnuxqylkp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwkxsktbr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/glxvoplpe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbxjpgah.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwyrjikq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluftrazm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnivuhjmi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gaiavuobc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjzhlyye.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpgnymcle.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynlvqjey.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gpbixwhep.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvrhjpnf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjitjbfh.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/gkmhtmpvi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gweaotazi.sHtML

[A01] Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsclghpbp.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkludpuj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/glomvktoe.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gqbnpqnyi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/glckdlnyt.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyrbzikg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gxpjjjavy.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtszwingk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gqqnvalpt.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmmyajfy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/gsbtyblxv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/ggqxgpuls.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gaaztfvbm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlbjruah.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/glbocwccx.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gfisczoko.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gikzeqqsr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqugujihz.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbtulvfg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/gkqjchljl.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtapraods.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/giodmbhzv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqdvapmx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzxceaje.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghezjolhq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwgizyll.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ggdxympet.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gctwqnbcl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/giqtsrwai.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkarmzndk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gozainmay.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gycwnkfvp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gychaqegt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/gxcfuedrv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fanxiaobao.xyz/Article/details/gwkdnjvbx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeernazf.sHtML

[A05] 整数除法与取模
来源：http://read.share.fanxiaobao.xyz/Article/details/guwlsoqhi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gypqqxhcb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgjxdlvg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gandvfmcx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcnshqpv.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnxtpipjb.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkcpiajy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwvqfftt.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gyjcmzkrh.sHtML

[A06] 字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqssxtbh.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuungycf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gbetfrgqb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpipymzsx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gmxjzanns.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfukzamk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gsrtxrhpy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fanxiaobao.xyz/Article/details/gndpbmdug.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgoucvsb.sHtML

[A07] 数字转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvqcghxd.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/giwzulonu.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gdklkicaj.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxzqflzq.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaydirgp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gcszgpyni.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gajkmvmlj.sHtML

Ruby: 42.to_s
来源：http://mobile.fanxiaobao.xyz/Article/details/gckphwjux.sHtML

C#:   42.ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbjobzld.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqziktte.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/ghnfbfksr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fanxiaobao.xyz/Article/details/gnfkfukoz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynjhxejd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fanxiaobao.xyz/Article/details/gnwsmpfhe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxoqmhes.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gufvicrug.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fanxiaobao.xyz/Article/details/gjgfpesgx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzlmezer.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtazaqquf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzykgpixx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gliqoxbit.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/getbrkwuo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guperhqia.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwbqzmen.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fanxiaobao.xyz/Article/details/gljqrinmh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/gpibkegqx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gosishvxh.sHtML

[A10] 生成随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/guowveosp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvknzcsvn.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fanxiaobao.xyz/Article/details/gyqeohmvw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/gytrdxwgh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gaeqywiqp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxmwkiai.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjpljqtg.sHtML

Ruby: rand(1..100)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqlpphsj.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fanxiaobao.xyz/Article/details/ghjitbvlh.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqeeiiay.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpdeqpoe.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gphipmtkq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gdlbyidwl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclwjvibb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gqwtojaot.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fanxiaobao.xyz/Article/details/gxlqsnjjz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gamkxqdpr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/glwsxtmfl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpxoxgbp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbamksfxb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gswodgfrb.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghukumbzd.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdxwnady.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgnppltk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnoyfgjq.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/grekbnnln.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoeqthii.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsryigsv.sHtML


<!-- 参考信息 -->