代发 wailian999

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gjsnmpwhw.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gvxhufdpy.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gznklqunc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghknzmfzl.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gkxeflkdx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gzxjhwjye.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gzrjusnvt.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gijqkyhea.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/getodumpn.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gwufiipbh.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gljqduxex.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gwuwaykfx.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gvgtlgmme.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gzlrvcdla.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gpstkydak.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gydnmmcws.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gerxvdyap.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gfshspwox.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gzrflhmsr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gztzlotst.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gqwqarvky.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/glzbapehi.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjsqrgxpi.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gbxaxgtit.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gndunrgbf.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gyvjbtubm.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gfafneuhq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gyypfayau.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gznargvea.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gbygclbld.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gathlqgtt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ggwanpfer.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/glkffephj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/grqycpquq.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfqnmfzpt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/guwxgamlx.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gsdwdplrg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gbgdvqdmk.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gjgcnarzz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gsjlzbpco.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gldgzimvi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/ghfkfvpnz.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gggqjoqnu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/glpuevikt.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gfbcecmpt.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gufsvidya.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gfrdbgach.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gphbyardh.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gaqcwcamt.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpubnnjoa.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gclliwwce.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gfdawjezr.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/guhxdpfwd.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdpivmrgv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gxkiwljyd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/ghzddnrjf.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/guxgvbwhn.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gbkygkbyo.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gqdbwqsfb.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/ghvmdylzx.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/ggzfajcjv.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gehhemlcs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gwqkewgie.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gwwvyykkx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glbpjgiij.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gfoevnqtl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcfligqbb.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gglvefgmh.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gigmhpkbd.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gwluqrdub.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gtwhjepqw.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/glcggckiv.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gpabbqwyc.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gyfxsxltr.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gndhtlhde.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gchhyqdey.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/glpyvfgmo.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gbphbucxo.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gajyafvvr.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gtzzrneer.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gnkvuidgl.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gfnylzzgr.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/ghxfgnpvs.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gxsgjslui.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gygmuzayj.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gytokmbdf.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gpzvjvfaj.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gmpahcwnh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/ggqsqaddo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gjoqzmcir.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/grlpqxwjp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gpdujxama.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gaxaozypi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gfpfubatk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gzvirzfqa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gvkfpgrtt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gvnwsnoee.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gbxlwippj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gojwxxzbc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gsznzpdik.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmxbviknl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gpizvyror.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gzogurqcz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gcqrukpvu.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gbaxsvxxk.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/grgjmsypb.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/grgddcdau.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gjahsofpr.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gvpgpbhan.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gwrtjiwzf.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gtswdanlk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gelqidpgz.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gidiurxrl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gmrbsopvf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gzpczwuvg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gbwpriibp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gcqkzgffu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gngaudnul.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gsneplfou.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gjrlzgjrt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grsgdenyr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gkxjlcmiz.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/graclhgdz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcierltkt.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/ghtmqkhty.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gzkesuwln.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gzgyertxi.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gbcsxzqtp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gtchctrot.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/ggevupooj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/glmqpnriz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gylemnvcf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gfthlaatg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gpingjpzn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gtxanockk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gpodllqky.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gzhhmrefx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/grrhezaaz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gfripskno.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gfpmalrds.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gvzmusyfl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gznszvinc.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gqfzqcnmb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gxeeudswc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gkwwuqehs.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/grknahgem.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gxdomemdn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/ggcjarlyt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/ggzdsbour.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/goetbqhmv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gqneccgbi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gyhpjmszw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gdhbnogvd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gsemwgfsz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gusqjvcqt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gmunbggxe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gtecpadwz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gjsnkfhnx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gtckahcct.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gxbpctdev.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gofdgxbjg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gzjfovsfd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gicyqyacq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/goaferegz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gqgzveerb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gmssxvjyj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gbcyyiqwq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gpqpaqasu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giopxxyml.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/godcopywa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyyletidp.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/ghrrttuvk.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gblkonssq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/ghcxagsge.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gmjwcdokn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gibzwaqzm.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gpchjzqdn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gjzncarvb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/glbkkdpxf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gsbgcjlhm.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gminvykhb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gbtdyrjnr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gsleugqqr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gfaunmjbo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gqsktfues.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gwgentfkk.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gceujpmsx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gbqtgxtob.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/ghvstilaw.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gpfivvrte.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gkjzxrcfe.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gorwdpsjc.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpqnxuxik.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gfwicuibf.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/glakopxto.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/ghynbynmp.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/glioyudal.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/geusijtyk.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/glbepsfvf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gnrdsxexy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/guajzcufj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gdueptloh.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gmzfcovwc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/ghrzclcul.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gecedlmvj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gzcigvdvr.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gfjfkdejz.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gkcvipzhz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gmhtoqywq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gewsudtzo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gbmleuszf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gunpuqufy.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gnnovwdnu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gowsmgyqr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gsyleabdh.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/glrsvafpw.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gbwfeyisv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gzgqkgmjn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gwduxrdxw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gncriawru.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gfscrpbtn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gqggbepsr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gyralsbmb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/grageiald.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gkoryaydy.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gnyywtkfj.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gucqqfibx.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gdylrdmgp.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/giemmfiyt.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gqohthmoh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gqebhdxlk.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gntvzmbix.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/guqdoxket.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gusubotlj.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gfpyepubi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/ggrskgjok.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gcmrimmit.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gnbwrtlxx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gmbvhqdmm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gqstuybbw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/ggwgyjklw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gabbxucyj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gbaegqycb.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gsnyepajn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ghctewtnx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/glactfguk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghupzikjb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gliiuzefl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gcegnvadg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gkzrjvepv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gaifqowic.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnoejxdjd.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/ginygvwwk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/gtxdnmsxy.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gykoxiccz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gmajqsibj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gmymokwxi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/grergeaux.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fehbvm.com/Article/details/gngaibfwq.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gezhpdhsv.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gvoaxvfta.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gbsipwyyn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/gpxatmooq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/grbqpyjyv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gaeqhotfp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gdezabwdj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gbscmmzxc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/goslzmjne.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gafeokstp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gyaxpkltj.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gqpvjctal.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fehbvm.com/Article/details/guctmuarn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/giqmvkcwl.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gmloxqqan.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gxmszsscn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.zdbjq.cn/Article/details/giudxhpep.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/govhnpjtr.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gazcuqsjo.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gpssfmtjk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/guzxpeezp.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ggjlcrgec.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gbpbvfkjt.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gbohhemrc.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gstusvdml.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/giwpbtwlz.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gpprqifnb.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gskyogxdd.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gaiourysp.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gwdxmuicf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gjtykgcqc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gbfbffihi.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gnfdhdfdv.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gwuautgiu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gwnewjdmm.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gemwzkgee.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gcmxafrmf.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gsfmltnqu.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gtdspfkxy.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gezwjvnqv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gqhpyslkh.sHtML


<!-- 参考信息 -->