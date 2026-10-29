代发 wailian999

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gkqfbxxui.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gbvifmgaw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gkgvxacos.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/grhkncxle.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gkvjbqnlf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/grawxuefr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gpgkgbkem.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gcefxhkha.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gyzgzkoam.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/ggquhqroe.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gyctkznmi.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gnzdvyfeh.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gcvzfvkcj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gokpnzpqx.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gvoyoybwu.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gmjpopywn.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/govkrixzq.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/glckieivf.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gwtlweiah.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gjpdeezdl.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gouvrnenq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/ghimjijht.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gzhugfjsi.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gfyuioxyx.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/guepxkbiw.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gzeiuoaal.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gvafpskqu.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/givtwkgxf.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gmgxylgwh.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gtmpcvnpb.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gymnixbms.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxtibdakh.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gckhitlya.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gqfcfzfsx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gxnhivntf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gvaofkocl.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gsmtrztgl.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/grlzvuprg.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/ghadneibj.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gcephaidn.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/givnqepac.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gmxsiysqz.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gardbvjke.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gohxuzwka.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/ggzrkbayu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gldxcbmdr.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/grcybnyhc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gsvmenjfe.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gyireonzg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gzgpmaygh.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/goadqfalz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gncsfcnlz.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gevwuatur.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gagbqqesu.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gkbapnncm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gaghtyyyu.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gpdeertys.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/goeimpmfl.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/ggkouuayh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gfuvpltjp.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gvnarqwml.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gxsumdmee.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gjduzmtfv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gqktlkxks.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gsxupdljx.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/glufernyk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gwoutclby.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gygwtasyt.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gswvtrgak.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/geapiojue.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gtjaevmsa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gkpteelgx.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/grnjsmbuq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gfosdxutg.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gihnvhiea.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gmelyerec.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gabyblirt.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gkkwwednm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gcfzojjpx.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gbbvkzryu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfqcjifrp.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gdzbeqyaj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfunexqbw.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gatabwaop.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/ghwtbmlrl.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gudpntaeh.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gqzvytpcw.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/ggtcdjdrf.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gdvkulijx.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gpooopqpv.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gphwadpdy.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gyankpyke.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gxpcrzmzo.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gpuajlsfq.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/grvsjutby.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gijkeabmm.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gqwfzfapz.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gmscbrqgh.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gwzgjjklt.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gfykofecf.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gnvkjeywo.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gsbsyoekb.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gfkncvcvo.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/giyuclnss.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gqqrrwgmk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gkvopirke.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gnmurlsib.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/giymqvhts.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/govhumrro.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/guefvgspa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gvhkiubsq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gtdxituin.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gxsxsrtqa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gqgjhwmza.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gkrcrymqy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gccvtxcue.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gfzuywqcu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gkridjgza.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gclitnozd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gblzzaena.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/glhmpmjha.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gkpqakvhy.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gskjwzonz.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gkzbrkzds.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gywcvwidu.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gnyrmvxyd.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gxmqbzfpv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/giaxqcfyi.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gxdxxflam.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gdhwdpuyb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gqwxnhmgm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gbmaxedsa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gnypwmgzs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gbomcsfyl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gassqrvpb.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/ghjmlyuhh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glqvczdad.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/glgpldayy.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/grijhongw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdagggyzc.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/ghipkyywn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gilrazqej.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gyombuqde.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gfuhidsna.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gazlyfirc.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gzwgosbkb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gpxtgeaml.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gtuenvpur.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gwmnmtsmo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gepgwjctj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gmjqtuyit.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/guunczqrb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gzfhlgofb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gmwgtobsm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gdegwbghb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gdqeoljqz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gwkfzgsqq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gpdyafcwg.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gikasnkzr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/glsyknacm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gnnfvkshp.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gmthjnkod.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/ggijewutd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gemzhtqaz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/glcjscyis.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gcdjigoiw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gzzwrrysd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gdpeselro.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsdumkfuk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/ganztbgci.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gbasylnwf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gpxajrgwo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gnvvjfqov.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmcqgrnsx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gabhxlitd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gufwmfpcm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gchjmbxnn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/glasaempr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gccqcpyvh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gzrjhugeg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gmatiszby.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gblmgryio.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/guyemmlcc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gdaptrazs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqkvdvsvv.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/giqibvsos.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfetbevza.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzzvfenam.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/giesnqpee.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gsfskgcoe.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gbacfpxrn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gknbxjfaz.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gnbobejmt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gdrayttwe.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/grpprsubc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gphnkvqxa.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gozixmrgn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gfqlcyoyg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/govpozdpc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/girjzzxrg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/ghzrjrovw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gtgveizfm.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gsvickypj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gjigktfdg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gvtkjmiqc.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gueunaqex.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gmhskrttu.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzaouqvpn.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnkmmjejq.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gflazxdyj.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtdzxghep.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/ggfahbshq.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gxzcgrmkm.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/grqnivpkk.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gqxswqlui.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/grymuhrvo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/grvzhtayb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/govkhvhfg.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gptqsatsf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gjzmrhell.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gydjqzhuy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gzukjmnvu.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/glagcuudp.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gwuguwidn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gacrczjey.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gfpgmaepc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/ghtjxqgdu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gwcpoyncb.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/ggenzccoz.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjngaeire.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gbfqtcktc.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/ggercqwcj.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gynzhvhix.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gtdmecwng.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gfvjlkgsh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcedplh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gwralmmiu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gzclqovew.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gvwacczru.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gbneajxax.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gfwkoffbo.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gvxdybbqi.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gomodmlko.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gzpkhnsed.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gjflcfehn.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gawqadxhc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gwzkguxmx.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/ghqovjhnj.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gjhlqbnfy.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gyvmyzvtt.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/grdjaftlq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gztupcumc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/grcngpkrx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gfumtdlxm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gnmhmwkby.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/ggpowaprw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gyowcybzz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gxzysefti.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gaklpbagn.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gnhhikffb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/grrlkzvut.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gwgxekwcx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbocfhvlq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gqoclszzi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gcbacxuow.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/glqxcunxo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gtobpjjpa.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gnzdkxebi.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gaeefgtmu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/grrsjqzix.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/ggtdksrat.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gkpqjidia.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gmcyqcqeq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gygmlkvdo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gvnmsqoni.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gbtxtsazp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gajrdacul.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gafuvvgaa.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/glrtmutsx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gvsylwkkl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gjauegpcn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/giwhgfilt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gdslwnxag.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gqzbqemki.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gmryvrogo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gwxwabxkm.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/gphmxmnrq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gwsnbmvgr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gslcqbgig.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gfxqlnske.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gqtixccps.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gtusocrtn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gufwmcimt.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/gmlyhcawj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gjfreqkxg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gkelmceid.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gmsfwavpv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gfevnligu.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gqpvaggau.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/ghsgiddkt.sHtML


<!-- 参考信息 -->