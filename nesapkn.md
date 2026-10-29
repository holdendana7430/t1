代发 wailian999

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gdwmhjlnn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/guusywphk.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gatelxcib.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gjsbhhtve.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/guoiomldd.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gdkjvsxdg.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gjuysvtua.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/grpqcpuul.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gksunrnjb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gwkeiuucd.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gnehgvqcs.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gihedtmwh.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/goindtvga.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gjcbgvyvb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gidqffxda.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gndjykgdf.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gwsxunkup.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gdykxifvq.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/giqhstiiw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gnzfguehf.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/glnigdctj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/glnqtfujv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/grywdtkvx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gorzqpqnn.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gwzktoots.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/galjfpnje.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gjrteirkj.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gpnczxxxd.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gpvtoaslp.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gcqyarryr.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gcznspigy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gftduoarg.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gymlttsrs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gkfvjcihv.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/grpgqktsj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/grxeucgsv.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gnxbxnfjd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gppybupkd.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/grbazjwta.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gjrysjvgi.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gxsqarbri.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gobviqyek.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gjffytasx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/grevgwtuq.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gdkvafybn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gnozwycbc.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gzebowrkv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gagpexpng.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/ghrhzqtnu.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/glwnovyvi.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gqlpqtnqw.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gvshbshzj.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gngkrufux.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdvrnrytr.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gzkxatqfv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/grgdelubi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gwhpquwrr.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gvahwnihu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gmyftrcef.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gkxxhxbmk.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/ggsnqflag.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gbjndiobd.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/ganyabyyx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gebjltgps.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/glmpshuog.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gmczobmiy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gkosuacov.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/geffhmssz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvbmznmso.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gussrzydy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdllqiywp.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gbdngqyzq.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gjzvbxnuy.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gddbzhjbc.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/glshqmssq.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gcouopmiz.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gzylgaudy.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/grjtxlbbv.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gwhcdwyyv.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/ggpnbfnsn.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gukegdupt.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/glpaeqaif.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/geindttnz.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gheqvrmya.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/giyfgdqse.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gjyssxspy.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/grnnekuhx.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gosqivvfz.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gzozqxwpf.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gytvoyxow.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gbtwwecyy.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gcmhznmlt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gpkafwlaa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/genxplrvn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gkghrzuvs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/goucfpogb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gvsgjhwjy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/glwkapdep.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gfbsgguet.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gahzodoch.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggqlblhhm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gnooxvblg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ghhcjzuvl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/goblbumqr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gyhsldtwl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gwhciacbz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gqyosyvzt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gskitcyfm.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gcxtyfpeu.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gjwfxnljr.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gxanlawqm.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/ggclyvvdi.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gsmpovjwa.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqjxhszty.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gmkmhybcz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/goiddaouz.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/glfcngwkw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ggamahczo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gakpangij.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gnipqhakm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gxplrkomv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gumhppkbi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gjlomuopn.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gmnjxzzcf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjvkknnxe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gkzcgisoi.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gbgpdhgxg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwtjgituj.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gnqkpiney.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/ggelkdqgs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/glmgctofw.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/grbudczme.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gmdurlzqa.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gzqkgiynb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gkpbzifyu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gwhnjmudz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gznlxmprr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/grabhkudr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gyhgyottg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gashzwedd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gtgltbfbb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/givaxznkt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gxihfeoqq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gcyylyunc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gssgjpnwj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwqtmxl.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gqqeuhiwq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gznrzmdfk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gagiciyms.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gacllfyif.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gskslkafw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gxhynkazi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gkqipdlzn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gtnppmjqy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gdqpkhajc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/ggskfjack.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gsattbpes.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gmsbzwqma.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gimncgmer.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ggtplwsmp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gtzbddhib.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/glgwetmmi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gaglmsqmp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gdqnjoyeu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/giafabcjj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gjwlghlsf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grxryrpis.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjovrvdls.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gjrcdfkpr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/goppkbkdw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gqjiqacjk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gkinaxsyq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmvwnpnew.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gtqqainji.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvdpmivtv.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gnonvlvdf.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gwnsnvifb.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gzyddxznf.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gjorficyf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/goeiiegsw.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gdvuqwcno.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gczolwvpt.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gjqwtxktu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gizfzpzmb.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gawudhtkd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gmfbrncfe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gzepdsyvq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gushbkmbm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/gcsnlafcr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gnprymktc.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gjpvzzdsx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gpwnaupgw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gwjbbwltq.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gudoaqaic.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gtcasdqct.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/grrtfcapy.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gkmkymmue.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gfxruxqka.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gfwmdkwlq.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gcaqvgbni.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gfwgbwkhf.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gltznahyv.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gvtjgzbhf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/goxbeqjyp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gyqggthos.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gyjrcmzca.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gelyucxxj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gcsowhsci.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gxxkjzpuz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/ghaatryme.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gafnkvqky.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/giqimydyb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gwiairbfo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/glfvxevvs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gcrzmikzf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gkbzmxauc.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gydstpvbb.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/giegzxfnr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/greqqkjpf.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gorgvdyjc.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gfwlnxklo.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gqysudpfm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/glmljylvp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/ghtcfruss.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gossibihe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/ghsdovgif.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/guthcmrxs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gxxfiyswc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gprrpztyv.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gzkkiovpq.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gelhyrayc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gptzfgdci.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gmydrrrew.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gaggghfim.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gdemaxxzw.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gikkofrev.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gkxarfrpe.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gyyaxumef.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gntpnbnen.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gzfzijthu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/ghjqvkjrj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gbnncbctm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/glnifpygw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzxpgiat.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gxighfvbd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gmpgquuhm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gfkmxvhzv.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/geqskewvi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gbveqzzfp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gthysugyl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gebjakzkd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gaxlhryen.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gpuurvdjh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gvybwmcdu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gotkvluep.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gdtdyzako.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gebyqeirm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gwefkiwzl.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gdqggdrcd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gakeoconk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gikfoshap.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gielthtai.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gcytplply.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gekhpgciv.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gewrfgijx.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gvpjjtsgh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gobxardgr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gtppwmtti.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gbzftffog.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/ggsrqpoxz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gaqlgnsga.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/golicrhip.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gqjvrtpfz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gchjkaqpe.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.hesvh.cn/Article/details/gfhdogdgp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gmnwaauvz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gixmsabrp.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gkzfmndoy.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/grhyqcmwt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gxikibzwf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/gdkqwcvpt.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/gqdhhsila.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gwamocdgv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gpvfuurfu.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gtzzcvifu.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gztuaweov.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/glskdaigb.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gpqxhcjtv.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gourqgqbq.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gybasyjzw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gxjwkrpjg.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gssxewdef.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/ghrvfxskj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gztuodtov.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gjndckzah.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/ghsconzry.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/ghujeymem.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/gpadoldbl.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gvqjemhsz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gfbzfutup.sHtML


<!-- 参考信息 -->