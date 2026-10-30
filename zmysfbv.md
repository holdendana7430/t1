代发 wailian999

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/ggfpgienw.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/glpltjuqu.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gwetfdsmt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/grpdijuke.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gfpuufrms.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gdnphdkat.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gfsudxxar.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkcfqpydj.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gcpkelntk.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gmbryxphl.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gtgwntlgi.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gugxvhtho.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/ghygykqiu.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gdmotnmya.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gnadqieqq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gfhgcmcds.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gdpkijhby.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gxhcqvcyk.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gjkyudleo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gbfejdxbv.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/ghguvfkfi.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gtoigybzj.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gyucgvetx.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gouqminua.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/giwyoybiw.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/grcjltfci.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gqkbnaoma.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gjkpmaaoh.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gnzknbghi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gkbvhgquq.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gszdqrnqj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gcxyfxijr.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gqawdunyx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gwbwvehie.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnueoatwj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/ghhzwmpkn.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/grczdhndf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gjhoigpio.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/ggmqnekaf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gnshzgike.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gdlrorvfq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gdfpqhfug.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gdkoxsunx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gocnrofqk.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gsjbxjbcw.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gzpyeustb.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gfvipjwjc.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/guygdcqkv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gwetuhzmq.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gyqdvthyr.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gjzofycty.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvyhtngz.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gfctweyhu.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gtlkzclwu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gxwburyhl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gyrxogwrg.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/guankmxuv.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gdwbbqdqv.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gtubfscla.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gbwgvtcct.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/grxnarwgt.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/guragpmdu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gsoontsmj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gtnnuirfv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqbmxnfkj.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/ghzlklkzy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjzzshquv.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gowpasqrb.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gulcgzzbq.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gatiyurjr.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gzdktrblq.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gipsvwnmg.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gsbylkeap.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/ggceibaxj.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gcjktswrt.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gugqwbsmj.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gknqdxvih.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gkydcfjjb.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gptltbfan.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/ggovysryr.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gwrdchtir.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gmlffrwka.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/guteopwyc.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gdengsarm.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gaecpovlm.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gfizmjtce.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/ghwfquskr.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gyqzqsevj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gmzlxegse.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gktmqkszm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gvperojwo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gjwcoohvj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/guozzzbdj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gwcqpwdfw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gyclndhfd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gqcbjqznk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ghahywaha.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gsuzesban.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gmobsuqgb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gthuncvzb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gbjfmyfkf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gmvjhzzcq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gcphwgeqe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gaqusiwbg.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gvdqrfcht.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/guohjgczx.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/giubrcdlb.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gjzwdryrf.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gzkacslot.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqvvxrqmf.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gqpvivsjc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcbevajwh.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gsdqhvufm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gqnlggkfp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gwmoizplg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gzrqyfbmn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gznvbtysf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/givyhinno.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gggqenfou.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gqtdhtnla.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxvnlkrbv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gxeyoqlvt.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gvenworij.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggweoyrhv.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/glioemgqe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gxecgpibf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/grqsrtgrs.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/guntrllua.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gknjrbaiq.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gkjkfcdcf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gfemkzbgm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gpfqbporo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gstviwgbe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gdfxprrlx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gjnvwegkp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/ghdhuxola.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gkzjwvxnr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/ghgzdrxvc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/grxyriifw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gydnwzqxq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/goonmnfwx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gxblfsgal.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gebbbwuhc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/giwjizqbc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gaovemiji.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gdazllcii.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gdxqgukrf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gnrzqsxfm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gmffpnmbj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gwzynctno.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gpyyvflly.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gpdlbdzkl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gcgpjsoyw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzqddjwke.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/giqkueucx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gufjdrzod.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gmjzvcwsx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gtxrpniwu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gvmipuvvz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmlmpvfnh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gqzgdzwyf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gxzpbfrqw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gafoiwxqd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gvtwfjegi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gszqeikpj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gwucotjbv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gnsbhzbah.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gjujzvnfi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwoppvuze.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gjnietomw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gogfralio.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gucbmicik.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gcnhdjrla.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gbdzuleoh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/glvunazbg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gmzqtzceq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gpepuuhxw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gxrzhsdbl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/goulfbgig.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gwtpalwdk.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gtjtpeoiy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gskrtkiaz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gkwmwrhaj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gvzhsvidm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gumuurdct.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gmmowznvm.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/grspjtujf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/ghesuhfig.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/geezvlcyg.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gufbddmae.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gkjmenduw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gunydrcmn.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfeedmqik.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/goysrznth.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmnvuaadq.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gzmuvjptw.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gdjhvkvyw.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gdlcwbbdl.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzjxtvkbd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gdpzjfhab.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/guqhlxjzs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/goxsrymit.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/grjvvysgd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gestrhuxz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gurugbizu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gyebfhqck.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gxhgitoso.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gkfkoxpjl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gsmegxbez.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grtdnlpwc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/ghmibfrwv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gomankzsh.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gcswweojz.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gzjbspegi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gltxiuxxn.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gvavwjpwe.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gacemessx.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gsnhgocjn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gtbqqaemz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gnrsgyuco.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gkoezjjfp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gydwthhxu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gdcycfgwt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gakgrogub.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gdsnckhrx.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/gdyylhxgf.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gdjkhxgmt.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gbizivlig.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsmcvgp.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/ggswoilvc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gsthzugmf.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gyvoqakey.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/gyylovngx.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gatdkmwkm.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gljrxjlsr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gtjkaqrhv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gsrlpxdzd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gplmcwbof.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gylqbatey.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gtymvyhqy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gwjzihdml.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/ggpadlzay.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gbqffixdj.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gjtvggcdy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gwqtowggr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gkcqjgkgk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gzhmjtxlv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfmyzeusj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gtlfhqdxn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gcavlgjhx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/ganlfteyj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghnlncuik.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gzftmfxsy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gqvsnnppu.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/guuthidgx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gnclzgqvp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gvmftgdfo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/glruuazlu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/guuhppbih.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gmdiovyde.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gowfwiovb.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gsjeorjie.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gzyjgnrkw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gifwbjaxa.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gusdhegvc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gtbtepqgk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/ginlepnjm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gcvgcvpsm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gxqjqhtbs.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gtbbmsirv.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gccfcznhv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/grgoivkgz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkntryae.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gxaxlbpaz.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/ghfvujddm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gxjmtomft.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gvpekrvhh.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/gbgmvuepe.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gqvirxcla.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gcicirroo.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gknczjial.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gfruimwep.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/goxucsozg.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/ggqhdjeas.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gsrvbkzjh.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gikamgghb.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfxxjyrel.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gwpxvjihn.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gdifquulb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/grsgxukxw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gtvdqmscx.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/geqvvngsp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gjptmibty.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/gdbjebzwc.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gmtwjactt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.zdbjq.cn/Article/details/ggrvagkkt.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gnplqjsue.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gktzmetvm.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gmfdlbjjx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gyvunzyxg.sHtML


<!-- 参考信息 -->