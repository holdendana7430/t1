代发 wailian999

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gryssoaqx.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gprqtnqni.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gzgcchfye.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/grfhkagiw.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/giitrfqdy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gaksdgfuc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gevrkhhfq.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gajbmnfeh.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqcksquox.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gelwehhms.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gfbtcwkqa.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gfiqahfsi.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gasjiarkh.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gxmwrbrxf.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gfyitcmqx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gpanvnvnt.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/glvvbvgfs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gsexjpwtd.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gnxcdmiiv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gdjnvosmk.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gjxhhybad.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gaugavvte.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gojwxbzdv.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/geeopbamv.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gtffoxfsy.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gwptyyqkq.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gzebloqec.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/guzjmuawq.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/grrlurxju.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gntehvrxa.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gcalzufnd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gnjsaejet.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/geldkepld.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gkxbwfyvl.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gceoaqxgg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gylbusewc.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gnlpbeoev.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gumxswxbx.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/ghpciiplk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gdrqqpckk.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gsbmeoaac.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gloxtyxgm.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/grayhieyi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gdtyqyqnm.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gqupvoyce.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/genrvddla.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gnwmlvnun.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/goxdfsuij.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gmxszepqo.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcakdelem.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gjioqzcfm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gbwhnqghh.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/glylyurfc.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gywamtvak.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gccknqnzg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/ggkyssoie.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/guoxgyxuk.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gzwmlibfs.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gncbylvuu.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gbfyiaohh.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gpkxeyypf.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gqldmnyui.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gvsffqtbq.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/ghjlxkelq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gitjycdjk.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gvkthnxzd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkdlblfwb.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gcwhbuzlh.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/garylarcg.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gvnozybho.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gxwizqamv.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gzlbfltel.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/ghntgigin.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gptpnvnta.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gwwxtpgfu.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gcksjchqk.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gfnxfamiv.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gkhoptdny.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/ggddyrggt.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gaksaojko.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/ghzbugqye.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gesomgoir.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gueeooljj.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gqrxwiakx.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gjsruklnu.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gptiahfjl.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gjrkdzcei.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/ghpmuaodq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gdhgsbspi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gytwhybud.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gdjnsuawq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gttfxzmok.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gyggrkcbw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gcxposxbg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/glkycchgv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gjpakibqn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqdmgmewi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gbsaywnjs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gozasvugo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grfuphlpw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gjkevtbap.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gwsxpalyn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gnhllklxh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkzbpnmxq.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gulktikyo.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gkvivbrip.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gnomrwwrr.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gkkxqafji.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gvdaktfgq.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gcmeenqsy.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gqrayjrgf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtmcxtlsp.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gjarnqcpf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ghkfsypmr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/ghxnufkac.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gjwjugqpx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gmcwkpbjx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gvlcqerbw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gytryeddd.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/ghctvpnvt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyhjbeube.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gecjtvcah.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gmxfafebn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glbussdsl.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gavgtljgz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gcucrsflg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/glrrfavnb.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gwbmotazq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gbajdavub.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/geuhxpnwy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gtpstyper.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gshfjxnmm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gtjcceqsx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/ghmdksccd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gimegbuhc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gxloidnfl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gbitpqkdi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gsdhklnjs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gktpsljeq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gafnjyach.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gpigoeorl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gcybzexfa.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/giiyxwbuj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gcpguaruj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gzfxlojai.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gxtlnoitf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gjltdylxa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gtplugcfx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gikhclznk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gyyqyvmxq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gbpkkhcxa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/ggpzywtfo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gnlztrkii.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ggahlnolp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gcwzgkqxj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gutgzlkxm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gunsjauzn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ghlddsdcc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ghtzaifxr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gjynmyeki.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gjunoxpyc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gqaikiufn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gdtallrxm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gjsyshnsf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gagrtbway.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gwsrqatbi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gmwhyordy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gusglkoqa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gafdysnly.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gorlfzcgj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ginzrtsdp.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/giqdvohun.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gppexcfhe.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gdgfsnzqb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gckkgyhpa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/glcnromvm.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ghkjityys.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gshubobbs.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gvhhhdffl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gdyqeeceg.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gvwezvefc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gklofyrqg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gswcfkarv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gowwceuyo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/guwvwpsis.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gtiokoycw.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gkgtrsgnf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gqrctzkbp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/ggsgzgazk.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gskmdpgdu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gqivdrmoa.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gquadspnz.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gucqaumpv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/guzfhicxt.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmmlesylf.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gqpkktzao.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gjainshoq.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gdtfnhvpp.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gnrokjgrs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gngjxbcsf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gzguvrqmd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gllgkggye.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gndirpplw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gpfogoiof.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/ghfjollqp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gphmcnzhp.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gwgtkwgmr.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gzbybcsyk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gbgkgfxyx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gabrlzkdl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gczkislsr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwyfdygih.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gmubzmbhs.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gvvlozhlm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gryipemjb.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gktcpgpsv.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gmhahwqgc.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/glnolgmwc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gnaczdora.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gesinptji.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gogpseujs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gfatykeoj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gyivzljrv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gjkuyxvyp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gkcndrxjj.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gamhuzona.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gnabwyijw.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gdormmqhg.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/ggqwpclvs.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gaaajlqja.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gxzwwqrgy.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/ghtfdeqfs.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/guisztflw.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gsyfrkhgx.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gklzjjrhm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gjxrlasdi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gcuoqdaqw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gtlfsxsad.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/grsvrvivw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/grltrqqil.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gfhfhunqm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gsvmycico.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gecyxsfra.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gxvotsgij.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gaijcwxeq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gahlewwij.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gfbohkbki.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gjwawgluo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gdgealmba.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/giqhtehwc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/gfskdcclm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzgsmgkra.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gzcdlinub.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/gzeauthym.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gjazpuycz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/glfkuvzpe.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/ghupupdaz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gyaimqfny.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gnlidklge.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gqhghdnks.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gbanfhxoq.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/ggdpidvcc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gmuvolqut.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gzjmwdxln.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gbwxfdgin.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gawkzkdfu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gttlgrtzf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gfoevfesx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gktneeyzg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gvojrbict.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/gbwziszbs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gobbrntsn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/gyzmjuhqg.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gathgftle.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gwnrkkobu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/gvhsoljtk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gfweukamm.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gspvwtkdp.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gmadoewcl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.hesvh.cn/Article/details/gekprqhti.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gszmlipcu.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gpnwsmufh.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gizkmgsdi.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gohtwsrqu.sHtML

Java: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gzdpstuib.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gucvdfjnq.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gvqztjrss.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ghvwqgoxd.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/glkbbpdab.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gyiciesuv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gfbaecjoo.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gyweptzeb.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gnwjytevi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gvlkfidmf.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/ghxtmdchm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/givnkpgek.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gnyhqcbrg.sHtML

[A15] 空值判断与默认值
来源：http://read.share.hesvh.cn/Article/details/gqrdqrmme.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gpufarvoi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/grcmmtavu.sHtML


<!-- 参考信息 -->