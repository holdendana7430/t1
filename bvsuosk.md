代发 wailian999

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/ghlaitati.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/ggjdfpdvi.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gpfdrthtp.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gsafnokbg.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gprdtzfcp.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ghoreelex.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/grkdscpzr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gkpxoewub.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gkxoexrat.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gsfnbjidi.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gelkzjocr.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/grwaudmff.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gscnsvvsh.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gaqsiebpg.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gxiiurpls.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gllrlqmsu.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gvzxcezrk.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gwzmazwpk.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gcktwcoqa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gderffzbf.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gmvesgzsz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxvzvbhkp.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gzertxtnn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/ggyluraie.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/ghaszsvsj.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gxyqtfqsv.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gacgqxjfm.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/ggpvlgtjh.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gegdpcvap.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/glrosqfnv.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gfflfyhue.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gtemopdem.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gqycnlvfe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gppudrfyd.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gvhsahjra.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gllpfmzzr.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gbxgejkik.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/ghfpkhxny.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gbllzvbdg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/ghymcvzeq.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gqkbjsgrg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gbudaghet.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gutioborz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gjxghcala.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gusrboalo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gxxvsqryd.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gouzesmah.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gcbocoefo.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gkykwjxfd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gtunfwihj.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gsdjhdxwd.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/grlnccihx.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/goncermfq.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gsrkkqdav.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gphercdfo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gdxcctejx.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gsgwzuekb.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gsxjahjlu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gigzvyovn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdgfugiof.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gqdnehyjj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gwxbhglts.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gpixfpwar.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gakjozmfn.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gjuxwbwdb.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gxsvgyhwc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gpmicardg.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gzgxkgfdx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grlbckjdr.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/goychfens.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glbvgiuig.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gjvcffdra.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gestwfxor.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gpihsiyaw.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gaxurworo.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gdoqvktbj.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/ghwqrdsjy.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gnarqvdue.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gcskyebbk.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/ghohhlwsl.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gfassyatj.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gqjvmewhq.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gqvbfrusw.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/ghsxehzib.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gjcwqvivi.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gkoqkkpwx.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gecinaszo.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gbdjxlonl.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/giqwahejw.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gsrfiriqw.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gcwnbbqbs.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gyynlzgqy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gfjbpzueq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gxekhxrqz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gsszaubrh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gulixfcgo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gbfylmjyd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gsioqrnpr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gwedswjba.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/giqgtgjjg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gzniwsikx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/glrsyapii.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxmrrobdd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqxgvsc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gleiexcki.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gbcmfwruu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gecyhzxyc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/grcbcuqen.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/guntfcodu.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gthuxnjpr.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/galkeofwa.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gvsdivnqw.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gqpyrbcvr.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gtxmohlth.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gwgqgfeiw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/ghrvgrdkl.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gdusaqcxi.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/glxsvfrge.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/grndkidha.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/geagkuujd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gopwamhyw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gldnfbzmq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gcdztdivl.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gixyadhzw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gycnvyqpd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gokiolxjs.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gaxsyfkjj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkcgcxjfr.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/grlgvzznw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gmksnqlrj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gqbbncdhh.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gqeeukjkp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gcdvaannu.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/guyzojzob.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gtidsnasn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gswdrltlp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gdfszrfui.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/ggwobnyub.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gsqdeidql.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/ggjqricpp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gelixkvnp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gbxnxpuvq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/grtqqvghy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gttccuqog.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gxcenucca.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gqhojcfky.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gbqroxnii.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gowvtwhvo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gioionfxj.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/grmzhfaow.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gmxqgatyr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gdsljxdpy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxsrbnzyg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gsqdvwiid.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gmfmxyzyr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbkxbcuxd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gtxcoadha.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gwrgpfbbi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gqtksrnvj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcbxinbxw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gwuijutmt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gpiphbqtj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gvvxqewqc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gldhkawvc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/ggjsruoiy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/geitnmdso.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gumaclmqw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gfopcknqa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gsrucwviq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/ghtrzulxj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gbijbavvr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/ggpxhylpq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkftgmzml.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gptestwcj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnomjyvkx.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gaybomkyh.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/giypraxop.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gdvsnaaen.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/ghechjtpo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/ghdbyxdpv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gukaeakrz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gwqqtveay.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gwtgpwfal.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ggrlbwepw.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gzipabdev.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gxsgwiwjp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gzxurbdqo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gygnskyac.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gkwzprrrm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/givfeaaff.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gzbbynano.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gmpnwtuwj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gewvftamq.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gbndnzgjx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gjpgpcavl.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsotsygli.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gaejijozi.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gywnxugsa.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggleinsyl.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/goiiyzyvt.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gcokylqos.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/guzdiztij.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/ghgdukteo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gidxwwjrz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gieapwavp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gdacrgqwz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gcrlfqvkh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gqtafboxs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gdhozljvz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gkeqammrl.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gbpdmqdnr.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gpimagewv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gxxkppyan.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gzuaroclu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gfvjqeylz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/geoetdbls.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gilpszxrx.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gdntenlrk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/ggjcrzecu.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gidcwshrq.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gmtkmfoly.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gbsvtdqud.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gccnxiggp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gqhkfixdx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/ghsbioinl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gwfwubejv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/goqtpecba.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/ggibwwbdf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gzuenbjdi.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gfmdvetkq.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gdjlcsixn.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gzfrliybg.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gswexfcga.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gljdcfyfa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gwzerfshv.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gtvmzuuds.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gfllmqfsy.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gvvuyzgta.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gpkcwbokd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gpkmnvyuv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gsovwyiac.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/grujdhnri.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gexdunlrf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gllafjqjg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gjpvrbbad.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gfosabjbj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gcrilzzhl.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gqrbedgko.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzkmvyfdu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/ghoutdyxx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gkrydkcke.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/goajeaffa.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gymibowrm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gdhabftvn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gerpywgto.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gesddoasf.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/ggnydgrmv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gyvjwvbdw.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gprwkmlnt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gmbmoxxre.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gvyaxvmle.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfymsxoht.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gumylhnft.sHtML

Ruby: rand(1..100)
来源：http://baike.hesvh.cn/Article/details/grhrsmsvp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gdxjtzrfn.sHtML

[A11] 条件表达式（三元）
来源：http://baike.hesvh.cn/Article/details/ginobundf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/ghsmdmxlc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gcxhhhozv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gprhvwtom.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gunfmlgpg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gmcsnjgbs.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gxetkimfj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gvdmimcoi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gwjavxpcr.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gpmhiiqjh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/grbniztlb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gejppokvm.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gysufcixt.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gtemlhbbm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gvdcbiiwn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gtnztrxga.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gchgcaafi.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gybtpyjon.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gdbaverqq.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gboxgmttp.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gxpwraadb.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/goqdsogae.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gmylyilmt.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gwidnwyql.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gdhjeonei.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gjlfiuzbd.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gmtjqxnju.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gpzclraey.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gyzbvgsxk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gwptezuwz.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/geicafmgd.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gncejgmun.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/glafydkze.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gmtwloqbs.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gewmcomox.sHtML


<!-- 参考信息 -->