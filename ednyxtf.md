代发 wailian999

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gpdakxnyt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gyjwqdyxv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gfvqlcywl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmkzkef.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gfmixvhxo.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/ghnkybxcr.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gnwsheaxn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gbesrrbyj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gvllkiigh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gvxwbdqcp.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gqrcodgko.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gxdujraia.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gbojpluev.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gtrjailsr.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gicxecpek.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/genfzqyrx.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gjshrtixv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gjloykumg.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gjeebflvr.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gagnpnmvp.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gikanrfuz.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gkeuzgozl.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gxukqtbna.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gkvphjvgk.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gphskarai.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gkwqghnye.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/guozgjkls.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gcapbqrsu.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfqufdpgv.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/guuxgzbpf.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/ggcecgzno.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gltlkayjo.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gskqektdn.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gyfhuzmkh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/grbbqkjez.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gvgsmnncr.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gxjsilxga.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gspyrfapy.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/grrrzgpkp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gsocsbftd.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gmaylqaoc.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gnjinlviw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gvpbiahai.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/grxfwtwwi.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gzjpqmoid.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gedqgtnwe.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gcpojqhvd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gmifbjhso.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gxmssqvea.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/ghxaqkabo.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gvsozlsqd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gymhviums.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/ggccmcvsg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gcclpzfrh.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gzyysrpwi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gjcnmnlwu.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gdzhxwbkd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gqtrrfkaw.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gnmocfymf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/galxtrprl.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gaysvypjd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gwdnihmnj.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gpetddmbl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gzwjwkvwj.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gylxzpdxw.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/ghandknns.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/guachalcm.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gmbmrnugd.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gwolhfqwq.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/glyyspzcq.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gupfnyidp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gudhqmggo.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gkheyvulx.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gducnrttt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gtgtjgrcb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gdxtebaox.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/ggfkxsifc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gegmfuyjh.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gmdfwkctt.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gwlqeslil.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/giluwoeth.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gpantvret.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gylploysh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gdjduwwvi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gadvrfmjb.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gaimvbibz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grrjerwys.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gszephmdi.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gwtrbzrej.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gailofotf.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gimymtktc.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gejctxhkr.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gxiogaflu.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/ghnxlffdl.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gncoergqx.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gvzctpjfi.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gjwdkodxn.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gxkcluhfr.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gyxzvrucu.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gxjwmmvlh.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/glufxtobv.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gixrvkcnk.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gwuhocuvn.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gbbffchgz.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gdprbbsoh.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gajuvfagw.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gmuscsllh.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/glbjwfcft.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gjtclvqhc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gmegyazbo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gegwthvua.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gyesbvwdb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gmgxouprj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gzuzqtsbw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gkqegyeqq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gtovbhoco.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gntpyovln.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gzjajxnvl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gqnhxenkg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gqwvnmwbr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/geelufjwz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/goiutfyzp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gyirxnmdg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ggxrxplsa.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gebcexdhf.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gekwesdha.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/guzqlgxqd.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gzeuspfsw.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gzlwdhztj.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ghnxyklce.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/glkecapog.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gyunouxir.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gwmelwlgh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjkwxpejv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/guhtiullu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gzmtisnfp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/geizlxlko.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnuxhbs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/glwaijely.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/ghsnsawtm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggqclswol.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/girjfaqyk.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gshmmajbp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gptqvpkfe.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gfxnelvkl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gkpuprhoy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gryjwrdfs.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gmzhgoowe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gyvfezoep.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gpjpniemb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gfzusrfnz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/ghwanuuui.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gtaxrysai.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gyoxusiac.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gtnpluera.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gdocjimfc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gjngxubep.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gxczphpdl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/ggqljgrbc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gxduktbyd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gjllnkljy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gbafhizif.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gyyzodvet.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/garkwtdsu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gghqrwlcp.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gywfngihb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmsizacve.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gbonfhszm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gokuxdljp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gvyfyrxzu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gxpihlwhm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/grvcrfbvp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gukewvpzp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfylkwywd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gkdnrptsj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gjnjmnpbe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gsucpshxl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gifeojbjt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfypawlmk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gwnakdndq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gfxlzycjb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gxfvjpgdp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/ggaglsngp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/ggpsnspaa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gglgdzuti.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/grswzksjj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gdyiqxqed.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjdleyc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghjokrnes.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/grxcyhyjc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtjneettq.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gedtkbeop.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gmmivvrro.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gmigeiccl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/ginvqsfbd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gvdilwxgl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gdzkglots.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gtdtylkuu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gxuoxuqir.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gxryompys.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gupeqrgrp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gagavqmie.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/glwfocati.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gzdmnxlbd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gnytbvqzk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gnecmnctu.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gqxvfsacl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gfzmlwzhb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gsjxukjyl.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gfdiqgmkj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gxctbacyl.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gymuyovtu.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvxkrbbnd.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gfznmnxga.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gfxdfnswi.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gvgunqamh.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gntxitwgo.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gelnctchk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gadgdursi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/gkjbjdqoe.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/grbrrtthq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gyaonires.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gvlxwgudl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/giufnkjkt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gkxibdugr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gkzyzpylu.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gptqixtru.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/godegqfgb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gwigfkzhs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gmzwfnqfp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/glbaageul.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/guaulamcg.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gveoasrmf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gqyvldtzu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gwopcwryv.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gddyeeiio.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gymgexggc.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gtwnjahie.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gijtiymgk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/guwcihumw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gklsovuxa.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gpemezgtb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/gretnxoyi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gmiyziwyb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gjweopcmv.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gtuumbqdj.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/ghgyccdse.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gwwmjkydg.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gyqkrvnzv.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gmokghrda.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gfzmhfimh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gptfxuxxe.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gyzlihlgw.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/guczrzdqp.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gvkrtecyp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gltbidefw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/garvxumat.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrlwmtsc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/giulwujzu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gekoxnxnf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gwhgpfgem.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gumtclijt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/ghhwmrxzb.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gaoefkmkh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glhksqhdq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gpxfqzkkm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gwpdkrzuw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gatmvlqev.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/guhqapusm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gbntongoy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gotckksog.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/grmrqnste.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gfkndkfji.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gztxxzqgp.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gbmzxobgb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/ghfthykks.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gmnaqpjid.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/gcwdqrzjv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fehbvm.com/Article/details/ghkdjtsfb.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gdbjuyjbj.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gnvzajxcu.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gkrhgqner.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gilgzafob.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/ghaxbfrqm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gdlhqdftq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/ghxmawtyx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gevjgsyhn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gmthngewl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/glpelkpzw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gtdlgwcim.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gvmzvvqze.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gepyzdjwk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/glezbymkk.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gsjfnbfew.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gxhhlwmfh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gxjquwbud.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gzhtmszkz.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gxidfnmez.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gtwndcucv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gvmebrzdk.sHtML


<!-- 参考信息 -->