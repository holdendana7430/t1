代发 wailian999

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gbjkjzisl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/grvpfctvb.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/glnulggwn.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gdlprhhbw.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gpdjzdeot.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/glwwghorc.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkikbflfl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/goimtoxjz.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtssiqsfs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gkfipmiaw.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gejncjpvq.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/geuiywuub.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzniuaiim.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gdcakpsvu.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtngemvnt.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsnjzjnn.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gidmycuro.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gbyvfknkr.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxjalxbl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gsdoyzfnq.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gaifdsmbs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gszchxsyk.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ggasweuph.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gsmrcodlw.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gjirxecvq.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjrybidp.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxekyibmx.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gqrzsqsrz.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gitdaahyj.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxhjrfth.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gikaphcin.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqivyzaj.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gdqvdtegj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gazhpeqlm.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxwykolc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggcagqems.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gueikqseu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gffzxsuxq.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/guovllwpz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpqujvzn.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gjmwbvtfp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwydtpqx.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqxdqteh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuihwoio.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gxqhkrgqi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gnrvejslk.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gguaxnnch.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/geinphxzm.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gyrdxnhht.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gdjznwoki.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gdokkywco.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpccujxqk.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrwlojbh.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxasiard.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/grzdysoos.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynsoqwmt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gclfrgmzc.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gsjtzutst.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gavnxkkud.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtzvzse.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gexcemzgp.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuggwpan.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppvsbzco.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gsvnsjcmq.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmuvyqsh.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoxzhfoy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxbyknin.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gzyocaspw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrbxxcab.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/geqvouwyn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyzpbonst.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpfmmpej.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gaidnoprk.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gccfknnzb.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/ghbvhpzam.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gsfrcsuao.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnpttost.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gknemkarg.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnphmdliy.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/glbutplkl.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/garemorvy.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcrmrwaq.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjegbhea.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnkinenb.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gallrbxus.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gaixmdbge.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszsinoaw.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqiigupw.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvjunzxp.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gvsnubmvz.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjgwgypn.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gjecpnvmw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gihrhaycg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/grtvdghlg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gvatwsozt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gtabeomxu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gweiuwuuw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gjzitfxur.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gmcpyveqx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkwdebrl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrxxkrbe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhcodtro.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genpdpguu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/grngvlnox.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gsanmdhrq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/giheornrf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/goxesyzxj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzevytcr.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gcqmeovyh.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/ggptfcirt.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gplmglpvo.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gajqzdxte.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcodwhwjt.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhtipuji.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvyybeaf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/giirktsep.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gdygwcafz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/girhdpsty.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gajuekabc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gtlbezimy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gqwpabjmp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gosflwxnq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gligalfoe.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/grdoueqaz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcvrklhod.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwozwnjf.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gxazfknnp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzizhvyx.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gxkotozar.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/ggsysutnz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/girbayybx.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/geocgykyu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjstqnna.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbhyjlth.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/guhghjkqy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwpcydwo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gugxqyoco.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gftinanxs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkoyffzk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpipiwzb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/grlbxtlfo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gutbysvgd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/guvwnyhqu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/guzncejps.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqostbg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gdhcuilkw.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gjuididbo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnzswyfn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/girculjmp.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynribcvs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/giscxncdr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guotojakt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmhpxlnt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gffxkcdyg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdzwkjm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gkfhwbabk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuksnooq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzdyhddv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodjrszm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggvwanyzx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gifmymqqn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gscagshcp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlehxmta.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsnhdwmo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzrnbzzz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvfcrdkk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazauidwe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgrbwkdf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gflgeuueb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkagwvng.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/grfcbdgab.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekrkkseg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guoeoxljy.sHtML

A. 基础语法与类型
来源：http://wap.fanxiaobao.xyz/Article/details/gspozihar.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghxednybg.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqywwodhi.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gkkiprjyi.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrdkbikf.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxoiohfc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fanxiaobao.xyz/Article/details/gymmxgysb.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyyohuee.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gwiuthooh.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gafuargus.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gfduvoukj.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdvkqiwz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxavujkp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfldoptqg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscwxweki.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gelqmdino.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gnkkriemb.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpfvtujb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuvpqfwq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiymcroj.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpyiafwk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gzvkhfvcp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrstnonq.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gkmpkewly.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewrbevxh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghldamaff.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/goneltqhy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlwjecvb.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsuounmx.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gyhuivfgd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gdpqgulga.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gaxcudbab.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gpqowyqyz.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gtggqvsww.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/gtmpnlnud.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/gphykmpug.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapikjzwt.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjtopfeh.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjwcistg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gwnfueiyg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gajlkeqho.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhkyzmfa.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvfwzahbv.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gffhoziyv.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrtyqcxe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpcbsuiv.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/giavsdvis.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gxderwmnl.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghedpvrtd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/geuplxpye.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/ghubbwxsh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjgvirno.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gqeeguxqc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gotfohncb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gvoqmxffw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrwtzivt.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmbiqlra.sHtML

Py:   str(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gutjgbzys.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbcwzdvb.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gzibujwyo.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnjmvkvp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwvvfyuh.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmsuhzqn.sHtML

Ruby: 42.to_s
来源：http://baike.fanxiaobao.xyz/Article/details/ggipwgftl.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxusddio.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/gragrpatb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzilxdrd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fanxiaobao.xyz/Article/details/gketcbikx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gmvtihwhk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgezwjsw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gtryexiyf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gjynidlsx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fanxiaobao.xyz/Article/details/ghlhwesol.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjqbfevy.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcedefmn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvkviiyp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrxuvhsg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdcjjwvn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvpwwxhgk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/geonbkcse.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gmrlebdpx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/gnlwjgbaa.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/goakxszby.sHtML

[A10] 生成随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gfzwdxjuo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffurefzg.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzovvyymu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gbfzjytfi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnvvokmq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/ggwczzunc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvstflru.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/gdublwlmx.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfoymlbj.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fanxiaobao.xyz/Article/details/gbetuyiks.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gxopcajtx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyihktxj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gduopzghz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gaogppjlh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnrhygmo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfrxydil.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gruhmurgb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbouyibqp.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwshaskop.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzdnvwws.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziozlbir.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/gzaglsqmy.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwjuwavr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnuanpne.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gpteahggy.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcixttqzv.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/goobmmrkl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgfqxxgk.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geswbkuii.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvacxuczn.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/grkewtqdf.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gydnwddim.sHtML

Java: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gezzvlglu.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzwivkbb.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxblnghcb.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gasxmwggz.sHtML

[A14] 注释写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gygzkfstz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fanxiaobao.xyz/Article/details/gsbbgrdye.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gamftgzrg.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvaknhqn.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmtnpsdz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gqffjfatm.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsanhgki.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsflfihq.sHtML


<!-- 参考信息 -->