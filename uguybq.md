代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vmbbddty.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hbftebwd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2oymogdfh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fzungtoi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jigddhxn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2imstwqvx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2yasaxzcx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kluppmjm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ugvkojau.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nxtncliz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ampzhrky.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2besmmman.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jqpcryri.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qixwdted.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pacftndh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jbhrzyhi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2txwsixac.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2bvdotzfp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jwbxvymc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hxznnaov.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lfadifje.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2hfmudyby.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pfzbbjoj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yfhrhsjy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2pcxelrcm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vynemuym.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2scgcwdqe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbiopbw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2aoogqadc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2roqhvfcs.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xihluien.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2tmoprxwd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yrecpzbm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tgavvlzv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rsyvpbxg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2whvxggcp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hgtbsnay.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hsfsirfx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tlgftgyo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zjhzzrbk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wcbmyunm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pixeaxwf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2frgoygbp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ustjmbjj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2osvzykkv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gvmjbjhf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2awfghkzd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wedcqcmz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ahwmuikx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ajvnraoy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fjevplhq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yympkixv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bbekswzk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2prcztosj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mhrtyxeh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2darydqqf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ctptyanv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2crnruebr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2uufrnsnn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vxyqhnkm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vstadwuj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eciqwzam.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xyzuxvbj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lrkizfmi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fhckdtvi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ctfrvjoi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lgnmhmgp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhilufwc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dufcphbi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pvmamzyt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hkjrrrzl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zanwmust.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ihtlodrw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rxsnbkia.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ampuvnsk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zebzhpgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cesfflre.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kmxvdcvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hprllyoz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2bhkgepwt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2olzctkrv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2unagivnx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sywhqzje.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lpdcixdq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nrwlpinv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bmotetru.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jsvuvaoj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sijzdfev.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ncsvneqb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hkmwzasg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2iqhsgpfd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2tjutsacv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2agqfirgj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xhtmdmjo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ujlwnpxf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zwdtruff.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ljtjpjtq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dzicplre.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ugctsuhf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gxgfqnrv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2juzydzbo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yvdyjovh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uasuouqf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lndmnexp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2eatmywue.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lwpkwbli.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vramgmfu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xfvwwhyh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2djpqavma.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jsqnnxad.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uwznwuax.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2utgbpoag.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yukubqwg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gdzfcstt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bfjoxgun.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bzwwtgca.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2eumzglbm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rgyjxdoh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vzzkwvqa.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wrplhiyr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bjgcjhjb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2opfzeziv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nuvhrwpj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fwdlbols.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2cxbizwkl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fjekckkd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2bjuephpb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fjfawnkw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2wuyhqesr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2gbgvddku.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2txzlpthz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2prnwozte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkdhdzra.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rnvxywoe.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2zvpiphns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spjglxkx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2pvqykzjb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wghiqoqh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qmxbyjav.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2qimodqsq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2utchpaqy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vtlfpnpn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2htcotqtz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2xtjxaste.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2urpgrifu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2gzqqhuzh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mmfkjgmj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2cvulkiad.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2qgmxtaja.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2deibjmta.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2fobegfyk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2apktvqeb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2fpyyshfj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2dnbuqntf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ewocfnlk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2chyzzgon.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zgymuswy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2isbqleza.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rmrckcsj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gmxlhtjv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bhndijfg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nfepchnz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2iviqunaw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bosyyxwc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fglhstep.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aezfphaq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oerigxpp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tvjurxcd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dxmbscpk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gkrxzoyt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fqmfncsk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yerjyoyp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jgxweurz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xmwvyrly.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kgqbxsxk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fblbwmvi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pswtfutd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2idowuqte.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qdljlofr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vqtytlcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kulgkkig.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pgocebit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbojvviu.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ekmrnmig.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nhrxipco.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2gmurxyyu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bvidrule.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2obcpgipu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yqbebaqj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gfejnksv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qfuylkox.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jmxhdmtj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ulitacgo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2caazxdot.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bivbdisq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ecwqgxoq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2kfvlobvz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wmdsuwnk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ubildahm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2zgfmaoqp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tcfwujrp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2kvoehfib.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ldcwpzvt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lfptqzbk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2plvkwnxw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ntoldfiz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uujhydqv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2owtjbkmu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ztotjhvf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uffisyuz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhunmgds.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zcexsxfl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2wzngvkqz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2weyigalu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wqwdaahq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ynfxgkkn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ettqvkic.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2nhvrsmtf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hjvfydqa.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aqjtnizg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxqxggrz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ycjmlakg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ppwiwzvk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mofzsvmc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dbigrjdc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dzaqllcw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rvibwexg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qxapaxyd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hnxiuvjx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pnggjrti.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2eyuuuhnu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bzxwsdxj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2yehtxdyx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2umvosuzg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cqarodba.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2cezrswpy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dlveenov.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2gtcwrvit.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfpffyc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lbvsflep.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hqspevwe.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxqhtyr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2cbqxjcfu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hppcrzdj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2hzquydwq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2wqpcgeih.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2aavppadv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xnirlagm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2rycgajjv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ijgxjdfa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2hxklywsh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2djswptyr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bgabcwcn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2jqlgufyl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xgtuvaht.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qschyejb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2agqgrxwd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2folkpmjn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yophbjdk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsycxemc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jbhejbsm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hjlggqnr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2xetjlbox.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vrrukkvy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xscgailw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xhxfnmbh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qazmwjhf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqcbotxj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oiclwasj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cdioyzye.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2hcziryyc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2yimkmobm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2yghyjckr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ojvsfmdw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dxrzqkgn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hxqxoill.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2thmfbpzb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lmcoxppz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ejkonopd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jdyyaokr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wwfsqtre.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uxmrkinb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uowipisu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2myeoffwr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2tpcixsfu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lsngsaga.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dvindvea.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvucqcn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hbbgitpt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rlzzdjuc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hqvrjcpk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dervvaam.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tewnelke.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mdzeitdj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2guupcahf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uyvsxjaq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qdjfsiwx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ptdvhydl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wedafldg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2swzyznyl.html


<!-- 参考信息 -->