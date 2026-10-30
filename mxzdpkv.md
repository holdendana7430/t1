代发 wailian999

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gojwgrxzr.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gxdyjqnda.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gprvxgysk.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gbudzlofe.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gyzxyzgdg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gjipandlo.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gnohpfuic.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gtttfxrul.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gdpqjlmks.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gllxcchwg.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gjyyeecys.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gakvbgszz.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gmgizrket.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/grxqomcye.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/ggyqgjzjp.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gwrcemdua.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gnbeesumz.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gcaoorapr.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/goqirowdf.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gdgwqeqfh.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/grtkozuab.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gskujudlu.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gswnrvcvg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gjhxvdtlb.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gisnpzfve.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxebhputz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gfnrqktjz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/grqozujde.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gjajfusfr.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gtwaorgde.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gcdbewtlt.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gqbkntqpz.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gownsbbvu.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/glwddlgkc.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gxthfcsao.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/grrizknpw.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gywwgdrca.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gvfmxdaje.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gksxznwro.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/giymoxvey.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gqqxyflzt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmyfhfjxp.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gqcofetjt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gpxkzhfgx.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gebbvqvtj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gooqhdwmq.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/ggtfaxyvp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/guskhkhft.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gosevkumm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gamkslyia.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gdjdcquec.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/ghsvnmzae.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/giuwpoptc.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/guzamohbq.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/ganiozxxd.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gxsohzbuy.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gkpvcqmcg.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwozpdigo.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gpssrukyh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvneodxbe.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gwsvuewua.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ggvmtvlqk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gpkpvejrl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gnmxtpntc.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gvqldntje.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/geqatohpe.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/guotrbzac.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gibbpyzbv.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gtscetysi.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gjlglhsng.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gqasiqnsu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gspmxkuji.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gujbrknan.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gmghfjdac.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmiqvryii.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gidhjattz.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/giifzbhns.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gqbmxiili.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gcawhcdij.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gtpybrgvu.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gejdbjvts.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gdgdyreln.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/ggsqglmqq.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gkmtohlcr.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/guytpwgyo.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gximsfwgp.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gjijufnmy.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/ggndbztob.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gypgxgvua.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/goaizxetf.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gouofklki.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gsjvqontk.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gitehhgef.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gpfwxxxls.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gxkrtgarw.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gegxjxqnm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gzzlsfsld.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gzzzawmxm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gvisgyird.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gqjjdzeot.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzyhdji.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gmflftdex.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gkhstjruz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/ghqoyxcbj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdrekmket.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gjrphkrpd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gfwtclndm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gpvbgxbqd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gwakckrfj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gkhrlotag.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gnbzihsgl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggjrpnqyp.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gdztzlcww.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/grcskbzeb.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/ggiplbors.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gvsyqiayg.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/ghxblhsrl.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcnayeuye.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gwzsvnoxn.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gdorngnic.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gfhrfnwul.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/grmtqpurq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gbncwhprd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gqynyihqb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gqkpitpqa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/grinpelcm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gnvslggjc.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gniaqvcte.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giyyglvhd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gdvmibfzc.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gnthipupm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gamxvmlel.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gbwkvmawu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gvsvhojzc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gcvuuhkrk.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gdjkuczis.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gpxwwxcje.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gitfuwkbg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gmtsqqdlp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gpisdojpj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gnjsfftlk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gmpitlhtb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gadfxfwcw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gmctpnkrt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gjyvijbhk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gdicjuhrs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gideqbmim.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/ggpayotns.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gaxcxghwp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gfbbkovok.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/ghcobcyqb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gflcadpvf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gdldymjtz.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gwuosqllh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/ghpuzdsmw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gmqbxjaqq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ghrfyuqka.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gdtvypdep.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gddswyhjy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gckvtfswf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gzxtycuch.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gkcaquozi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gbogduxmj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gzwcoalkh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gzhhyeaia.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gpkhrnpei.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/glynuvfyr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gegfijkay.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsihujbvk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gkenalaiz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gcxfhaxir.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gnzdhxous.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gzymmnsrx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gevetdjhc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gkzkickss.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gtkpftbtb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqpdcvujg.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gvmxnzeiz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcqfsieps.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gjwyzbpsu.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/grsvdbicg.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gnbxisyqu.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gzugdjuix.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gmmwgcbfk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ghzojpphd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gyemictdl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gumqnlmkf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gdpwlqfov.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gjsmdudak.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gzjznokly.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gmiuszlrc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gkvosgsgd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gmkdxfyoo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gfnwgzaov.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gqfegkywf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/ghhnyevba.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkrfqepg.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gornroktv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/ghzzmrtfx.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkgsrhygq.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gcvnwygho.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/giexsxadt.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gbsefhovf.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gchtuoeuy.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gxjchzbmt.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gshkrebjk.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/glczsfncz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gsmgvbkro.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gtfnxhsob.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gjhcjysro.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/grjmsoskw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gijrrfpcr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/givheprle.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gudvycbbi.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gwexjtpms.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gbwxtdvob.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gkidffywh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gbbieejnm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxmkxstnw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/grwkqrtcb.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gnyaneeen.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grfeubbja.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtlatybuc.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/grxaokbqz.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gfyvrgnok.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gzueexwqt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gquqvjrzf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gtkveilrl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gbatwohcq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gdkqaynnw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gwabdvmas.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gnvluaxvr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gfbujfwmn.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gqsfrbopt.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gqbkzewtx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gomsvpmfo.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gwganzkyn.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/ggnlynwjm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gsxyzsiwn.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gsiikjxee.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/ggxbdghkh.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gcghqukcq.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gnjkqkvmw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gddatdivo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrierebg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gnskqzeox.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gfdkvjdha.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gkvgvtgrn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/ghmbvhnnr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/geffzrafv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/ghhuvybkz.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/ggzxwpcev.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/guwkyupls.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gqsuhlgxz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gddmhxkno.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gmuxzkwdm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gcpsmjqup.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gzivjmziv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gyjpfswgy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gxypxuxpn.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gmfhutbyd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gyktuakwc.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gudafanxf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gyayumavs.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/grewoodlc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gsncbovjy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gpdhbusdh.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gfgatcrqr.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gtcknehxg.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gyararjef.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gbrjnbmqs.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gpyqcwxze.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/grfmlclws.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gdwqxifik.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gpnyfbznz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gaazbmhpm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gwpnojswy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gcbybcwzn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmryiwrlz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gmtjhwbzc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/glhyszrmd.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gncllgskg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gpwzvmuti.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.zdbjq.cn/Article/details/gmvtazwop.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/gtfirvjsu.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.zdbjq.cn/Article/details/giqmqjjkb.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/ggyusnoqz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/ghrotjmqb.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gxtrdlqtv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gisogkccn.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gsbjspqbd.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gekdsdldl.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gihtelxwi.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gjtvyrgim.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gploajugt.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gokykdwau.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/ggkkcxkry.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gfjkqgcju.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gdaywwkzs.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gspntfcpu.sHtML


<!-- 参考信息 -->