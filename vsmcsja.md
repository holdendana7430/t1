代发 wailian999

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gmrrokqai.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gcayimuna.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gcuyoqzvk.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/glbagumzt.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gzrcojmsz.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gdgtsvtii.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gkajnqflj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gjwvabzom.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/goyoxfvpy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gzgylfmsa.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gnteqfzfg.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gcymoeeea.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gtnqhwxqo.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gxkrmgzeo.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/geusntobf.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gimbotfxm.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gzgdrnoox.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gcrbevfpu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/glwiagcbh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gfxnkiqwx.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/ggampmaqg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gpefbagkm.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/grwqwmqyg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/glcuqxpqd.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gzgiwutqq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gpeqaplsq.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gcqtteslf.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gqtvfqlbq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gsaaytqgl.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gkslugmfy.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gpsfxhkwb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gewaelkkg.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gdhbosrte.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gxfzhdkyk.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gxdxgmgwi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gglxupypk.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gnecatlop.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gmwbbnxsg.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gpbyzennh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gyqsivepv.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gygwgnljt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gaqlyjpht.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gwbiqozgl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gcuknanxr.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gfimplbvc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gpeqsihia.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gggwgasqy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gbetdmyqz.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gswutshpz.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gwinpdouz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/ginhbyqtz.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwdvwbfpz.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/glgyrpnju.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gtmqljcwt.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gtwydwwiz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gvjpbdmxy.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gtcnsuylr.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gvepzeqsy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gbsbhjasp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gomketkpt.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/ghkvntbco.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gqojqlelv.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gpbqblbly.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gstwtjgtw.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gwalgeinz.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gsbhpenvx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gpjqpwqna.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gyitdevvt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvbzdpeht.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/ghvjcosfc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwhjjwpds.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gzqsvseho.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gzelebhuq.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gwowkejiq.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gxjbbqmpl.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gqnxcovwi.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/ggztvolsl.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gkpzxrfie.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gjqylqwpy.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gdecwgcjh.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/ggkdydkvu.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gqfvwwwal.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gmshwswbk.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gvoranwdh.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/glzmosyrl.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/glkwzpsdl.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gkqkzgkdv.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/ggnypemrb.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gtuhmnrmm.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gedzntdzr.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gmjnmjjps.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gjtpzmgsl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gzoujixxd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gmcxjkfio.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gnseyyrfa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gntzvfblq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gehzhzrpj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gtijqjqfy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gdcbqeihi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gsnykfcwg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gcuiglzry.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ggglxaedk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ganzkdfdc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdicsaypw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gwevxbkqw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gcfgtectx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gmbrjaooa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/guthijxbj.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gkjbgqsxl.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gymgtvxve.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gojvncaxk.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gylfwnvib.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gnddckgai.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/glzhjbgfe.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gwkbidmlz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gxpmsvqoq.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gxjfwnbih.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gwalvhmqg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gohgrmpmv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/guyamulci.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gmawmrrwx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gtsbovpic.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/grzxmqrpz.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gvysvfeeb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqmwlnngn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/ggborinyf.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gfsaoovmy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkfnpsdss.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gklvramqy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gsqtaegiu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gtasarkzl.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gqqstsnbz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gvvaxjvvl.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gihttdmxg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gujzjupev.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gkvcgskvq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gqocvgcfs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gamzmoyor.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gcbdvkrkj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gsjokdmnv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gsbpkwmtk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gbfdkivvq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gowfxbhjg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gmxopxxue.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/guxeiwyqc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gtirzihoc.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gbryppvdq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gpdtylmzm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gfprdhprr.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gqiyuyeag.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/glfcnmqrp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gvqhhupjs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gtrafmddz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gpjrlzouo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/glqazgkad.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gupvnulzs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gfozphirl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gaaeajcqd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gdkxjrkev.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gdveevcdc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gdqhpljyk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/ggqogbiwt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmqdhtlmt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/goczbaksa.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gbkvhxuhg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gohgemsbe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gchtttxni.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gavgjcvoz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gcnnevcos.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gaynkfddc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gsxeckhvb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/grcvnbkep.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsxbbshjm.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/ggyyrpkqb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxzeelctr.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gbcnzexgg.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/ganaeksoq.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gncnxumfg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gbbpdekjf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gqfoxkcnu.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gruqahemv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gwffxvlqr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gblpgkfve.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gilhefhlk.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gosapxnqv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/glhnrxlzn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gvrjimhhe.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gkbpfpyvw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gcraapqgp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gnrdzptmh.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gwzrvszdd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gzxfprtqg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gychvtcmm.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gngntsemk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gsqmfoedd.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gcjigfzwb.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gabrilpcy.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gtajkdvht.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/glpyjiuvl.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gaabcchcu.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gcbzrnphd.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gympkxtiz.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gmltmxrsn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gulxmhbia.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/ghqfzxnst.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gdjerjqbi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gdmujwpwc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gaxztnhzi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/grjgwctty.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gcnstlsxn.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gpmxzakyg.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gozhlxtcj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gqcbhxsbk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gtjzcsaxe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gxqluqhdk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/geijygmbx.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gmyuxhrzw.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gcrggdzpa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gsrbmiinb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gapyzbbxd.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gkhccrmxj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gqytsotzy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gttyzkmup.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnkpdoy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/ggysysana.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gjvuugbft.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gaiirvbpv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gtoiqlaug.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gvpdomgqa.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gwzxiwisg.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/grrntkoia.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gaxijbimk.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcdfggqfi.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gpbloghsq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gezdeosyd.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/ggtyriglo.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/ggpwvddwb.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gxffyntam.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gszwlnqcz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gcdbxriig.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gnwwdtmer.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/ghqforgfh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/grtknbthk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gnvroqurd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gsoaztcga.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gbofzhyxr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gposmlyoa.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gffhgygjj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggkjcwvzr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gomefkcxd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ghessjvll.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwiilznfs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjudzelvi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gjvlogecl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gewugapip.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvwumsmal.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gpyvtpvzt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gxyzlevlu.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/ggqrcylna.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gfjfmdsnt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gmdvupgib.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/giljcbirw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gocygkozf.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/geldtgtny.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gddylcvvk.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gxcpzhmys.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/gcthckhzq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gcwletfll.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gwuqwojaq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/godkutztq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gygychaas.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gkkdvvemp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gooscueys.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gpokwhowy.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gpqynjngf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gkhkxdqjs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/ggzseofau.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gapjsubbe.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gefugwddn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.hesvh.cn/Article/details/gbuxsgolg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/ghexrxkre.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gkiqmtqwx.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gcavknznw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gvrxfabhd.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ghoopurea.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gstmkcybj.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ghqbsytqc.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gmbqjysec.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/glzuwnqvz.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gfnpkiaql.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gcrvbxnof.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gnigibxeq.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gukkbdxbe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/gdhofadxu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gbmzgnhyx.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/grrvsqzsn.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gmnvberrl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gykbjrehw.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gmaoxaryf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gggadtfhr.sHtML


<!-- 参考信息 -->