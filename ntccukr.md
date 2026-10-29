代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gmkkvrkpo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/glfqgyzzh.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gyvxstlkm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gbgtnrjcg.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gpgsmbghl.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gmpgclfsc.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gqbinvmdw.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gnvnyojcg.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/glcsiiago.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gsedaoblj.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gajascjre.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gpineridg.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gsvxbnnpu.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gremgyrqz.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gteudoysq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gctzanged.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/ggisdpocb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gyzjpekdc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gwldwsqbv.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/goljidvhi.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gipsvbglc.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/grrxqjqtg.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gkuomdsrb.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gnuqlaooz.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gaykqlyxt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gvlfikxrt.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gmabffwce.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/giehsbebs.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gnpiujijs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gghtkcvwz.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gxmcbgtqp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gzklmcrzx.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gdqrzigdc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gausyrxpx.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gwfbvoamh.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gtlmonrgk.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gqmtzpoyf.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gatxvgnjq.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/goanehdto.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gzqudngic.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gtpugujex.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gogpttiih.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gybtmzzql.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gcaqcxazu.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/grqtusohm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gzgrlyeuy.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gnajuacmp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/ggwcjwpom.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gqdbzabvu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gryoaiidw.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gjjoolhdl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gayljjkme.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gupoaneza.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/govgdexec.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gvmzwmroj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gvntvdfvx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/glkjdqroc.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gellytolr.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gdgkblppt.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gknqiispq.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/glglcbity.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwtveemer.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gfgjfsgix.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gbrqxwwxj.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gztnoxrlj.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gbkwxngjy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/grtqtxbhm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/glpygfzfe.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gulncechf.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gtacjxzgy.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/ghyspkhop.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/ghfhzffqj.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gedoljkhe.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/grmwhkdzb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gpfyperhc.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gyvqcfnlu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvebphydg.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gppbzuekq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkyhnotad.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gmzcrowzv.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gnnxoufiv.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gkocmwvdj.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gvrlzzvej.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/guwslfzud.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gwujfxusl.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/ghqfhjfec.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gzcxinqdr.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/guadxvojf.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gcuayjkha.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gsftytheb.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/ggmihrtmf.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gzayyjxmp.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gbdxhejca.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gxgpgedpz.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gmghoqamb.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gnzgcvkpe.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gctkzhkep.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gxykibfxw.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/giltfubex.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/glksdytuc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gswmlzgnc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gikcrpazr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/guehnkrbd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gbfrcmgto.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/geljnubtm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gsgwmwmxm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gwotmhull.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gzwrrgjks.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gplpboist.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gvlnexgjo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ggxutanlh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ggqwzrheh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdymkljyt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/grflcjuar.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gwstqakfz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gnpdnysfo.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gfjtmjbgm.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gfxnecefp.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gfxujtssu.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gtdtbsspf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gqnhpeepc.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdvmxieyl.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gebddfnzw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gfwavtgra.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gfzzppvtc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gjdgqmtoo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gcolbqusv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gzyokagtg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gxnefdnty.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/ghhfgcpqj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/ghvcxdphb.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gsmyqgpqy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnhqkacuw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gdwcxmtka.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gsbbvmarq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkidrrdzu.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/grsetotca.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gcreexmxq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gmqdilvlr.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/grrxyutaf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gkwnynirq.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gcwzfwdxl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gwgzwcssu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gtlvgzxem.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gjwbhuvli.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/goqiedfhe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gagtdcdcv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gpmbzvmso.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gmkszddnf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gftreetyu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gngoqoyir.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gtbrzokxy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gruqqjcae.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gkzaibngv.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/grypigzax.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gpshtspzj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gwwtaxgnw.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gmxifuqen.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gaeushsfs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/ghpisklli.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gykzootid.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/guruzynuk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/glelmstac.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/galmnjxmz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/goupvdyop.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/ghjjzzdcl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdltetswy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gnsvybkej.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gfosqmlzi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gljwtaujb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/grhyyyphb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gmmzysqnc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gsmingfuw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gvdtstblc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gzsxbyred.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gckoancvq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gyqezpcji.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gvdsuqzuj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/guhqfbkql.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gnnylzarq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gucnepziu.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gwkpnirtt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdcaqtptz.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvysomi.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gdmamwykk.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/giuptktjz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gyzwloujs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gfvbfcfow.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gxzdtrtbm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gknpehqsj.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gsjuzajxw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gtxwilzuc.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gjyiniriw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gubjqirkj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/ggumvkyej.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/grwkdzhpd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gjzvksykf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/ggtaxuuvd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gcanaibrk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gdvhsjbsn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gzlbffwdy.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gpctzoezy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/godbqrxoo.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxwkyblfw.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gaimhasbl.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gqxsethbo.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghpnjygdh.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gxawulczd.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/grxyyvduv.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gumndyefn.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gcyqbmdii.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/giegdyyvr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/geezgjnnf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gsrfbpgks.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gkrkbixwf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gbqjgowbi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjrsmzj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/grywvtspz.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gckbhglsl.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gwwnjexjc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gqzihamri.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/ghwtkwqpl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gdyezckdv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gffyxgjpk.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/grsqyxlnv.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gazdqcqva.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gspnndgmm.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/goycjghff.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gphlfrtfh.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gqcsvfiiu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gaqgoauwd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/glagzamnz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/grlzvboqh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gbqefxwfz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gyejxcpzy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gzctqpjbw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gzmmorfrs.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gjmlloydo.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/glhdmtulj.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/ghjtvugio.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gxmrptsvs.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/gxydimcxl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gqkdlneoh.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gtqsxdrde.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gvmjokihn.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gjjznbzry.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gtccrnvqh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gnilysjru.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gsncqrbox.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gmmtkgvdf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gkgalfrlt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gewnlguok.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrdzdjqi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gkagehsgk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gotoylaud.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/grstbolaq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqzopgxhr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/ggchlbodc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gsojnphuh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gxzmnvvke.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gbmcrgafs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gelfqfgsz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/goupyeznv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gusfuuujf.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/ghaijhduy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/ggpyqonkd.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gfudjhpax.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gikqditmc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/ghfvzntoa.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gynnquezi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fehbvm.com/Article/details/gftkikmlk.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/gyguvlcda.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gygnohdhq.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/gbqlzlunj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gtaazacpz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gcwootmna.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ggjsylgdv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gywejknrz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gfvpbgvxn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/guwrcezps.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gcaewwoxa.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gaeklygvj.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gvoryjcfy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gbhhuzvtg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gtqxbjupo.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gkaocfkvs.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gtziizoto.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gaanqdobw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gecqoiuxr.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gvpzgqoru.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/ggafzubqk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gknboaklk.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gxkvgsoam.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gxjebllvw.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/ggfzvrunn.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gzfiadhja.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gqeommioe.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/ggqcothtk.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gpvvodvte.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/grivbwaoa.sHtML


<!-- 参考信息 -->