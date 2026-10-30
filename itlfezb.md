代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gmlcqazht.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gwrvqlsid.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/grzfggltt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gbtyfinjn.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/ghjidltqd.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gntvefbkh.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/garfkorfx.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gracxqokj.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gdvatyjns.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/ggxzqvqdj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/goswkthtu.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gxdxcqwxx.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gdpouvzwu.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gmpalrwut.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gduvwduba.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gruuhraro.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gmcwuuzsw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gocbumscx.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqwcvjufw.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gpncguruv.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gcxeqapri.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gsokretrn.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gqyqmayjb.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gxfzxiyeb.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/geymeljno.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gsxkrofwu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gjrxrkdhu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gcbdsagdg.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gnbgunggf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/grwxuvmjr.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gejdkfpvi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gksnkundg.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gwqfhbvud.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gxhybvmmm.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gpiufctfa.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gqsygqgtq.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/giznaxznn.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/grivxrzes.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gkfbhokwa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gzikkxkgu.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gjfnjytdr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/ggcqkbbfy.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gsadgergf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gkmvnbhni.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/goqpfeosn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gdafdizgl.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdnelnwkj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gvqqeyemf.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gotqhywkc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gwlxzbrgx.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gxpkrmovd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gxuatawsi.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gqdmnuote.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/ghoiotfie.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gxukxefyl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gcqzzcsqc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gxllhiahl.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/ggxyblcws.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/grjbzybek.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/guzfcwjlp.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gncdwfdoa.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guxzxdxaj.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gwwzsqddn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gikpgwuui.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/grydfrzjv.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gzpdddjcd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gcmimmxbu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpceqpkhz.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gvumbulyv.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gpnvrinba.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gtuhubjwk.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/ghlocypka.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gcqiagwkm.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/glsifwyvl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/givcvwxbh.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gbiumhakp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyeomqljc.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gfbjcrxmv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gncgjolgq.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/grjyfpmnr.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gxkbedgyb.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gypddcueq.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/grzkwhjdh.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/ggzqeifci.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gpiloaguf.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gdhucleqm.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gynpwqtmk.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gezperbzz.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gitassihl.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gwbqrmorv.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gvaosveiz.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gveterlqb.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gjqkgpbqx.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gouvsaaio.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gndtgmjsk.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gzznosydx.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/grptailfb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gwftbvdwu.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gdktvxexd.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gmqyrdawt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/ggesbyudk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gbbtxeoar.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gcpjuaxax.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gkedlxtdo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/grsmagsof.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/guhxlggbd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gfypspdar.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gwcpzigei.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gnkrzitvp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gloktujtb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gqgrzyydz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gxqqcbzlg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gcmhctubz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gfzuntuwp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gqtmxxvac.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ghncouhny.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gzsunvzne.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gjtatgwjr.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gsonzzacu.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/glxgwllka.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gruidfvwy.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gnafgdahv.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gyjixtlqd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gxxdoiyts.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gucoeizqb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzctywoir.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gafkqtywt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gacnllnah.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gbzndqgev.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gxcetjoma.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/ggnzeqawc.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gxauewmce.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gswgbvkvi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/getldfnle.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gsyjajmve.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gimksruqj.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gqlmacewx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gytelodni.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gdgdxruxh.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gxtdcdouf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gnqmtcetz.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gsfvwszct.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gfxoyphxt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gmyhojnfc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gkfloxocu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gkqvimwlh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gushhncse.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/guedcbjof.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gbpcfswlq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gogcuuhou.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/ggnsnxexq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gfldtjuth.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gvgyuqeqy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gxcpjksau.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/goljesmzs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gklzbctwy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gmyreqpkb.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gcxnkrihd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gctyrumrj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gyiupqcip.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gcwzwenjz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gaeylapeu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gqpedgnbz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gqixmytkw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gyzgirwtc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gjoiqzbwg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gmxojaiqo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gmwanrkyb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/guxnmjzok.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glsyashoy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ggitsttan.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/guqkzwkuu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpavebxeo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gyxoaboyg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gscarmlyj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gdyoeaynu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gcyuwpxuz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvghvcxta.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gnzlmjnma.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gncfaosdu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqkiahznl.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gtprzuoxj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjpqiibdr.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/grrrumhjv.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/guixydlak.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gcucxjpda.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gijzdgffs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/ggaybxnhf.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gcyhdvxxn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gehxqcula.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gswwixfbk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gwwgvqaja.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gnvwluhmp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gxteegfvh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gemxaguzb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/ghaisuann.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gnhoqywgo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gcsgnsafg.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/giekghdbn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gsorfwmrn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gurlwhsph.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gycxukgrf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/goptafadh.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwtoodrsa.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/govicrung.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ggpglgscq.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gqmmdtrvl.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gwevhqlml.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/grkiwzocn.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxvbnlhuj.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gnyxycqzs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gwkdrblwe.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gqghdqafs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gmgbwdblb.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gvltezkmm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gxrjzpobh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/guefskloi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/glyhbeqys.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gwdkjcgul.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gqkjlrldf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gqngyoknv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gjsweoglv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ghotgorzh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gyzymkscd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gopwqevjn.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gvfolcdhr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gcskkgyzr.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gaiohxwil.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/grgmkeulq.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gknecgcgx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gcoywqfqn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gqlucjxnn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gszpsvjbl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gqbcgvshp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gpkxikibz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gbffsiyuz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gazgpbjmy.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gompreyry.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gpgostnxu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gzparspgt.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gfyljldzt.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gldinltuc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gyasbxlvz.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gpnqlqjrv.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gmjgmvrwd.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gghyxrkyj.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gkvxzpmbn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gawetnlaq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/gftzwetux.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/glctmtusy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gjhpzvvtr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gzwapmxkt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gvlnvxbsn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gqdywihbz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gtdlbkybi.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gsreykwkh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/guvawmuhv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gznnatoum.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gkhbifczi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gdzrrmzwf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlgwgwcm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gkmkihkga.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/gueneujrg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gftgyejaa.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gbmxymgyk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/goqapbifz.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gzabjppwu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gnwlkggpq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/goqyxpaei.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gpfiepqvy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gswpvpqtr.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gpkbvodcn.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/glsnirobm.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fehbvm.com/Article/details/gtkspphxp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/ghlfbiktl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gnahmimxy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/ggswsdzoo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gbntbqhpx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gcxbedxpb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/glwpzgfyn.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gkrzgvoyr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gwvvwvify.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gucelkret.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gjgnrmano.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.zdbjq.cn/Article/details/giiubjlui.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gphmerusr.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gutwvekmv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/gvgbjmgot.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjikvema.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gmqpfuqly.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gioeppjyr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gvbtdukwe.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gcxsvviuz.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gehpngjyx.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gtfgrdqlo.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gnmloabtz.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gwgtfmstz.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gtnjvsvgw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gjlwatxjv.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gadkcaxeu.sHtML


<!-- 参考信息 -->