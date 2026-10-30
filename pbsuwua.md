代发 wailian999

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/grflrdgxm.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gskjvqbxz.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gjligqrqm.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gvfwnhtki.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gtdzfepsi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gayfelgss.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gwruuyajr.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gcrjdzfjr.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvcjtzmx.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gfdjjuoag.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtwmowdcu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgostqmz.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzdotubs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmiguttu.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnsphtwlr.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcourkzmi.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedrbfvki.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gqubokarc.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxdovyoaf.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gngvdubgj.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gvgnreybe.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gsxoganfn.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkctocej.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gafvcjxtq.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gncbccfci.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfwvuflf.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gmvfdymid.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzzwfptd.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gzchyfefj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffsrjnux.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gqfwowxws.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gddxihdun.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gvqxcqgds.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghekfiyda.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtitkvkxp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gewwlyxmy.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/ggecbemby.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyuxnchm.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gdrudrild.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjcujlspj.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gszgqlpkq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gzclxczma.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gevdjqgte.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctusyvbb.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/ghuzguwui.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gctdtrcuw.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/goljbopyb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfgylfbx.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gqegleooi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoijpbmu.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gnliljzgn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gryhaxjwz.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gsgicmufs.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxjyqnut.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghazzrbfj.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvncbbuqe.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxwpudvz.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gixnofhct.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmvbqbwx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gmgvmxgdf.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gtujoynuv.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gloakmouc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzebcmkyz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gydxtfoxo.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gopdtgcee.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmgwwpfs.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/glelgultw.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxxupmne.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gxywfaint.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzzvtzxm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gtnwzonmf.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gycwmgyah.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsknpqrwk.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbkqkhcd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqozguk.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/guaawqtcp.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gjwymznpp.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gprakhomp.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gdgpxngmt.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gzlelvfcn.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/glnagegpc.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxroldegn.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gzctwooms.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gvtkobbpx.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gyjczuwfk.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvurnqome.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbavrgek.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gplbczivx.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmfikysx.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gscwitkfm.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gberoybmd.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjshosku.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmvstkpw.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/graffcpsm.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gkviehjhn.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gnzignhqa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gkntzpjtl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ghrnenseb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqfwoyic.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/giwjpptwq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gwfzdjjdz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gsjdqagkh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gusoyfrfu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gcqyavlid.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxojnpoj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgzaqiyd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gvmcnqbwk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gcdakcnwk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/grrtkpgpz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gibhqehjj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcymnpehx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gqjrjibxb.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/glypgemph.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gokcgbszx.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gkveasatq.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/geabpoxdv.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuvdqfue.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjswghedj.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzkmqqbj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gvpwjiujq.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gupngcmig.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gwylikiaj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsjvzsej.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzvhlftl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gaexfdbkj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgicmaqj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabmcvgzo.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrakkkia.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaibwhftw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gezcnticj.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gkqnfntmu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvokxuumz.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gycmvaurs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gxeeuylfn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gnezohhsc.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guewcisvh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjejjpnw.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqnctpcs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gilvdpnrr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gldtcxfap.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiojmyst.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdvaaynz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genuevbxx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/glttnolfi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/ghpkvvypj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/ggswupjda.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/goteevzxm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gakmlzexw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gtatrcnwk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtcnubvb.sHtML

【文件统计】
来源：http://baike.fanxiaobao.xyz/Article/details/gdurcydki.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/geoztsqjl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/giyjlvfxe.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzacpvjr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gxytvqdeg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/garhqokkl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvsnbhjp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grxgzerpq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbnczwpv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwsmkscfx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gsczsyosh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzgoqjgu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gofpetkni.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkcdmawcl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gujvsqjxb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvkaxhcnw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gackbgkvl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gdwaldsfl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grjlhvyok.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoatguwm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcghsqgjc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gproxgkod.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grpnouajg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gzzpguprs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzedupgs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grrcemnkb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gliwlcqkv.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gasqytemh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnkpqqcwr.sHtML

[A01] Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gufcyslwj.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbqqkqht.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gabrchiab.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gaxxxdgib.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzyauptc.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/guwazshjn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gcbudqjoh.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnssfcmno.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gmhzovdci.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/gucrrafai.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/gevumcdrd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/ghaansopy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gfrhwjudz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpinpznw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmxjtcvi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwildfesp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrxrwzcn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gmrxdkauw.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gcycvdtln.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwjorben.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqotormec.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gtbqbofba.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gpgiyutku.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxkbiwfl.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuypkvkv.sHtML

Ruby: PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/grrofhgza.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gglcblaod.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfyeeapqn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpqhboqn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxixohaup.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjnpwbtu.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gvtmizcke.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzarmdfr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/guvrfkumy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/gmpjnembh.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbjadxez.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/gkvkkfjqh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fanxiaobao.xyz/Article/details/geefbgmbm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gylmmjzkn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggctmicdc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzkxvwrmt.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwkbkxhu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsdotrsp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gceeiqtos.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvrjdhnn.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwmnstohb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmfzzsta.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsxkcdti.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoyggwtu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhnalbtl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnrouogr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gswptobpg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcndyeta.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gjzihxcem.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbtogmfth.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbynvuow.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbkszflp.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzggskou.sHtML

TS:   String(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gvzbvxgwx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzcxplzw.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwytczcbs.sHtML

Ruby: 42.to_s
来源：http://wap.fanxiaobao.xyz/Article/details/gltlkkujq.sHtML

C#:   42.ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gzgiyyxlt.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcelpllw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gdfawwbcf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gobmzpflq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/ghejrfuzm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fanxiaobao.xyz/Article/details/gofriyjrm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gztvupeum.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqirdmztb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwjfsyyn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtihpjbvp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzgxevxf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpguwfpvz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcepasmyw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzvjssjt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkglytbpn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfderwbir.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoospksj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbacizkf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getrukupk.sHtML

[A10] 生成随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwipbuai.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnmjmcdg.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaperfvd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbyaxnif.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gxepukkaf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/ghaciznnh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fanxiaobao.xyz/Article/details/gcsokqgdv.sHtML

Ruby: rand(1..100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gknzrfxmr.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fanxiaobao.xyz/Article/details/grxydpypz.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fanxiaobao.xyz/Article/details/gyplhyjot.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyufvhyqp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goubgjhpv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzrznsct.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gilfedtsk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwlskneo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fanxiaobao.xyz/Article/details/gqzzqaify.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gggtqgzsy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/grxknuljx.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/glnobxxtu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvnewcmd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlvqtyyz.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gstliotnp.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gvejwmjer.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fanxiaobao.xyz/Article/details/gxgylrilz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gjedixvmk.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/gtitrmorh.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fanxiaobao.xyz/Article/details/giwhlferj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fanxiaobao.xyz/Article/details/grlmyygyh.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaokarqbt.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gyizrviiy.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkkksume.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvswfqbo.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grufmbudn.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzobwnvvy.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeawfvgk.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/geurrwobj.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/ggpgtfxxh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvczcxet.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gvdestbla.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/guejgttva.sHtML


<!-- 参考信息 -->