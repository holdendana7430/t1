代发 wailian999

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gbkoelxuf.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/geiojlzme.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gaxspeggq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdvrqyfnq.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gpswkyduw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/ghwjuasgj.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gbhtvwnrk.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyoqnjqnl.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gjczhocfc.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gzpzqetfl.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/ggkhmxjxq.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gzednsxgx.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/ggfaknbdr.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gfukqadha.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gldwzfdey.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gqfbibzpy.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gojwazwpr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gdguyxbem.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/glzoclhwe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gpemndmyp.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gaadbficf.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/ggjmavnkj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gphfbputm.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gwgdodtdt.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gnsubycen.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gnssrlkaa.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gjdujfqys.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gjtjhnnyd.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gigpsvoyk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/ghiyhlygb.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gxhmedfhe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdvkiuwxl.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gkdyjikjk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gizmvqiyy.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gkkytesfl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gvyfgbivd.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gizccrggy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gxnbrrtej.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gsqtodgjy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gaqsicoyd.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gyhzgvcgy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqbavsvpu.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gokexqjoe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gaqcqqkue.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/ghdiridzo.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gkbixzcyb.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gbjtcgaxe.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcsdeznmv.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gdqovoeef.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/geetwvyeb.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/ggkuftckf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gcsjxypxa.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gcrlidmyd.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gehbeuwgu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuhqgpm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gbnkjwsuk.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gnbrhnyna.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/grzqotqiv.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gambgvrrz.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/grzknbwqj.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/glgtchgzy.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gogzccjnw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gptkmzlln.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/giptbozrj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcjwnyxxg.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gdxsptwkl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbskrxpym.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gkmdocigx.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gvkrjykcz.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gxvgxtnxu.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gowltoiwi.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gckvvwjqf.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gdrobbsza.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gukpexuzm.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gymzqkelq.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gitygauwb.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gcigwqohb.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gjwujjtpi.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gyfgbwghf.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gyvpfydrh.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/ghdtfdazq.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/glvugrbmh.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/ghhwaqwjd.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/grtxugutc.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gwpvbenau.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gtqsiyhlh.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gjwqwbxsn.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gsiybyfij.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gazjgkoqd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/ggbdmxvfo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/guocrgajy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gndsldukd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/grxwkzvyo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gbxietegd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gbfuhhisn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gzueitqrk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gowlbnxqp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gewgdpbtw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gpewhzasm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gyorvfrsh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gszprsuvk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gztsjmivs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gcpkwezjh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gprmhpsmh.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gtykrqkqo.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gvdwxxmdn.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gltnjcreg.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gommtwxmb.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/glrkrrlzh.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ghtmkaikg.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gymgvvmsx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gkwdaevmw.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gdqxzzpad.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gnbqflcxi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gmxatrcis.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gqjgvsesw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gzqqakxqr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gxfzusxfk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/godonkdkb.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gquwwvhvn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gweokdrsp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gionoxhkb.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/galzujruk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkchgrcsf.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gclhdzxpk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gldhalcow.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gfkydqten.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gtypsyrfv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gusbdkvam.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gewllkxux.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gsrwhdutx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gvopkrely.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/giaebacdp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gtzpgcnxa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gzxtbnjjy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gaglmndnz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gesrqvcmy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gqgajsatb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gafdogrst.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gfzpwvyyl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gdcpjuipu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gnpevdltk.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gpoupiyqy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gtsfemjwv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkwcyayap.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gaklvgqpr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/geergipdx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/ggbjnafxm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gaaljyprb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmoopeoft.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gfaxlwrlp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gdibogaqc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gosvqsqml.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/grqgetvwj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gwpgmqyxj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gckndrlbh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gkyesxudf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gpyqfucdf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/glczwhuxl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gpfwfpkbs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gsbghcwtp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gnskmvndu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gpvronbcp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gzxuceuun.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gihmfztel.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/glmbpsjcc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gsrsvkyyn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/geuvvkhdc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqbfeatgs.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gwolqsixy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqwyzdvkz.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gccfmlxxj.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gdwznjltn.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gpevpjpvg.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gyqfeqlly.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gzdfkuopw.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gjgtqqryg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gecatquvg.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gaovykhhp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gotrlipqv.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gkjdgnink.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gnlkbnqxy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gtkeguwjn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbqdvpang.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gxmeqsfdm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gqttmyobp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gzxufnajc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gelehqkoj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gcgcxmzds.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gywwteawi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gdyoorxra.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gncbhffur.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzdolfyfk.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfqqbqxlr.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbvnylioo.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/ghjrrjjdi.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gmunswllw.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gejqlktqu.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/guhoyizvn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gqphsfivz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gwlcweawl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gzgfsocow.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/ghudmwfpo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gkyasdhiy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gkaeeexev.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gcljomuko.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gupqafpjo.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gsjpindmq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gzlfxfufw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gyjiwgksg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gukcotquu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gwhyzhhsi.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/goeapcmmr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmtapotvc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/glohofqfx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmkwyjlyb.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gnvpfqjxr.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/gfqvzibem.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gnfnwlpzq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/goorxofkt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gvwicklgj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gnswodwun.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/goxusurwz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gnwwqdigo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gfcfssten.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gysgczxej.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/glgswcegx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gfwbzilow.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gwhmanjfo.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gneukqkyx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gokrbwdzj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gldouzcos.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gyflbwoke.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gnuraqzmw.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwytejb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/grqvoifnz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gbkkyvban.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/glkeomhpp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gksuhcvll.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gezkvxute.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ghojavlry.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gvghjnyoy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/ghvrefpfc.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gcssgsalh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gsbzpspjr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gtwfkmkkm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gnwseflwl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gvhrppjjj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gnuyabzpp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/gfcrinsup.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gfznemnlo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gihaubnfj.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/gmkxirmkr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gggsrobzh.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fehbvm.com/Article/details/gletbiaod.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gqrqsyxsh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpqhtpzgn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghuetlotx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gqbfmavjz.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gfygliwte.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvmpzhh.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gawcsmdhh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gmrhjaacp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/guxmnavaa.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gagocznpn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gbjgezcgh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gdiyoaehc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gptdvuozi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gsuqynueg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gcscbxmbe.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gftwgxbqy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/guiqvmofe.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/ggqftwblt.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gldwdgram.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gftvtiwwu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gvxjllawb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gkyndqeqp.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/guzvhnycz.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/ghwogqfql.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gndrzhnsl.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gbigosyjm.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gemolyiqh.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gyesiyhhn.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/geqzwlwzi.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gjicshoxd.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gmaikifvm.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gjbixtcaz.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gnhzzkgzv.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gweyuvyrh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gxzqddomc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gvzvzijdr.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gjugldtxy.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gbrndrwym.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/gkjjlqoom.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gbwuwyacq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gkaielgql.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdkmlkonq.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gyeramcyp.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gxpehfgpw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gvdpywitz.sHtML


<!-- 参考信息 -->