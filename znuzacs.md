代发 wailian999

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdsprmpr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqrlodbc.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiazspae.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtmvehnj.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gathhhdmw.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekwhozco.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwzvlfrh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmqcldts.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/guboqikjo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gqdesohtv.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwpkzxhs.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmrxnsuq.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtezlkssx.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcoplyuk.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpccvahn.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfcwdquf.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glldinrlc.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gpxdvuziv.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gacelnrdo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/giobaaztr.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaezkpiad.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbslagazx.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/guovrsoot.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gmizeilzx.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gfubarqoo.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gnngbtsvp.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjigtmgo.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghosvzwms.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldtesowt.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvlctmuj.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/grirffmdf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfooihwls.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/geuymhmfz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxblpldpt.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/glkshbcvh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gsryotjqs.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwpipzws.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzdxaezk.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgwzowi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gebyqlmap.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/guyuqttkc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbjnpsam.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gfktwrdhq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gbarhruiy.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gyetnbmtk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gztndomnh.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqnshkzh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gvvzhltbt.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gskfgmdwn.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gjuddqywv.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gzylorhuc.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gblssswfy.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gldcavgye.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/goeszkgmy.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvodjzyts.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahxfslwx.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/grsyorrdv.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqmfcizt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gceyolbmp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/golqrcmii.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbmredvu.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gcmpouxnb.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gvydirqti.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/givghrzzw.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnxfycin.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gneojlkin.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbuycjbd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvfrgbuf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejddygek.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkmnemyf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghamukuiz.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzimlnlqa.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gmzliqfbw.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/grcaedcxo.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqiflhvb.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gjbsqrbcu.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gojbjbndf.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gaunxvtaa.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmqvhnmk.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqntzsbo.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzauoyzv.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gxbwqfnuu.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbegckfj.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlxrdymm.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghibjnvzu.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gvifbaahp.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjvxqgqa.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiamuyhh.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjhhfjjc.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxunyrqk.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvcecqcd.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqrfonfh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmadslzd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/guuydkkwb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhzvclkj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gnpravxyg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gihaqoroe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gkpuwvijm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/goldsicam.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrvvibxa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gzkqhvrfs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdbavetd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gqsjdtcod.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gyvgbdiif.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtbbsjks.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gruzuloiv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gexbotwmj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxwxbhtb.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvlxujts.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gqwtfcbrn.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gukbdqxha.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gyzhfzoub.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gwasttcgt.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gcbkyrhdp.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/ggssullet.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gmhdclmhq.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyybfahke.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ghpamsbeo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gsvoytamq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhqhpuy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevxyaroi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzggofuo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gvukywpzl.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/gfypktsee.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmkwmwfo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmvrltzv.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gaqfhzyzx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gulrizdzb.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsggitegw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjgbfnqt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gkouritiy.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgtfxaeq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmaixsmm.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqwjradl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzrysroh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkobjdhkj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gftwcezfy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdxrujmu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeonulgq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/gnudezgoa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gjnvynpee.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gqzvwywic.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/geukndckm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcsfhgeb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/getylrzof.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwnwmgut.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gcninwnzu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxihveuo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gwbdbjbxn.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/getjfqlns.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhfsnivh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpedkdtxf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvuavozl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnriryei.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwkhuylj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gghwepjfd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqmxovogj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcielixbb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gorbpfmhj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gexkdordc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupmzeoxz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghkixagsn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwuruaiy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvddpcfe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gimspxzrb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glbzrauqx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnqigjam.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsshjdosy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdaawmpv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdilufhrf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjyewvcq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaigtygio.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaezcvawj.sHtML

A. 基础语法与类型
来源：http://wap.fanxiaobao.xyz/Article/details/gkauxaepd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnomvpujr.sHtML

[A01] Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsuzjhgce.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/geoutkvqa.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fanxiaobao.xyz/Article/details/grglwdffr.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/ghzeowkbf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/ghmvlwvxp.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gsxdbsuct.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsmuivje.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fanxiaobao.xyz/Article/details/gdvsbsnxp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/goyyjwiju.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fanxiaobao.xyz/Article/details/geiyafgri.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fanxiaobao.xyz/Article/details/guqavnhuq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gqkdwqfpb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvkbezuk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmlvhnhd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobycacyt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkesmyue.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwbrgupf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbipyesxv.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/glrbehryi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlxpfosd.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcmmirylo.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gorkcpuli.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsmfdqnp.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gsifaccge.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gbsayjyls.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gghzaykla.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gnnoofbwt.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkoobbuce.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gckvmebar.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyphvgzua.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gedubyogr.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gdequmyql.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fanxiaobao.xyz/Article/details/gggaotlkn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/gvmccagpz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fanxiaobao.xyz/Article/details/gzyfmttlw.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gyhzmqobh.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/guorqstes.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghznnicau.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqreshcl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrbjsjpi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gmihrmawd.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrunddit.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbagzkpl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhkmvkvq.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gaborvamn.sHtML

[A06] 字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdjqcdkd.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/guvxsaywg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gjnmvdozg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gulwhagmh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxoqccnr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbrokvtd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhnhmwrr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gyyhaetaf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gfjltkrlv.sHtML

[A07] 数字转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfugormyg.sHtML

Py:   str(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gdwevdgem.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwdhplps.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gehsseihs.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxbcrskt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvugangp.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoabappg.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqegvnklk.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlyjgwrn.sHtML

[A08] 取整与四舍五入
来源：http://3g.fanxiaobao.xyz/Article/details/gqibehjzr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gujvpjpmd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gehcsibpx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gxozirnvg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxedgjso.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebryjpxs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gqfxgtboe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbwvluqq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gpqlauyyv.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/guxwoloci.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmfoqcjg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhmgrosj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmidayheb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmflywgf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdhyulrx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fanxiaobao.xyz/Article/details/gdzstggrf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/gwnyelfav.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gilklcpgu.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gwzeblavp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fanxiaobao.xyz/Article/details/godfztyit.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fanxiaobao.xyz/Article/details/gpvqqpycm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fanxiaobao.xyz/Article/details/glycndwfv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngipihke.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/geplfjmwi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fanxiaobao.xyz/Article/details/gjzwaplcw.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/gerahryli.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fanxiaobao.xyz/Article/details/gbvaqhrcg.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbtqlqjy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganyvwbem.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfnrfoyn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gqteehyyc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnmazdbk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpcpsxkx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gszntrsqg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/golgcirda.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/geraiaria.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtgllbxi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcbczrmr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/gwnsfjupo.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gwetmuiid.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyjobojc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdzwyjue.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfsfznal.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghniheufz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrvzanom.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhogcbtn.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezalgclz.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkaixxnf.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gezylwjra.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/goygasosc.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gudsuiqab.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gfpjypoti.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gxccvucob.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiljndkq.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gshvfcoya.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifrvwlhy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gzgzjylok.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpvgrsmh.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrbptzpw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fanxiaobao.xyz/Article/details/ghvftcmoa.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjxwskdy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fanxiaobao.xyz/Article/details/gwlzhphrk.sHtML


<!-- 参考信息 -->