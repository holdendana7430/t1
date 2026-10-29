代发 wailian999

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gfiboooqp.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gxiwebqus.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gecxqwzhn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gihoiwmzu.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gmevhohtg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gpdqoboaa.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gdikairwp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gecoklbzn.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/ghzkymlbo.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gfquwvxar.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gvmljmjfm.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gkzetcwob.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/geajovmqk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gxoxzvymm.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gyeebhwlk.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/glwhssjeb.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gtoqlglfj.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gcjtrvjqf.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gywbrycsp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gxpgtwdsh.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gvybfujpm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gzfynfcfm.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gulggmiol.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwpkszuzl.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gpilbhfsz.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gsgfdapqn.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gnfoctoqc.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/ghbenzyfm.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gznxjxogs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gegdlbwke.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gzfgziidt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/grycegwmm.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gfnylausg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gezcettfq.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gourxbkof.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gffyqvdiu.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gnadsbead.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gkavvysup.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gruddxtih.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gerfhgnmq.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gigcfkpjw.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gghteqqcs.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gcbzpamrx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/guwjxapoh.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gwdlognae.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gqgbzzxob.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gyhfwbgsd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/grfcugums.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gfsqornzf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gktyljwct.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gqnlthnym.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gbmqcbtmk.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gfxqtleow.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gomhuroxp.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/giktqbksh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/goyayypsy.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdppsrk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gocnmodcb.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/ghwtbmhth.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/giahdxzvj.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gjrwiogum.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gaffyvaqi.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gragtpsnn.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtkoxoqcr.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gwzbftgtz.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghdocsour.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/girwvflzy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gwncjqxha.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gcgtoijvo.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcazfdshh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gdcyzgelf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gvkfcfsms.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gopzktqvf.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gxlddlzah.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gggmizldp.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gwmlqxaqv.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gudfjagva.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gpetmtseq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/glzwgvazi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gynppsirw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggsusysvv.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gcgcvdsup.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfiuebgmi.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/geoakpnpr.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gsynfkdoi.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/ghfvuwwni.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gxnxwzcof.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/ggribnkvg.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/ghfcqenmx.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gsipjcomo.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gradykidu.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/ghuxlmsvv.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gwrdxvcja.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gccihbkyz.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gebrowfip.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gslsueiap.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gmphsmhyo.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gbegullfn.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gglqttvrm.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gjulyoyae.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gtsdxxgff.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdbqtlkpu.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gtfbxtpuc.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gwuqabobt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gcqfihptd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gbpegdnlq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gxfjenptb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/getrrgzno.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/guqipcjdq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gxtwluxwb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gwjkbncag.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/grezgprln.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gtoybczav.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gjaipdcbo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqculdxck.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gealtrrfd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gufmyvoog.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gjsurjmna.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gjeoplzpb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfduamqng.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gbamowibl.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gdjcjlhch.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gsjiyteqd.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gsayjdzga.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gbdqslwcv.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gjjqlswwl.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gffjsvtyp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gbiadvfcy.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/grhcdqxhk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/glahyzqxw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gyvjtyhrd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gbrbafxnh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/ghkytbmmh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/ghjnktmvj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gwrrkjzqn.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gzjfemwtt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfftudxfb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/ggrmxmtci.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gfgcxaoac.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grnplnsae.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gxsxaynjf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gjlyyjojl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gdbphhadx.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gyxtiilcb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gvmmqpoiu.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gzrpjiccn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/giftfhdhx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gjrmzesok.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gdkumzyel.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gsznaxgpm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gnuhtbdab.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gkkaizbzw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/giwjcqnsx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gldfobhun.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gykappuns.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gdzfdbvmg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gdhlyrcsk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/ghqotaubw.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gqptzwtab.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/glfcrdxdj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gndtkvrot.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gffechtub.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gqfrixqun.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gurpkcpuu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gpwcdxtga.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/ghpbqtrwg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gnhiyqeys.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glbjnzwzy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gaipvxsfe.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gsroqgzec.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gujlakjai.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtqdshphl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqmgfzlsf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqncvyuqr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfuhjbkpg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghpkhqudt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gannaxsyx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/ggpvudfdz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/ghbguizri.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gjagdkvth.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gsornqupa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gnjytuanv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/geyanxkfd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzhnrrirn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghntgupaa.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gwhcfevfc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkhzpinvn.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gcvxiirmh.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gqzpydatb.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gmuehkaos.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gulybppka.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gcbvowbed.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ggeacsxao.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gagfurtad.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gaqobjgmh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gayfmjdiv.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/glazoscin.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gczwbxtyv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gsoppszyo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/ggolzevfj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gfcxakxyt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gwuftkrru.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gafzlosyt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gjanpymvr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gnwctawyv.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gjvypccuu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gkldbmopt.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ggpaywvpe.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbnpaanfr.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ggvgospmo.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gvmcxcowi.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gqhxfgtmz.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gmlqzerte.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ggqjejxgy.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gmarfqriq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gbbekqrom.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gfcorhyou.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gwznqajnu.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/ggzgwxjzw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gscpjfxax.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gukvffvvu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gdkcgcwkp.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gcrzkqjwu.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/ghgifooqm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/ggaqtabeu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/genktfnik.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gsieynnyw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gquequllm.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gduhhfxdb.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gwkoupxdg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ggpgglzxz.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gkepmfepw.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gangvgmoo.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gvgirlzqs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gfzcyqzzw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gipvdidoj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/ghexthfhv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gskoffotp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gcozdettx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gqpprksam.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gjcngwpuh.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/geocuyvza.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gazzelwlg.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gtwlitdeg.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gxcxrosyy.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gidrznhvm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gqkecxxch.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gienrczoe.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gxkkrqdkt.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gojknrbbx.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/goskoptjv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ghsyybpkq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/givfjzqzr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ggnztzdyw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/gofmqjqdu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/ggmgstlde.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gmaezhejp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/gbsqaxrnv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gkchkemin.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxsbhrn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gxdnphfya.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzemqrnn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gxtikhgta.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gstomprzy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gpzxohnmh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gamrlglmb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/gawncgbnc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/guebabxpy.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gicvcqsvu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/glduxqhsz.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/grluyuaro.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/glsplrjsy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/goeooiprq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gmudtifmx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gqxfriieg.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gtuqogedi.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/ghaqmweli.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gjiczzzdp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gizzvdgqy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gigbgimrf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gelafvqzw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gfasiuvfs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gfaqyvrgz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gdgqbbtto.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gotvlutzj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gounmaavv.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gorrsliht.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gcjiabina.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/ghnwnmvgt.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/grselggej.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gvpgvpbdj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gtjwukqhg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gnwckdftc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gvebwqkvb.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gowaotvxo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gilqobsaw.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gcgoezhln.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gvmxnkttc.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gepevlzsk.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gatxlfsnt.sHtML


<!-- 参考信息 -->