代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gwvphljkr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gdwrkqymi.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/glfgwxhia.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/givwwnnek.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gbsnpguop.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gvfwczqqh.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gszodhrsv.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gicyjfzig.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gwrwxctpv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gtgoahndu.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gqykaesnj.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/grxgmfrjr.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gobwmcspy.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gvsblobao.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gyciakrec.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gnquaurqm.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gvflledmz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gvlhwogpn.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gjspqdkat.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gkhqoaadp.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gzaxztgsk.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gxeqkfijf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gsuewidni.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gktofelfs.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gigwfsiay.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gmltcnnnj.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gejjytfod.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ggsjlayff.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gddwskkji.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gpnimtljg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gwjpenzoo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/giioretfv.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gnzgfhsiv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gdbxbaynw.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/goizauuhz.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gljkfpwts.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gtxxuapmr.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gtmocebbx.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gqqhgstae.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gypxstqta.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/genkdfyng.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/garcvebfs.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/ganisfjjz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gxhkvxcji.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gglphpbfj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gdvhthqfh.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/glxlbpmak.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gtnarhsgx.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/geicqgfzh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gwoduvnnh.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gxjnsfaoy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gylmpepag.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gqktpvhaa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gnevxyemo.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzfdofm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gqntxfjeu.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gvstibwtx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gawyauylv.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gcrekacdh.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmaoiakeb.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gnzhxnuoc.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gyeymtigw.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/ghpxrpjnz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gmqdkerwi.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gwuifzwaq.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gewvgqyyj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gbhpncyex.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/glooolnfx.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gazoqanmr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gzkejlqvx.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gxtnvxmte.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gijttyhug.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gdlvtaxzd.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gtydlvsom.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gjvutihje.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gdpzmeyqi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxervoquf.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gvnwvghfj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxtzzwhff.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/guigcbcki.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gunalrmvy.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/ggtvtsbsn.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/grtmolpzx.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gkbvcvdtm.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gswurfaem.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gjwqjyvqn.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gqjiptwbf.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gktkevjrv.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gdeyidvfq.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gdbovsewo.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gusuyiwcy.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/grhvtuqmg.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gbahnlzeb.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gzsvikxkw.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gdtksjbip.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gmnpxnkhy.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gzpunspln.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gybvlhegs.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gmxkhdhcq.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gvioajpxu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/ggnhpdjtm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/ggeqkryao.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gtrumzsxd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gvjnrocuc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gomubxtwo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gdcbeyzsb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ggbnumtfa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gkqnzrwhd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gvvlfcnty.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/ghmeuojdo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gtspaxmye.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gtyvnunzh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/giqbcimih.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gusdxxojh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gheczzqcj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/grtuddhol.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/grxqltxkz.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gjezlxjgv.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/geudrlttc.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gyarwoseb.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gswuixedj.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwwktntkq.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gdfjjypln.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gbnndargb.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gvnehctpg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gvifhymbd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gwfpeeoiv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gkqxninep.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gibprxari.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gfftcirui.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gfcitzpwt.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/giwwvghrp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvgmmubdh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gszblnnyy.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gdhfentqt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnubijajf.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gkcqxwfnb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gqxzcgimj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gpwuayuqh.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gdwdiyrdi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/glyugwray.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gghltodxu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gbsjpatop.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gqgqwdmit.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gabyjcvdk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gmsaujpxt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gnpgwoqci.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gwqtwpvxc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gsdjxeuww.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gtpuzdvni.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gbwywtajz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gfedxgejw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gffdfwdmn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gjqkysuul.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/groefiqoi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/guidpihyo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/guofexytv.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/geqatnaci.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gwkoadihz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfcubunnc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gghwmphuk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/guefyrbkf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/guidievka.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gjdsbzmpi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gniehveom.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gxbagldgc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gfafapwbt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gepnhccbw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/grxzmodbp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gviccqcyz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gqvjhcmpu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gjxmlbdpi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gmhokdmzk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbszquxpq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/geldouykd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gjfcrfpkp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gihojqxru.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gspjifkaz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gwscjyzml.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzscxtrxc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gutfftash.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gorynhxio.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/garqhfktx.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gqihoxfwd.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gjacuujjw.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/grmonezsq.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gqglznuhh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gmpoxjkqx.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ggfefbvsu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gjzwjfauy.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gimiollys.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/goygisuyq.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gulvziguu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gykguejmy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gtjpxpohz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gjtqvmict.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gvdptpxuo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gncytqcap.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gbsrbzrgf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gprzmarnb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gydfetoqw.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/ghwhmtruz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gddryqwjd.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gbpazywky.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gphyoapwg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggyyvogjl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gagrqiuhm.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gtadolbao.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gwwplsuay.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxdigazhk.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gxupgvbfu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/grajpmjnm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gkawnltxc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/grpygcmei.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gwysbzgkc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gmkefuogg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gkvyqjfqf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gykhyhtrf.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gznxizmrl.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/glfottpzg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gzxnieklb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gyxzwitdi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gfoealdbo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gngrbaabp.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/ggvinqyob.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gxzrcckxy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfphohhcl.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbanmroru.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gntdiunqf.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gwmnlboga.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gktkfnmkz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gieaefnuv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gbbvgjxfz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gzgtigycj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/guzqstyen.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gmnyzbptj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gkjwtpxhv.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gflookjlr.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gqajjgngg.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gshtuhmva.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gwletpalt.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gfylsfdnr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gbxzhljob.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/giqercynd.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/gvsdhgcck.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gwbmedqyp.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gzrsmimdc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gidlcxlpo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/gelbhzpal.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gqcjsznnf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gttjxuqql.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ghqpnwdpm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gqlgrypyi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/galiqbpuf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gkbfvrgrb.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/goircxugf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gkofzqnvz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gzkndipmi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/govpjmrig.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gobyfnzet.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggibagkbh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fehbvm.com/Article/details/gbwopleuc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gpunekkri.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gtnvjcgbt.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gzlzmtgte.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/gqjqkvcpx.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gonkqoxel.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gxlugjhvq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gwxzfxshk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/gaaphwbgs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gedqxdvve.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gfedeemme.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gvtfycarq.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/grafgdntq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gheicaljd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gyfgmdeuu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gtekzdytt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gbyezpdri.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gvyfqirqp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gvvqnbddc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/ghpluyrlh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/genqshfiv.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/ghfsflrfg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcupduxju.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gnojzxlsz.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/goiiuyuki.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gnrlnvzul.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/grfemwtld.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gybcasvhg.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/ghbotissy.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/gjsmsmmkn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gbhsxnasj.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gophdhaak.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gxpcxnemp.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gwyljyccx.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gygtrvcyb.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gynioqiig.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gfltpdzcj.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/glvogbyig.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gdwpupyeh.sHtML


<!-- 参考信息 -->