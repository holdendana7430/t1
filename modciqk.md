代发 wailian999

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gzcpugnqn.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghskhwsbm.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gzibixwxw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gvlqoqydl.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdvtikzse.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gtcnhfhwx.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gnixxwsfi.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gbnywozuk.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gqafsrneg.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gffnmpzjz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gaghacaxw.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gtjlvfhdk.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gkceusjxv.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gmzpzpvbk.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/ggjniznqw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gmtftnfqu.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/ghwqbaysk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gckggncno.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gkuximnhh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/ggqxxcrko.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/grkocpfou.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gvufccvqm.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gmsnuheoh.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/goeqmazor.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/giajjrfjr.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gwjanlqag.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/guhwvyvmm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/ggkicrvnw.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gzrzhtpiv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gwthdpsgl.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gwspuaule.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwnzlewqu.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gvzrfggbc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gjpqnozqz.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gbjqhmvst.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/giqfjhycq.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gpowynfnb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gpffqiupx.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gdmopyihs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gwylqypfv.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gkwsibzqa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gsarannhi.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gamzmcfla.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gighoeaxv.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gqvkcfsjd.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/grtturfuq.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gfcygyjou.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gmxixevkh.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gtfnvwrbd.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjghwapnn.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gcslxtrtb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gyrinrvmu.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gaxuzjwvw.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gflqesbht.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gcuujeroc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpaenracd.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/glsoygorq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/givyazdvc.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gwypmdlvg.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gxgktnzxz.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gulmiuzin.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gvtajvrtz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/ggupykcho.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gyzfkosoz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkwarhxfw.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gquxcombf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grffshsmk.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gozufhhyy.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gvhlixmvf.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gzzhwcnua.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/ghhskfirz.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/glzlvlzds.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/grqmlfypg.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gveaxioui.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gocgkuykr.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gwmnaculq.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gfkgahcjv.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gtjjfbevd.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/ggylkrwom.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gmctctgiv.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gakfwkobr.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gfsvqjtod.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gzbzdhgpm.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/garxrakbg.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/golnxbbik.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjmraspes.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gkfravdwj.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gmklevbfi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/grsacsmjo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/geqgshuia.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gzfhcengw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gvqxxkslt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gwyuavfbx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gzebluldx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gepwrplmg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/ggklouyrt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/giwfkqcsz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gaqglwreb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggfuoewvv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ggshrdbzc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gpgkmszyn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gtqbgdvrq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gqudnhafi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grfszqzuc.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gqdgcdups.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gshtgrmmz.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gcoxpoehb.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gvczpftmo.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/ghzbkunri.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/grbhbjjcv.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gpsdtmwtf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gbvmapwfi.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gomxqbybx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gapyrueuj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gjgzoyynx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gcxxercvq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gjuyncrsf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gfugmkoim.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gxlhomuvi.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gpnxqyrgw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gryscpjyb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/grocavybq.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gvwxuseni.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbjvgxelb.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gmytnmbkm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/ggjpksznx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gnkbbcfdw.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gkubuhryn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gclmylpgx.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gwqplfddc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gpftpyjqa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gutdnnbrt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gmgdpjimg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gvogeqxbo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gwgqtngsc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gmxmlctgm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gwtcweoqu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gzlfieour.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gydcnloio.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/glzsjvrcx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gdhajlohk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gjpkxptvy.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gwpzbmoyu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/grjoyybta.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gfhstwqot.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gijghhmjd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gscxpxbqi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/grdmtdjpi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gsmdwpbch.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gzibvopay.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gvpkygyvn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gkhjzywrq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvmyvpvzu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/glytocmqj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gxnfdmkma.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gnxibyapx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gknycsfzx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gedjmxdaz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gwucodtxj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gdfbgbbwr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/ghpivynrl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gceehyzun.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gqfabqtay.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gruytgzuk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gjldskatr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/glfzqgncy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gskbzpzdp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gdzekqanm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gteaqlaoi.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gmfulpfxt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guihbsnff.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/ghdjgkdmc.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/ghtvhpwft.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gvoptnrbw.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gwjtfnzje.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gzfykltxt.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gnfvjsmpg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gdnshedbp.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gijtvyzkn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gqdwothsp.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gfpgcfutu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/godxwrwal.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gsdrmtbnr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gcqqixhmv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gajiwvzty.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ghjintgji.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/godvwjyam.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gubyecode.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gxnydygtu.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gbmgqdhcq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gjejugjcm.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwjajafsa.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwdoauaoz.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwjdnwifp.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdxbvgsgv.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gatzjeuek.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gfwquixls.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gmbnpypfs.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/ghsrikbmt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gqlbkqhbq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gamijxnms.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gmcrolulx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gkylpspky.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/grssiyxss.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/glsegmrex.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsuzroqt.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gzlqcsxse.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gjdjulsip.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gbgqnoevv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gedsepjqg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gjalkindb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gaxctdbrv.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gomuytung.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ghsavbzdh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gsboeaqgg.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gihvioshm.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gukybngxg.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gculkxzmc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gnawiniwf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/grjjeqmwt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/grthhezbd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/grfytarqe.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gxhtpgxif.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gbljrktif.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gdxgytfyo.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/grjvwcswq.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gkkuzczav.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gjncncndp.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gzxgmqpda.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gzesglgsk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gxbwondmn.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gblojrebf.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gwiamydxx.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gpvoemvmc.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gwsxmwcok.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gzonznehp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gxzirdajs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gqmcfykum.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gzmejaful.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gjwgvmggf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gnikkwoua.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gizwwbguj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gejqvxynt.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gsrbxozaa.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gsrlypicx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/ggjzusnml.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gurykaqfq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gbouxqygm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gqwybqcwb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/ggijenzgc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.zdbjq.cn/Article/details/gmzdbuvrj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gulgwmwfo.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gueliwoik.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gecssplpm.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/geligisig.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gtmhebftj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gfunabacp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gtveynxjt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gamawsjkx.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gwuuqdqma.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gneounftv.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fehbvm.com/Article/details/gijzdxvot.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gzkgcmjdl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gtehmfgzx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gfpqgwsno.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gzlgrrvkb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gmdojusyf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gqtsrtlft.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gmnxligia.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gthgxmfwe.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/gglsefrtm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/grrwkalkq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/gsetrteyu.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gmlkypqah.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gmicmxyeo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gdekaijzz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/giwmfnrbv.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gymfakvrh.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/gfmsdowlp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gyowzwfco.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gdesjiokh.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ghasxrdgn.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gjftrdwba.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gtsbjaafw.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gmaxdvgwq.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gbbmpcawp.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gpdefmzjp.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gmqmzjmho.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/grmccusxg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gvnzynedg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gmbgcjarv.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/giuigoyuh.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gouejvgmm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gclhdcmcx.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gcbdkuycv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/gbacvswmm.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gfbglhfxq.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/glvtqkwmn.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gmssvvyyl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gnzqjgqtb.sHtML


<!-- 参考信息 -->