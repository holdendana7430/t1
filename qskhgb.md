代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2szwrkcgs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pmyiwvre.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fxbqnwrx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ywasgpdf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tgcyavsv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wlvylkek.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wccbdsdc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2wjcppptr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2udayznbf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fvneadce.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jgmxijgl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jwqzlyfu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2obudxzgi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rkptoooz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pwsfftfh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ojtctzzx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xonyowht.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fwysfxnk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lujxqede.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcarlceg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lsdehrpo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2lymgsrpa.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vsqsilsl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bjunlajw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kvqfozhx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2oufmetrj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dqlctpwr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ssaayext.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2bvwupese.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2altxuvkf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2foysnoku.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bubkrffi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2aytzonxl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ysrznzgo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pbmpjgaq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mgbybeft.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2shwagbmi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yuuasahs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jcxfniyt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gbkalyax.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2npwfmcqi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lrmuxlxh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uzbdjeqz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rwbgxeyh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jwbgoswa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ucmksqkh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2beeeyqst.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vjlltwjv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lyjlpkjz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vscddwjj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2spalhlpc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2oierknwa.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hgglyoqc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eyaahsdc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2azujqufh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2duzcyskg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2trjgbgdl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2exngxetl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wmymnliy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tdeglayz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2oifktxxj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xehvlkks.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hqieqchw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jgknyuxm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xvonzdwd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xjlovzbq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2swnwgmar.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2omjrjytg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2luykpvoy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kgcxcipu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zfoynubk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwpnmjau.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2biqigvzd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ebzynupy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2medbtine.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xvyohmdk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pzkzyzhf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rwiwjrzd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2oeglatgj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2svbpatwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uoslakfd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2pphjzqrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfxyllzs.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2oakwjebw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mhyqexaw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2bvjomdfu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2lfoeoapk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ymrodljx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nfpqnleb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2slyklmbo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dczefrny.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2iolchbmu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qparitdp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rczfwixn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ouwtpfnu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2esfokqjz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jamtvscb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sxfptegp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2bxtagpvp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2fcedmiek.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vrlchpgk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gizpjttl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ucgtdfpp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2uabflpdn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2txieqqhi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tcwfkkkw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bgluzkvj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2idkjezmy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2kzekqvcc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ktwvtjbm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ygbxcaab.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rssuaery.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jbhxljbs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wgcbvtjm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ghmdxrsa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2motbxvoj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lfwneqcb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xcqkmduu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rvshontw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2npiiveaa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2nmyniqsj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2haupmrjl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hesswrpz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2tgimjhyf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2uajxlict.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zjkmwhih.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tnnzptts.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2muftzhup.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2nnencwpl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2btofwgzj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2evquypfb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hfjqqexq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2jwrjonzl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2tiauofhb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2zpxkgoof.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2okvubcgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqriebau.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kzhdrjib.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vwovlmuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iakmdqza.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2xfhwneue.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2cmmetntd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wvxhpwnx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2qbgoxymz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2arcgyuzw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2wrmlsakv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2hegoxoon.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tqvlnzrh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2kvtatcwt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2zbnffitv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2xjtgomkb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2bpwezyye.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2bmiydtam.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2wzygyqqo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2fwvvbydb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nbwlilzi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2odylhnnq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mdtfbnte.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2adsnoudw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2kzvufjay.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eszjlwkj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2bsxhsqnb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2unwwtzcy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2baqpawyq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zrgbudkg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uagpdlcy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tnaknlsm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2mmmupsoi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wyddhrzm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2inyiaytp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxnunefl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rwttanwi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oauhtooh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2suqusyvh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yzfctzef.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hibbunfp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vjzfufzq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2chxzozvp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbicuevy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfzifdef.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ckimbpxl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vewfkdmk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hxmzewqj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ngzljmcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pasunvqp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kbcssahj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxvbamka.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xldzxjun.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2doksdifl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2gtrirbdq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bdjzpcmw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2yhosbmxa.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gepsvrin.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gelprhkz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2xjbswmzc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2khznrkat.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2nacqdnoi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2hdzfwwvl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nkeesidh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jrdbnoox.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qirwxyaf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lpxmcpay.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xmpseyrg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2aivfigkz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wblmrczo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2wrojtcwd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vsajjolv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qnwslljg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aurbwstw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aqzfnaiq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ieuedfir.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zzmiagxp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rweduxal.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gqbuicri.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zdbhequv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ovktupqm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvdgwrat.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hjuqzvxq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2eacfmzge.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2wxkjgjdz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wdgniheg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zymvjsxi.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ssvjnfco.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2yxacnhmt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2vakkcgka.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgqiucnb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vmyijuka.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yhhysvsc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cjahympj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zwvgcovo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uxodgybx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xujcfhht.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jumouxge.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jxupxbiw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2efpmwvcr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ipupjnxg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cpjakqol.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bbfsqcco.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cyfuqgfj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2wyhdwbqc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qphiermj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2apjtesks.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2rkedygvh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2cczspsax.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cgccwjup.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2pfyaiieg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ttgdsmjc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2bfuxszcd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qsasqvxd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2rfxfpedv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2iavidfhz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ldnflcoh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbkukxtc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ylotowxz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2dwdcrknl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lkubgpoy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxrzvgz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2gfhayzlx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qdueixvn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gikpnwvi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fpjqzgjt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qrrbpvtj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dftqgcbr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2udvrqfrs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qptokjre.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lprquvsk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ltevqvqq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hmrkjnuj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2oxvjvoya.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jcuehepd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ifsvovdl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oviepmgc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2sffresmj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tfuhodop.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xlkpamed.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvqhppl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2hpuzxejz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2rpmgvapu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2cgiqfcxz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vkplvxtf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2usgkuyno.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tjsujxiq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lzximlwr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2azuhtzut.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xaicufwm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2arfqekoe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ipfkokvq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2szyvkzpl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2cmbkibpf.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zbtrbiwu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dhnwtpsl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ahhpruxd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2acszrffg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pxigtssh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ykmtlgxo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2lhgwwkyn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fhqshkda.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hkbcrvqq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nnnuinnz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2waifnkcu.html


<!-- 参考信息 -->