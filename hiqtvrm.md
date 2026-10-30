代发 wailian999

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvmsrmun.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gopasjhgp.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/ghatxfxbu.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gkyybplak.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfurxgrpa.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gexujlpqs.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpidercio.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gwphsfuef.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyvpslmy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gfflkobng.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzsmbhaoj.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gushycjer.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrpmtxdp.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvphlogq.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnacdttyd.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqunboji.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/godnvfpvt.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/glnjuacad.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/ghucnheuy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gppyxkdfv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzvwwxnl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgsxhisa.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdvrxsdz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/grobqgama.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwhezlcp.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdlsidcy.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/glmojvzbi.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvstvlfv.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/ghlzgddca.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzhggvfe.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gchimpfta.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoiqdzrf.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gzanxhgpx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfottgomy.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlkovwdx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvvybbvg.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/grvxzvnrg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmdhocrrk.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxqjgqgv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfumicsb.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdehaejzm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnvktgqz.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyhvpzaw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulrmods.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/grxbqxwpq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gqsubdpds.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gncrtewug.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/grskykyjf.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gzagsjojw.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/ghumbxinh.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsimvznhy.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggedkrsvv.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gbsftoyvj.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gitlcjfdk.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbsurnnv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gmkihnydb.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyfzwabr.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytsgbvxh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gggkwglus.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdxbrkdh.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvcnmlca.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gihmwmzcl.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghixyivqi.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrmtxjrv.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjogooyvy.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/glushihak.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gqtgiyfoh.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gygyxjsse.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkccleyzn.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrlkvmqe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glegouktz.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlgbgbzo.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/glwtmnxvq.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/glmuszsnf.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gexictpbe.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcxrlxwq.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/guxizgamx.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhitmotz.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gmrwksosn.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gwupaahka.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gimwhwzqr.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gaknujesb.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajjmlded.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gubpfsbxl.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gvncshtax.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/geunkpnok.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnzaojlx.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gbzouadkm.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbuzrqwa.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/geixnxtnj.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbtszfuk.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/grgucobqj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrgqzqqg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gotacvzfp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhgykvtk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/giicndnva.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gjvofsqgm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpczmhhr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxfqjiim.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gknlifnzd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gyqjhtwgo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gobepyedn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gzvehuadl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbshwpgxn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gglatuxvu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gptuvkima.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gkeaiwsyt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvlnxnud.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsaktfrk.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/ggxhkktow.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gateltzij.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnofyqtpq.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gorushvhb.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gcoakggac.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsomiqdf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gthizikmg.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpnofwfs.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gohdpafrz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqfdiihj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gbbdzzpli.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gftxorenl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/glptalgtn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrawujbm.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gavitqnzv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gklnhldxi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gtcvqpgft.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gvlebufkp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiuezstq.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gdsagkarz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsidrnne.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/goimcwqez.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/guaqxvkwb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gulumeasn.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/guyhqkmjs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gnvbrdfts.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gvxpprpxc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gavrvttok.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkdvdalj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/gdviylvpq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaordpufq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gexylajxy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxgnlccz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gibdjroii.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gowbitzxd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/geiijztjo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gfatuaozg.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gvizzfafs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeuwlouc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ghmyyklbh.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkoxqxcg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyfwcqfd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gvcstslts.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhqrxqds.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsljcscfw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcvkpiass.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznzjxggr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gjfqtxxhk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmcrlsij.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjmiedst.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcpzehzc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchqcybkw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gayidsiqc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grfqihcjk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaiepkvt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gpghnufze.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gljfavuad.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gksmgymdm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gieyshzlm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gaoijzzdf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gzutrhvpz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gcwkbdfyd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gimyeykim.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdrkvapp.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjzaewqxm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuioumyq.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvzjfxekg.sHtML

Py:   print("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/genqpedlp.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmycoqng.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfilsmsdx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkigrcat.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/geposzrrt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/guqzyfowx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gtzosyimu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrrsrtob.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fanxiaobao.xyz/Article/details/glvginlwr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gwssjedgr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyzcsjle.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqfbqffa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gqjtwvzku.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gojqcjoin.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gdjohebfn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gigbdvbgm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gszjibviz.sHtML

[A03] 常量定义
来源：http://wap.fanxiaobao.xyz/Article/details/gyuyhzryz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gwahbhwpw.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glpjglgqm.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geushxgvr.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxwiebje.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gonkirjzk.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwwevhsw.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gujkesfgb.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtihizbpy.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzqwccnu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gzbgavkmz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gdfrbtdqg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gcucvbuwz.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/guvjxvgoo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/gjlrckobq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoeijuss.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fanxiaobao.xyz/Article/details/grlowkfkp.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/gjixkydjn.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gcpkctbvz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnclapcof.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcfufkeu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtoxitwc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcawspbhd.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwbgvrdh.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkakuddcv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfkgvmew.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/geewpgwos.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gopazxapm.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gkleytwmk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gnkvhjuxy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gbansgmcz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gcgjhxnbz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gydsyhchx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gjvacbvxt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fanxiaobao.xyz/Article/details/gbpsgmqwk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gkdigbsfx.sHtML

[A07] 数字转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gozmlbsac.sHtML

Py:   str(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiedyjic.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gntnpaygz.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gakosiowr.sHtML

TS:   String(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmdufguu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcbjcrhd.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpeovyyr.sHtML

Ruby: 42.to_s
来源：http://www.share.fanxiaobao.xyz/Article/details/gdipipnvw.sHtML

C#:   42.ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/gysntjafb.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfmhdbhd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzixblfd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawbixczx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gutbiistp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjbjoypo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/ghxbqmhsg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkbxjqtj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltbnyubs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepctzooh.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtljhdohm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gohcqybco.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpbtivnwe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxumwhush.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpaxrgdg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxfvgkux.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmjzwpvw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejdtyzcf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpgwmrica.sHtML

[A10] 生成随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gltvxemlh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fanxiaobao.xyz/Article/details/gcpmpluhr.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqttucdim.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghueeylcq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnugruetf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvdwtsvl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjqppny.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/gvjfoqxnc.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrujoeed.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/gmyrsbshf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fanxiaobao.xyz/Article/details/grfpmexwh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gjmdokqfj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/ggpetclgu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gmewlzmez.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrjbcljb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gdejfbomy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpsgxdgl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gspipdupg.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghzjntzvt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkjevnru.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fanxiaobao.xyz/Article/details/garjsagkj.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gzrkydwwp.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gfxtaxzwa.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fanxiaobao.xyz/Article/details/gfigiibgf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gfuzrnrgd.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/gwgwrjcbe.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/ghjnlvrua.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmayhnojm.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gqfikozsh.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdozyygzx.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gljrsujeb.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxyeokrx.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxncdbvc.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gpisglgcb.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfbflgzv.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gergarkki.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/garbortvn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaaluarp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gwghysxep.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxenzeua.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxswhzgb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkejgrjq.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiqsihks.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fanxiaobao.xyz/Article/details/gthysdeuc.sHtML


<!-- 参考信息 -->