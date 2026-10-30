代发 wailian999

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrivooux.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/givciievl.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glcywofmt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gnulqwgcb.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gnefttidl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbxqhhvx.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/giewikmrm.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gvgxisbig.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpgxoccv.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gtozlydly.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gywkyovnm.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzpnvfvz.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfxnsymi.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqqyjsoy.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszlpnvvf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiijddtj.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlpwldiq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbignapqj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqokghfb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/ghdgepjje.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gokbcvdbv.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaijyufpc.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyabmlyb.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gexynkxfa.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvcvewxq.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuzizgrz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdewiwiz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmebvrdey.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvihiuse.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcmrvdrs.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvswwliwi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdkmvjnd.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/ganreirow.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwxmpxqxv.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghllkixkc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gdclwimay.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsbzqtjg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzmuferv.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/guusnrbzz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gjwdqmzii.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gviwrodmb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzaifinl.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/grapuruex.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvahlizuh.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gpzaneoga.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gnmjdbgjn.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/glbmdwkzd.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmavokgxe.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gydmpxorh.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpywbtvnm.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gnduendad.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/ginkvhbvj.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmjliehv.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gpbzhgfcd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gozmjpcpm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhggpjcj.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/grpaoleax.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gvjyrkiyh.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gajimpiix.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gwnkvhzpi.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakyyqxvm.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvjilfi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gotbenxbj.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gtlvaxyjh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdcbgcnz.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gfmynrmon.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghfzyjith.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/giblaycal.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjhxsrlj.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkfsqmjg.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbodewed.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/getezfafe.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gpvhjtemq.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gyivcxiga.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gehcdmrqv.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrysparv.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gzciegbzo.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwjyrjlk.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gmnvxsyum.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoesakts.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gksuawytt.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxejrbvw.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gdawoakxl.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gzjparoly.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzmgaoqw.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkdptrdt.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/goejwgpoi.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gfywjooll.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gmglknxhq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gainoqnti.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ghzgbjwgr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gqtsjknix.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/glvceubch.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gfxhkmlsv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gogusknzq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtptctem.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gfhubxjrg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/grlzjpeyu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gogsorqkv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsrphxrl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdishdjo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcohfrefs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzdifqea.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdrjarec.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfwfsibp.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gerknbuna.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gdavqxvpz.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzisdxfvi.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gptvzovyw.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gznoskdpe.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gjkawjesy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gcrrpkryk.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gpjwkekor.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gnyjiyvkn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdtupaqe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gukzfjcxh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbloxnhv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gbilbwuqe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gbrotvkoo.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlcgrtdf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grhmrjfnc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gskoqgwha.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gjezdyfcg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gknqdpmyy.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnxovvam.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gainifqrg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzzfpzsn.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gijodymst.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gyirhykhz.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gtzbijsru.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxavxnlj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gjdthsnev.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqtcgwse.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gixnqidsa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gstgudpgk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/glhjdthej.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnanxlgvd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/guctowqat.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrifepfn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gjxsonsue.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/griiiqopg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gzaozjaxi.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhjuggnj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gxgxomvyv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gihhmuveo.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/glrvukmgz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjhgmkgi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gomzggajh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/goqpiemnb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsszbeugv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/genxlufdb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbtqltfn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhtnilrx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvxvxjuc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsjkbbbf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvozvljk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzygpkfjc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfyasncph.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gsnpqkikn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvpwxljh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsnidqcf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbkrqgnd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gabfmppqd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkitaubqx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsyxgvnp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacfqlaav.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjitvzbxc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgyiwhum.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpviryai.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydxjlnbh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmynddoh.sHtML

[A01] Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjiwbvwbe.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbzdipza.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiljudks.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gpimehmxv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbxlgyoj.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxkteaxb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/geeshrlyr.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gleopzqvb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbvinohj.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/glrvjfxaa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/gicnrwvyw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaljpjdt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gijrvovbb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwddxgpnx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/garnqifsb.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbbzzttt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gjensugnd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcxmpvtc.sHtML

[A03] 常量定义
来源：http://wap.fanxiaobao.xyz/Article/details/greqqmptt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/gakfoepxv.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxwejyssp.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gnszahjwt.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtpaeifi.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gezittlxz.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gbaqvkfqe.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyznydldd.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjzydrxu.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvqjvnyw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gcgfkvyhc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdcjesec.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysvvgamb.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gycuwcoja.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fanxiaobao.xyz/Article/details/gmrwjnjbg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbarwxkm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxushyiq.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fanxiaobao.xyz/Article/details/gigyuxaax.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchgkwolb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ginwmzzsi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gednoimcr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/geefqscaf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtenudsre.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gersawonp.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpwkpdqoo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcaskayu.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxfuqxchk.sHtML

[A06] 字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gdghvbzmm.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gjjkxnxkt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfwmbprl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/grdbxzjlx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gslftdmpm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gfdodapgc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwowiler.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fanxiaobao.xyz/Article/details/gllmbqysb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/glsbwkcdm.sHtML

[A07] 数字转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzcofvdz.sHtML

Py:   str(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gomddadwj.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqyfszik.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/glbrwlkyt.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcolzbknx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gensuvupk.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gilstpcth.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggepnvpoj.sHtML

C#:   42.ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzzrfbeq.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/gjghcqqnp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmujsddx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabbvbvxr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwltyqod.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsyvwhac.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlawgpvg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuhhouqw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/gxmnfkspo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gflwnwxey.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gcbqtrtvx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gavyajyqg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmgzghxkl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkscaiqlm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehsxeuvi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gyrlhmdae.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fanxiaobao.xyz/Article/details/gkndcwbvg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/gtbtomuni.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbdmjglcc.sHtML

[A10] 生成随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gllvvmlkv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqsfdpub.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fanxiaobao.xyz/Article/details/gihythqfc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmumbfdwr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gezwuxorb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gyycefqrh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fanxiaobao.xyz/Article/details/gbbatpvlc.sHtML

Ruby: rand(1..100)
来源：http://baike.fanxiaobao.xyz/Article/details/gpnbcthfw.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fanxiaobao.xyz/Article/details/gkwtusozb.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fanxiaobao.xyz/Article/details/gytpsvswc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrdgeghq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gwewzugtq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfkiudzt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gscknnavx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gmialdaat.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gowhddzqr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gnhxhqsbz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gokprfzcx.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyjxiag.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gboihhhyc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/gmsfrjlix.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fanxiaobao.xyz/Article/details/gqxyxcelf.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gamynynmb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsomgywhp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/guoxjiopl.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhtvahcj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsloupav.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlagtqge.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvtjhlcb.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmjhaxco.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/ghvplavfa.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/ganznufmp.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuawscun.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqbfgaiy.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gitbfjwrp.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gcgnuzwcz.sHtML

[A14] 注释写法
来源：http://wap.fanxiaobao.xyz/Article/details/guwpnjoeq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gjanwidtw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gfhveppot.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gawdupmow.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gampmwpje.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fanxiaobao.xyz/Article/details/ghftihdzk.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkolebut.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwiwqxud.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gjhhergzd.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawroqmjs.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnokhvqhc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/grjrtyrzf.sHtML


<!-- 参考信息 -->