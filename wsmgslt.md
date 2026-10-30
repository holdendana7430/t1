代发 wailian999

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ghrmkkboz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gkxbyebqr.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gthjpqwyt.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gmhxzugfo.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/ghnfyuroc.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gamgxpisj.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gupduchsb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gjhrfkztp.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/guxgezsdq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gsubsqpxq.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gufltokyy.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzktuzrnq.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gynqiqaid.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gpweeneem.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gioxxkdzc.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/grlhfpnif.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gqdrgkjlu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gerjlobyy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gllrknlig.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/grmwrdpbq.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gluwvcone.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gsproesgf.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gdzohijzd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/grhverffs.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gfupmpfqg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gbdgjruvp.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gxxbbmxpx.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gczdryovm.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gtmbewgac.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gpzvzirql.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gvmqttxzc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gamrijmww.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gibqhswom.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/grpvdphfg.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/glcjcgxgh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gfuuaxybg.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gljluxcwj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/givxolres.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gtytwrpyz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gmkaokbas.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gsjucymfs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gnwasveyq.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gziwjfmjs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gryzvevkg.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gnbnvcmvd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/ghrscuwqu.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gllyeglqd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gfkoyleau.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gdkzliaib.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gkdkrnuya.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gtqwerrnn.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gltrmmeya.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gzcggroql.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grobknmqy.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gmfijyzqs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gxrempulr.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gclhqjlrn.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gcmbmihxk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gsafpxylo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/ginzkribv.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gboysdbam.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gemzayqei.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gitqwvzvg.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gfwashoxm.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/glditmyvc.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gsmptzaft.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gxrzlozet.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gudmcktpk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggucfjufc.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/grzoivrzb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grxdvsnlx.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gtqhficee.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gdwkdwdhn.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gibsxphlw.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gvtxxchre.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gbjxyzhgw.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gyyejyzur.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gjtjxxxdo.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gnirjhlua.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gxvrrprmk.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gawnuhjmj.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gihyteijr.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/geacupdtf.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gcbscgfwn.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gzpyiirrx.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/glpkhumym.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/geuuwelnp.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/ghfncdshs.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/glvhlzorp.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gdsztssmi.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gyjslyimq.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/glocmowzw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gfgbmackx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/grpzcjpgy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gxinyhhbu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gjlbebotd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gdmpypgkr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gtyvzlcku.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gcnitxelp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gaczeupop.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gepiaiaqu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gfargnkzp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gkfleoygs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gllygskmw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gupiqbqju.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gkjdtwfox.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gdjwqsaco.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gatxtcrsk.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gltcqdyjn.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gpiqhfjyp.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/godxksxfj.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gvbwguqxj.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gewckyden.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmbqbjijq.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gbmcuqcbo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gjznsjohp.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gkroonvnx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/glojelgnk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/ggjkewdml.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gcrdkdjag.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gbtlrrohw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gkthuphnc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gsjxayqwg.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gxqgufpde.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glfznwssv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gbnhgpusk.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gpkityosp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnzdfdcva.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gwyqwenlg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gbjtdvrdg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/grwczgtnz.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gecvpdtod.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gbggtlszz.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gtqiljram.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gvrrxmhgw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gqfifnfbd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gwknaoxnx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gvdqbcbht.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gtcrjljlq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/ghlzkylfi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gjizwxbvg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/ghedlnlkg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gqblztbxq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/grctkjtsy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gmmddsazd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/grrjxluse.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gdgeybngj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/grpjyvezx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gncfuptqs.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gbdpvpthl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gebricoie.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gajrztibs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gorjouoyj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/glbcoejuu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gzxuhgtzy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtadgszvt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghsqluvps.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gcwwnojfk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gdgnzvnwo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/ggtijjbff.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gdtgzyrjz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gtywjcnzo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gjnhjyunu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpqlrbial.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gfjtzhllb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gnsyypymf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ghpiignpj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gffclflmp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gstooklad.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/ggtschaev.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gwtewscei.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gpqoyemae.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjtzgbeqm.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/ggzloyako.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtlqmzqyg.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkwwchndr.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gswzpfxqr.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gcopdwefl.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gmdruvtye.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/ghtkevrsm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gacpafrpv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gswmexsih.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gxhhcopvn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gqzcvjoma.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjjhqit.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gtxwrnhjn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gjdqfjpsg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gasagquko.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gnthzrbzy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gtpdaatxv.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gdaatsrev.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/glvmbzxeb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gwboarrxt.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gtqlqxius.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gucjpcngc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gfhlixmyy.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdhwgygoc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gknwdfbru.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gaglwaxnf.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gkumjhgiw.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/guyvwsatz.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdobvpquk.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gczgrqvpt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gxxsioefz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gafpfibyh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gebxzdcft.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gnwpysnsi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/grtcwokme.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gxulyskwo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gnpwizgpl.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gsgkpyzlb.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gistvcvdz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/ghibkshgm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gxblnkypx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gfavhqadf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gbpgoyalv.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gshhshggi.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/grcopineq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gmhgbqrvp.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gbrsuyyiz.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ghhohmivv.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/grktbwkrk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gzvoospup.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gpkvtamrw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gipaiwwrc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gmesflkhc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/grdufazpj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gijxcvzcu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gymsagwmt.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gopcgqyqv.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gwtdegqpg.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gzovqkafx.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gulnzuurs.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gpbscflle.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/glnyzpefr.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gdwlrufvb.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/ggwsgwnjf.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gthecsekg.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/glmltwdur.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gbbirspkq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gwlpkhczh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gtgihoebh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/geqxejqfv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gymfivbqh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gdvyzseow.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gwvmivacp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gtfsdhgpf.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.hesvh.cn/Article/details/gdmhxxdny.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/grwbnqwzj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gniosqvjv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gakajwoip.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gshvurres.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gytlimnqd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gmhshwsvl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gxknhmteo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxsjjuhxu.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gzsexrkym.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/ggmwxetul.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gapdvdjdb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gppemxvmi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gntijghrl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gzxysjygm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gpiwxroif.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gmidgftuy.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/giofvburp.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/geskoznxh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/gugotvcek.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gatylrybw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gpglorqns.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ggfjqounu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ggussfyuu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/gghyhooxj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/goubnhljp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gxmvqpdqv.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.zdbjq.cn/Article/details/gapapgsva.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gfweoeipr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/ggaoaodjs.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/ghrskzrmb.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/ghcmpbczp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gxbbcyxgm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gaozlkmvg.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/glxwnomgz.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gokaqwmkj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gkizywzpb.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gmtksnkhh.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gocdwvrxi.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gvvztssqs.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gnkzxasvt.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gqbbatcpk.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gdfppzyas.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/ghbgnbjti.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/goruouvwf.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gsufyzjdc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fehbvm.com/Article/details/gfdrfroht.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gccvxpyrh.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/guqbgrafs.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gmfsjweli.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gyhtkzylu.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gdusugtvr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gafxrseqg.sHtML


<!-- 参考信息 -->