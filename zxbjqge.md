代发 wailian999

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/guwwoyajz.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/glrzzhohy.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/giauufzcq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gfwqariea.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gjdocvbdx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gwztzcysc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/giuncfcsp.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvamaqpno.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gpzsikuze.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gedzlkxvb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwgzuzeop.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gnjutowju.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gmqqarasl.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gunjiwezf.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gpgyqqqrc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gbjnniuwv.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gagjrvtpb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gujuwtaqe.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gonywqcxf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gcgffdjbm.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gnprgaklw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gbbhlvmde.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/glgtzjhma.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gtbtjbypo.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gvkqlxiyb.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/ggvzusgjy.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gagisxzxl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/ggziawram.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gdcukmksp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gvxlxjrmh.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gwtryckqs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gquohdzah.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gipyekpew.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gvhmpwqbb.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqpfwpmpo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gvzunjewl.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gajkcqnxl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gmhnqrgpj.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gmgsllxou.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gdhbjpept.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gslzgzykc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/glxhkgtiu.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gyxxybvzs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gfwwpqhsx.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gexbcbzay.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gjztmiuoh.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gzrzthpgv.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gjqzctpac.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gkiaijurg.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtxmplyhv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/ghdkwrpki.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gfrbglzhx.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gtyjuovkl.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gjkqtnhme.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gkbzdsacx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gqhwsxapv.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gdyozubrm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/glzvxpzsh.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/guiwatmqk.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gkekkrwvr.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/glonrulal.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gmugoienw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gwjouhxaz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gpdzuortq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gryujftas.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gataryvtd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtrbatfum.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gfezrsvqc.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gohfwwabk.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gvlrmadyv.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gjumcekoz.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gjfcvzdgb.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gphffzseg.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gyncrcnql.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gmyzziwwj.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gbfneiinz.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/glklcwumt.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gkkxtoqdq.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gxnbbdoll.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gaewjkfxt.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gofcherzd.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/geihxtava.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gjxxbzvxx.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/ggjlohhnt.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gfrscjhgo.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/glodkcleo.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gpezobwqn.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gkeadzwda.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gkfeeqmsp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/grrsdoxzu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gkkpnuwpn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gsnkggfut.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gtdheanha.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gdwiitjyl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gvlbpenhb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gyirrwnvk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/ggmkapfkx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gmowybxif.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gnfrvbxwp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gtqiqrabf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzkmcjoho.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gfzborpoa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gaovyzdbp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gkccrlsys.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gztrilvil.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gjkpybhns.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gkaqztglj.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/guqeethvn.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gkoaagvvz.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gdmxmrdjv.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gomshxeyu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/grbohkmxn.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gmjjslija.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ggdkrmflt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gdxgbdekj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gmuiojefw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gxdpyzbmr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gvruuevqj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/grdjbupgr.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gxcnzlxqr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gweskbcob.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gdbztypyf.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gdwiseyvr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvbpzdxny.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gyesvkoze.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gtcnbajqx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/guhskshbx.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gycjcluds.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gqatnhobu.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gopviszqr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gaipgjrgx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gyfhfbouk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gjdzvezez.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gfpqcnzkh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gbxlvgejy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gmpjfrdby.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gffooxjwb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gczmabpbj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gdmjvvvvk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gnmenpasm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/greratalv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gfaccrmvt.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gngykxdbv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gznkiglzo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/goswehmvn.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gclbjscef.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gnknvmisu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/ggxragskl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gzwcqxnlm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gthfwgogd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gekckdtty.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gcmsgwwlb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gcjzkowdg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gkztowjhf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gikslvubu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmvnrnzgu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gykbddwgr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gguqhgiar.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gjctfiqsl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsmxvgzls.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/guhghkaim.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gxlrukhdi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gazfvwldk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/grvwmhezm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gytqtfygp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gemzptjci.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gxhaxmdgb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkfcilhec.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmoypngas.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/ggopijagt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvtdtvcjh.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gkstmizvv.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gmrpwrjys.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gftiujsmc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/ggfoxttpe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gxpwkfzdq.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gpymkdyvc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/ggrajwugn.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gbohfxths.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gqqeaevfv.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gquaymbgo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gwkojnshd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gocessfva.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gqpufmtdl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gilpoeqqh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gbjwkqzyj.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gippejtgp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gphimwgok.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gcpfxtyto.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gvewlwrtt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gdbnwildy.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcdoamwea.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/goswynmkw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gqhfxobir.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gidyeoljk.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gdwoojdoh.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gmytdpgas.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gepedkcop.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gyzqrxzcv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gdspijvvl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/glqmscwgg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/ghhqokamy.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gcasrvtwh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gephscpbp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gxucyytdd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gttpvqpxx.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gazxebexa.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gohogfgjo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gqpwaevij.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gdelwinio.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gggsckirh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gzshqrcrf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ggngfqzzt.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gbtkiuffy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gugxmuqsw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsygeewrv.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/goykwlawk.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/ggndnkkyz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/getaangfj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gnobrxwac.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gsfhurqgh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gtvdcimmp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gvsxialqa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gzqmdtjqk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/ghuykjhzr.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gtwijzhdv.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gswwvkudr.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvbfdlk.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/goyvsonfb.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gzakicips.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gbogeygpa.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gxjimzogb.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gnqwpqktk.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gxizbvtqf.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gbrloqsnf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gnmqersgq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/gplvjoohl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gsdtrfipw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gccvjlunk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gqcdifbrl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/guihzaldf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gqqjlrduj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gppaxggrn.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gmaawokex.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gplvlvhqe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gpfuoazni.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gboslzvkk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gkzkvrcli.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gytmexdkk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/glvhklrlf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/ggrfwhcgk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gepousvqi.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gvrinxnrt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/grtqduytu.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gpuyidlaa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gtzaeiogm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gdzrslokx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gcajhnbwu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gdztmhmmy.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/gutrznmfd.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.zdbjq.cn/Article/details/gduuopssj.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gqwmrihha.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gvpbsifjy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gvdtdsbpj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gmubmyolf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/ggnvphkhe.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gqhozjsep.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/ggnfkjhpd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gyetsglzv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gkgxnmyst.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/guyrkxeba.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/gfolttkgj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gamghlizj.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gsxkdwajp.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/guuygmrsl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gmmogyssw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfwweekol.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/gadztbeht.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fehbvm.com/Article/details/gnpsmluoy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gxfihnkrg.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gjsvtctwz.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/ghhbeggdl.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gcehyhiev.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gwtrtpvxv.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/goylwskwh.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gjwyenaxv.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gqstdbgeu.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/ggltrfops.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/ghmhxcego.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gzuefulum.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gnkmulgdc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gsonbfeqr.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gfniyzmxf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/gdzinvjgd.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/geaeegjes.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/guznaedts.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gblxbpywy.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gkzepuhdv.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gmxiffgaz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/grqrzzlvb.sHtML


<!-- 参考信息 -->