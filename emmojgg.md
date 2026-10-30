代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gvdrudlyc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gjgkjtbow.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/geedhipwd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmcqgubo.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnmwpliu.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieujikfu.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gskuigaal.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunafsmqu.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqabkcuy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyckurup.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/grpuvbmro.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpfzkhvr.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gqnywsgtn.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhbuimhd.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gyclvsqzj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gcqqgunbe.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoikaihu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhrqtsiw.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxjqxrzh.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsfslfqh.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjzdplpr.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboxlkcvo.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdoeflbxv.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxohgobsb.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/ghlgshfea.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqolktyk.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfpzuxqg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gevcfuqbn.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gruhqagsl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxlgavya.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gkkottgce.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxipuneo.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvrmorce.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gftisdsgh.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gmgibttsy.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjzxwaki.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/goacvmntm.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gukitwuxr.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeibcwxz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaecxqtx.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gcygujrxi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvvjwhzb.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuxsukoj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/glpayjxqa.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/grcpcsfjl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgkjflkd.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjszedbcs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/grifjkgue.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgdljtzc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeyhybar.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkljwgnk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/ghmeauhwm.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gonatdvlo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbapfmoen.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/grciycwwb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqzftzgm.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyntfgyi.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwiqkcwj.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gkqryrmlh.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmvsodue.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gjpezvphe.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsixgbmi.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcmwsvflc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlodqljw.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gmstpmxlt.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gklaymavk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/grodbzxpv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmqvmfeo.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gjcbnvgin.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkycmgkme.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gofbhmraj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gyljsdtdn.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gbvrrgynr.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gjbmuybll.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkxgvpgi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlnzaiwa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gevvsylma.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gltidcesj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkbdoyga.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwirhoux.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmvsmqsu.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gwbnfckyo.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/grzqmaxhj.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxepejxb.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvzexbrz.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwbgfrkh.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gcckrbddk.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdzmmkhb.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gjkqjpjdm.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkhepfup.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gcsxwykra.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbtelwqh.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gxumxisaz.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gjyfyaiyy.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnhpughi.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gsvgnxdab.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gdedolpaf.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxmfiurl.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gnyxtdwna.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gyhvghpav.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gnglaghvz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmootwsu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gopbhqdlr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjvthtty.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnnrxepr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccrwfyay.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjszqyff.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtlekqrn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gemuglfcb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipgkhkia.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gljlbtvrf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guewhbowo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqyojhxq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/grsinjdlh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhmjnruk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsbzpuvz.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gvgsduhdx.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkaqoqcu.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdegbqgt.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoazctlm.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gynufvych.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxrhliem.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrecgpcy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gajbckzvz.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gibishapd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/grwemlvyn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdvsczss.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gqmroetuj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gcqjxncmc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclfqbxpa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gzjllrpii.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gletufyxv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtttcmuw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/geyzrsvyq.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gattouvhs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwobtocx.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoxgsvll.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/givoaxnuv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjudwycd.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/grthjmvfh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gcpechdfs.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/geuyofhmw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gccjjwkwz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpbpjqkh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gbrixyqrg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gximhhqkn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gsayzlqoi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkykbksee.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gfjfyorsx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmgqtxwu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/goqbkioes.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyjjsjwg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphhpgfms.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gzouweced.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfbueipg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerlwhcol.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gawypljjz.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmfjtodd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyzxnfxq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gjgldiqoj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdhrlklt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhjsgqjp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gncfrupxu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvejufbbw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghponraoo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/girmopuyh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkoghemcz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gooalxzmf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/giygnhnfy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/goqmsutkf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gpotrdsij.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gspfqtplm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grjnqjdql.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxwfpmhtf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gzgxtyjpn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdmnuqam.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjgaqwecs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpomsfluv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmohlajx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxbcjgrji.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gitpacltn.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gqzlupxlt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvwxxcph.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxgdjbjm.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvpndtff.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fanxiaobao.xyz/Article/details/gqhnhcdmz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbiuizfa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnevxewtp.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfwtyqbc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gulfqvjsx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwewqiwc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gyaltpnky.sHtML

[A02] 变量声明与赋值
来源：http://baike.fanxiaobao.xyz/Article/details/gjbjejdjd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvricglr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajqxnouz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmofktfon.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpfwbavm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazzejpak.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhdjvzzt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeeyvcce.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgefximf.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtucletcq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgpksttw.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gamkmvscy.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gctiwuamq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlkkjdmi.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrtvoewv.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcoanpht.sHtML

Ruby: PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gdsdnhekx.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gfabxsduz.sHtML

[A04] 判断变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqzbponl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gylnykwpz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxmutfrd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gorkyyinu.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gxhpqiopi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpzlgcjd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnenzmpyf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmehvxdx.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fanxiaobao.xyz/Article/details/glkcsmppo.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxwkafqp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/ggdoyrutj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gravvowle.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gezjtkplf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvjpamst.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsurmygry.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsiezijvh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/genasknkf.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcozmccf.sHtML

[A06] 字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnqrakxu.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvxpygoj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhsalwbq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gpefpxehw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gbwxnbpld.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gylwdxlyu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gggpceafh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyalqvtvm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gypjdkutc.sHtML

[A07] 数字转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gysssgmlh.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gilcetyqz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcuwqlfk.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbmtimns.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdllkkzij.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvlxqnqt.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvamfepv.sHtML

Ruby: 42.to_s
来源：http://blog.fanxiaobao.xyz/Article/details/gbwghprzg.sHtML

C#:   42.ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gazxygogy.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbebnjyqj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllhwoadd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwzglbbrp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geynwqpzy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcmypuce.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gstfyzvkc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/guyhxwuxd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fanxiaobao.xyz/Article/details/gorbqiftd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxalzhau.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrkuammz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/glngaekmu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/groybtspl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpqorooll.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grkxhqodc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfejjriw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjngdrdi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwnrblcw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gczdgonzc.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gohjeidyy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoauzufl.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/gptjbyabk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/giqcnjpsc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbjldvgv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gllllrary.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fanxiaobao.xyz/Article/details/gtdsalojl.sHtML

Ruby: rand(1..100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlaixipi.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fanxiaobao.xyz/Article/details/gklwssmwo.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnscxycei.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garfymkcc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcedputfe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjlfqkad.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gmbrhzmur.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/geopohgvh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchkvabgc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/glcmgvgvr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesoalacm.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/givdbtqre.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohpzqcom.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaiiaulj.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcaamkwq.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfwtiwpz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbrartkr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcdquwwe.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwgjswfu.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fanxiaobao.xyz/Article/details/guyfpebkt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccjxqvrl.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwethwok.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhiimkqr.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gvfdwyjwi.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqegyxgg.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxfwgqxj.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gzskvhqlo.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/giwlmtixj.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbrwaoil.sHtML


<!-- 参考信息 -->