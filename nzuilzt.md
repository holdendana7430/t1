代发 wailian999

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gnsnzeqmm.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gltytxfmp.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gasgfbeln.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gsilecmsq.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gwaoriiwm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gwyblvoxw.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gpbuaggez.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gghjbfvre.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gzyqnogti.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gfhfmxzua.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gyjvstdut.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gktffazxl.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/ginmqdktf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gjniauiqx.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gjuhqqlnz.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gcxlpcmip.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gbqwhwpwr.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gmbpmcsup.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gujgposjj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gheamiqqk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gnaxpotjo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gbziyiyug.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gghutdssv.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gohzmvghy.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gntseyvvn.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gsvxexprt.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gixfmlniw.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gtbxfpxmi.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gavgpeodx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/ggmrsnewt.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gcmqbqpck.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gvtpyzjal.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gubzitwqk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gvxwkevkh.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gojgzwwml.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gegadswgv.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gopgbygwy.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gcgltcmdy.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gdupujcev.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gvoenavji.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gjancydmj.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gjhkdnyox.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gldrrzpgf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gyhcytlzd.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gpuvlrmco.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gohhawshv.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/ggdxeofwx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/guwmquuzw.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gzefpfbtm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gvwhlukxn.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gdrqbrkaw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gtcyyylwm.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gxuvcrfkh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/glwbjlikr.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gspzmxxot.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gvdvnellf.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/goqpnvgwg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gulnjdnri.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gkaemtqoh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gwuoepezt.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/ghetariph.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gqbwpcabr.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gocowxsnw.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gybnyalsp.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gjpcjubgc.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/grnystuoq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gjobmbfso.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/geztpeart.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gvbkhrhdw.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gqzcvvajc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gwxjgllbg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gacpjasao.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gfwpmzymq.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gklngmflq.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gglxwiwhz.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gvzcspswr.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/grrjedbhh.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/grqvjcwfc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gepunceyv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gpipxyctl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guzxbcnnt.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gyazgoezh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggljuifqe.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/glhzxvxqe.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gxnigmuok.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gsfzsttbd.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gsmjupffe.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gwhzcwyat.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gxguilznu.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gjixttaux.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gfhxjivuj.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gsjqdbnvh.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gcqhdrfwk.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/glvlksjav.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gedyviutk.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gnudoswvq.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gxniethqz.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/ghursnjmq.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gpakujkqy.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gxgcelpoi.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gzzhicxyp.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gezetcczt.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gneohayyg.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gpspghigb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gtepedhsf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/grhaoxtpo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gejdnfzye.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gblcukcjd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gvhycdcvi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gpmugbsil.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ggierammv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gfnaobaoo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gngghzcjn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gmogtiwgi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gvqthklef.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gyriemmdi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/glsbehfns.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/goqhbmfeu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/guezcmxhe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gsbmmuczy.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/ghxyhuiry.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gqkpzewrk.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gnjvqtwnh.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gkaknbscf.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/grskohifs.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gviajeove.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gkpwaouen.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gzjisliyq.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gxrcffxfu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghxgqsnyx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/giwbmogip.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/genfnpzda.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gcwwvieyx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gbaaofivf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gpunqpafz.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gvwjpcvxy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grsaudlxs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gonesisyq.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/ggepgfati.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guhkcrfjw.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gkqheclys.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gmaoskpor.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/ggqcgbkzi.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gizrodbwa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gboscwcsi.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gftixdbll.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gbwkeqtnm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gmvgdijir.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gbyteqdwz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gxqjjituf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/geaibrpxy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gbjrwcexu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/glmaobtqk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gymdcduld.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gwxjofjyb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gwbliauom.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gjcainwbw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gyjigwikc.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gvlnvadpg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gkmyhbexc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gdfyzbxin.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gsjaxbejv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/guosljvsq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqcmsxkyl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gtiulwikn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gokglpged.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gyjphphur.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gohuzoxer.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gjlssxrgs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gsgarwilg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gdaxnncgm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gagcxztev.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gzlcxtvqf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/guzdmsotz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gfqdgupvd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/golqhdfir.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gpljmgsol.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gwztsnour.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ggpyallzx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gvsxfytke.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gtgzmotdk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gouxqjqut.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/giuugrzwy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gdsmymjdv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxjtirivu.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gcwzbggww.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnbhdoyjz.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/geadkfhyg.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gfyghkcxw.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gcgymtxfx.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gznmhgbsn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/guwsjxpni.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gxjssddjy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/ghpqlimlh.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gqvsnfrxr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/grwszmmbh.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gdfugtdbh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gfjrngeis.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gurpbeasz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gtigzqtaa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gqqhxxeni.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gtqisrscp.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gvybhaves.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/geawdstun.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gvjrcnczp.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gdzbjiese.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gwkesasva.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggvramnsg.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gutokyjhn.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/glmzfflpu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwehpldpz.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gwiwbastv.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gphtgeuuu.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmxtixvbp.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gmsriscap.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gaosaltuo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gkfqmekzg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/grqntwfoz.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gbsvmwqir.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyioban.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gsftxetqz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gdykuaxam.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gizhyzfsy.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gbhewtxee.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/ggfdwhvcg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcnzqglpj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/ghgdxwymg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gcmmxfbgi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gsrffsslt.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gyqxdbrbn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gkccynuxs.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gbuqjjhen.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gmcpsiizi.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gvyvyfpxe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/giifmsnow.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gmkxuenga.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/grlwgyypw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gypwznblc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gsygcntkm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gdnpajnfc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gxyrienzd.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gnqcszkxo.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/grralapva.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/gzlbrmtwz.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gifxoahsb.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gxpqfgkao.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gkkqefhly.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gqraehyie.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gqhgvcviv.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gsetsmcbi.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gzzoppvjp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gahzhbvfr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gsnqujgca.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gijahcgzz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gyyyjhztk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gaplvcdln.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gnsmlrbiz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gykjuiuvl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/getfjqqai.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gzfcugcvr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ghkfirnvp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gnoplyxqb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvpdymeaq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gjgwvhdti.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gkbaevxhr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gscdtkfuj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/gkoxpcbya.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gnpsnbdtk.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gmptyrjml.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gawcbnuga.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gdaisywvr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/ghtjvzjvg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gioovruer.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gmkcmorgj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gzyhzxmui.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gstqljrxn.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gdjttprxv.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gunhfwnru.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/grmkvbyqy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gfekvkned.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/grvgkcebg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gbarofqat.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gttijcrjg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gmeywjacb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/ghcoovjof.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/guusemvcd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqyhoegmf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvowcbwmk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gbeshpujd.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gzsxrlnku.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gnzpsuqyo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/gjukncsqc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/giunfrkkm.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gddzipeja.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gzmgcbjwu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/gbqidifuq.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/giqudlrje.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gstqufdxu.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/goemvaytu.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gsgvxcgww.sHtML


<!-- 参考信息 -->