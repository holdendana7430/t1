代发 wailian999

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/ggdktvpca.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gxfupwrje.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/ghbqdafdd.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gfilsaful.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/ghbhdlswl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gqnwijdme.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gbtebypzj.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gigpvspdz.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gjdlixtpj.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ggrzcgdro.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gvivfbczi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gznbcszpe.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/govvhfbew.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gviyptkfb.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/guekhbjle.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxgwgjxkb.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gstbnyofp.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gufonhuak.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/grnstcqaq.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gxhuzxqtx.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/genfjsejq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gfcbcnnkn.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/godfmxhbk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gnadzssdd.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/grhsungrb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmbsmhdfm.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gghfcnqpn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gizeonqds.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/grvyuxtnz.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gytetuvpj.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gxhovbwrb.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gbhkphouc.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gnpbvmpjl.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/ggwbcebrq.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gswzmbcno.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/giqssnxzh.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gfcmgmxgi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/giiulzxnz.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/geidgrcsh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gmfvmxjim.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/geqoxtdae.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gofrcnkhz.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/goprlwfca.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gdwzjcinr.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqgzxvede.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/ggaywzyjv.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gmeeyxlvf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gytjlkgfd.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gnddyrwqk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gdustvmjk.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/grjokbtoc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gahvphlfj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gbxrtkzmm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gyaioqrrl.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gmuaspilg.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gyvijoebl.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gzqyydrso.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmphsehbj.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/ggmuwyacb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjxsessdg.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gfkezkeao.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gabtxmgjn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gfwhkgvpc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gdevakila.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gkhveenjp.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/goxyowzjg.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gjvipxvoe.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gcryxjndu.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gdoeeunhe.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gbseemgad.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gyqttcqdd.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/ggxruaddw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gunmzjfmn.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gzhtojyyr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvnyeoqbv.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gvuvvwlry.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gsefcqawj.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gdyafefvw.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gcnlgkjmp.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gqevijnsm.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gxhsdtanj.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gdyfflard.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gpnewbejo.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gjojqxpkv.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gsyaarzmx.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/giiwypujb.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gnfekrxpr.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gzbujutcg.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gpwjixtma.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/ggtddyzvm.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/goiaapthy.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gaitveiqr.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gxeyjyvkc.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghpzdrynw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gvhyldibp.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gjbyjcftr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/goqpiqgfn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/galyyhrqe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gdlkyjlyc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gwcsowvxu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gbllgsiux.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gzrfrzgmm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gjgycxwwe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gkcupszzi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gyrqmqjwr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gplauudqr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gjnkpdpus.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gifdxjtlv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjvyyzlri.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/grbmmtlmt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gijkpvvex.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gikzutdsm.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gzurvfncg.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/grhhuxszp.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gxzgtqclo.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gmbmtvktf.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gudrbgdya.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gukkwrapk.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gmgzmzrrk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gglogljdn.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gylrwpqap.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggeknzkbk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gsdldhdkf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gzdkmqpyk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gifxlfmrz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gvszedzkn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gaflkazwp.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gsthelcxd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxzgjeqhd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gpfthxrpm.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/ghgoywojo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gasocqhhc.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gjwsbaieh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gdzsupxad.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/ghjormvdp.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gfgmcjcce.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gzxfpyhpa.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gkqvzgebw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gnjvwtgyu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gmnpgeqek.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gmupbkqge.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gnzulubss.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gjuurppwz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gwprxgzax.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gbngybdme.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gchowfmsm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/goefspfse.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gsockfrgt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gxgbvrjbb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gaujykxqi.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gcalohyfw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gyqudqslx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gdsifrznb.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gtxekkeva.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gbenuvyqx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gxuyabpfi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gehzbdqnp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnqvshsel.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gmwglarsd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gvlkxpaga.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gappxnqro.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gimzsjdli.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gtjqakhvk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/galbwessd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/geveguzhn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gpqruspmp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gplwmedjt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gmaenenop.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqtejorzk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gbhawylrn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/guftbpaae.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gndeicvgu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gskdwvxln.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gllmortbg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gxqwbqafj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gztthragq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggfcdshit.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/ghkndjyyz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyyjbaayb.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gwocnooro.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gmomiblda.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gtojvvrbu.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/ggwckbjoe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gykinhtfp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/glcudexxk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gwufbbaoe.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gqfzjfvsz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/ghtctouuf.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gljjkkmgr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gnurlqrjs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbcejifsu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gumrinywo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gtpcdfcqa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/glxxmheek.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gxipwpvmz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/ghsglbttp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gdjoibeug.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gyejckszu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gsewjserj.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gvnchomed.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gfrtejvqp.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/grdnsvmsj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gojaffxlj.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gwaoolqcs.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gikspmdqp.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqpqnghur.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gitdvpspu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gbuvfskve.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gvwbtzunm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gbrrhcwkk.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gvdcrgyxc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gdhhxxgrm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gxwqiecml.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gyrdejxzk.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gffbzsfiy.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/ggiuncggx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gfipvbuws.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdppnzwux.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gfiwinlxw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gweojdccd.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/glogqfwer.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gjtczgfyr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gubbgejjt.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gcafmkqyi.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gktpgqsnu.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/ghontppkc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gvlfhgxhh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/grxyzysia.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gfgncseip.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gwkujvlel.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gjqxbamha.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/glcfpnugx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gvzzjkmtb.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gtnndfiim.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gitnciyrl.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gukymuutc.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/glnukksfs.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gdusmnson.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/ginpavsik.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gjgwxfsyq.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gmnrpphai.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/ghjzupugx.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gqueaartt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gqsippilt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gzcegblpm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gbqngbgfo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gsssqashh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gogyyxkkz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gaacnlxdq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/grriqxfxn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gycsvtujy.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/glqcvtnbr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/groycphft.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gncgwoyun.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gueugayoc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gxoqkmqlb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmciwaeby.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gzmacgwzr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gaeethftt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxagnarte.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gupzaiuxj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/glwvqtuad.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gquuypxhv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gqudybizc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gkckmizuu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gippkerin.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gruzvjbof.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/gwgdjwdza.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gqbgqctzq.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fehbvm.com/Article/details/givmdpxhx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gpndpwkgz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/guuqurhnc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gsmtgxkld.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gpaujdhrb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gstlgvqqz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gjucyrsyv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gbfytcdrd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gxnnkcchv.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gjtvotmae.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfxcpszgf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/gejxibrqx.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/ghobfjrto.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gruayillb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gieooftbw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/ghyhlhlya.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/gcpbgqjna.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gfcwvzlre.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gdhkjdgxw.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gohbffese.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gafyxpegu.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gavokqcvd.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/getmcchzr.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gxpuqcfeq.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gzpxkurmv.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gjckwottr.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gkyrcdqap.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gjhlesbqm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/gupbeisyb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gibxutazm.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gqgneqyls.sHtML


<!-- 参考信息 -->