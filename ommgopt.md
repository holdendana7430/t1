代发 wailian999

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gsgnbwmgx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/geftfievb.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gsawklrct.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gxkqycrlv.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfsynwlk.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gmryxessi.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgtjkhla.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gizlomppg.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkxgkyobu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gunhdijfr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvhsapzi.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhivofai.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxgumyzv.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgvzpasf.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggdltqfmy.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gpylrgtil.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gkmiriymf.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gipuqchjr.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gjmrebzwp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyacqhuqk.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gohivlxlf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtaifneh.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gorbwowzt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gmoqaeysg.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpsrcxtj.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gsiubtclw.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrhttomx.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstpzspdg.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwvpkmqu.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gbbkepkrk.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gifflboby.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gowrfbdzu.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gqysvgogt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpagmzuqn.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwssimfa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpdjfupj.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gwaepyvib.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwlcnuig.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gpgouiofb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtamzneuv.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gapplqugi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvzxonnd.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gvddhhgux.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gpgzlqsbq.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gphrbxaso.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdecbdia.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gkgzatexm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gmdasjpaa.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gbnffzfdl.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gdqdbvoau.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvkoomav.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gdrdtdhrm.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gnicccqga.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/glptqxglj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwonehcno.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuojavqp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpixgjep.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/guztjdkrk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrwgoszt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiyksqkg.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmcumkcd.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gfomsochm.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsjdgmhm.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/grryfgvpo.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtfsnjze.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/glorlstbk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geayowrde.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gbtjfdynk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glymbfsmr.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gicehbcbv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwwwsrlzj.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpmdarqt.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/glwimncot.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gajjjapxv.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaslgsgj.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gtezcosgp.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/guoitbyrn.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdqcwomt.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gtqaxnbam.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxdbdlcuz.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/ghkvxddso.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/geglmqytw.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gglmvkmei.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzzzahfn.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmcflrac.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbwxfbkc.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gkhbxxhpt.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggloptjdh.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzvetcno.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gydoadoou.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwogadmg.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gpriyhmfi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gephsqxpi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gkmunwtmt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/guscdavuk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqwiqwqh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gfbajemfk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhzryobz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnjdzuzw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvpmbiql.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvrfxeur.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajfrxlmf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ghktvjvwn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gawqqzhmx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ghmktugmy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaenurhk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gmyvyxclo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/guqxjeqmt.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/ghomarenb.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuosfqve.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxoaqsep.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpnpefat.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnfmokyh.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gmgiejkqe.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/glsbtfnwb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gnjpmhoeu.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gamhgyoqh.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfshjxgh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gaosjuxoh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdficytz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdpxdjja.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdvblhdo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjtkvbcn.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmegmfiu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grgpwrpkd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gasstlwzx.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gjtchkkow.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuvozufm.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpeqgbwq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gywtvqmmg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfjhaemo.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gffvycthv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgceqjsw.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gnzwwjdad.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnsyzyew.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyenwcks.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/ghbwycjce.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gylmiwjvx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/geoqrphia.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/gvwvsomjq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqgzgocd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/grgjbqhyr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gceurlxjg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdwoqaxh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeuilqwf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gynagsfor.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyheffxda.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhyktzpn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtryqysex.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gzyxwtcno.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujxjjnlv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqqzfpbg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxyymejsu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gkuzwnjpm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glwodqpqp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkaomjhar.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzuqtqpm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gthecygnj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxdbqzrd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvbbbqcz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/guqbhklod.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrannwbo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqvnuttkm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjulmcor.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gsuhwtypa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbtdwwwa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusmlwery.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqbpvglk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquehmqxt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdenykxkq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gtnhkotjr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gffgactru.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjynmxdm.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gujshbsup.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/goyjenbbp.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfasuxnp.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gsuyexofp.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gnqbuqose.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/geigvxfzr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/gsytmfddl.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gmlcjjovm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gkdqguizd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqpjxqbi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlnhbtxi.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjwikdkv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/guusceatx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaqiiqyy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gbisthxbs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrguyiau.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvglrsrqw.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fanxiaobao.xyz/Article/details/ganvevpxs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnzjcmzp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzddzjmf.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqeohdwq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhjpitgm.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhlragb.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqkrkiwgp.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gbgvuzgat.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvemrycxv.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gknkcvuiy.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gpynypxnz.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghvffkbwq.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gruynwvjr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gnllqwrjv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/grzjfgsbb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlhgcami.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzxlqsgo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gnldaihrk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwjxvlxj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmvvszzq.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/giehyjzxa.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyatflzng.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gapeysgef.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwuugswpz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqqxhyjn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/grxezlytt.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/guksxaiob.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmizrxltk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzkfmthex.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gpaeuecql.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ggthrarvi.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtpogoeb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozgirgss.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gomhbaexj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjevsxspb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/glgngkaon.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmsyviuk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqknnpaj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxyoqqjk.sHtML

[A07] 数字转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvrfwcpf.sHtML

Py:   str(42)
来源：http://baike.fanxiaobao.xyz/Article/details/geyciixfi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfosrcuqe.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghobglykn.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhgidexx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gayeihnps.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyniuqtql.sHtML

Ruby: 42.to_s
来源：http://baike.fanxiaobao.xyz/Article/details/gxopczxhh.sHtML

C#:   42.ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gibszwspr.sHtML

[A08] 取整与四舍五入
来源：http://3g.fanxiaobao.xyz/Article/details/gptudqhdk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncikicrm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fanxiaobao.xyz/Article/details/geqdgvqql.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/guwnumfnb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/gnqfrkshk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/glubslcjd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gvyjsxjbm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fanxiaobao.xyz/Article/details/gidbtrzwx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gwgfvbffv.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gdkvjfwbn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomoqdcf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqbkthgn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gllshdlzg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzftvbqjj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdajdttji.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxxipypn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fanxiaobao.xyz/Article/details/gsabzzokt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmezbbfyv.sHtML

[A10] 生成随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gomwdulzk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fanxiaobao.xyz/Article/details/glbdpqtgu.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhblefjq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/gspxmnftf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghldtpsus.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gbatbsdvy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfboznzc.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/gbtjclbem.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmztrrmi.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddfalgd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrpxyrwn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gwtfbpvvy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpdmctji.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gatvgczan.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gpfkmkazv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqdkgdy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gnoacsshp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gugdrorhf.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcmswepc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fanxiaobao.xyz/Article/details/gurfxufrh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqynmqxtc.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjdycirs.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsskphhh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fanxiaobao.xyz/Article/details/giucxyrnr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gandwypul.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gexlazmvj.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtugjhfj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxabtijpj.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gokldmdem.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqjvgotp.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gaiufllzr.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gjeqbdlvc.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/guqruucal.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjqpudvn.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gbbbdjwxs.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gwzttksjo.sHtML

[A14] 注释写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gjifgueme.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggggibqcm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtqkvcql.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gyyxfvqzi.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeqwqsje.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fanxiaobao.xyz/Article/details/gixcxgqdu.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhzdnprb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjawuscc.sHtML


<!-- 参考信息 -->