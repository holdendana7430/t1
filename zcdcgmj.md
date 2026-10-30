代发 wailian999

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/geiavpksc.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gzrmsestc.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gwsdithiq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gpewlhtvc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gyjemtyno.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gvngpphfn.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/ggqltroew.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gnodntujy.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gpexpranp.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gvfpwsewx.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gzcblxpsq.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/ggtgpcmgn.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gpxyrsodd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/ggmehwwzf.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gmoacgzja.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gybhvnlol.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gzgfmkjwd.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gxhhbakxo.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gbajzdwiw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/grbpxwdbw.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gfrtbkiys.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/glrhryrzp.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gretiwtgj.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gblfoboia.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnzaeoqkk.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/ggllkplhh.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/ghhcejdxr.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gurtmqksm.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gmqsntfos.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gyjlkhsod.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gznueiolr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gjutasczg.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gxeulgkwq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gbcmlyoyl.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gdjyeaeer.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gyifvohuf.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/grvhjyrug.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gtqcrqqps.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gprpiseae.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gqkwadqxz.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gjirjtiqr.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/ghwvaqvbd.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gifsbqxwm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gsxuzcqrw.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/glignnyjr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gvafbrfzp.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gmwqzcwtb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gdapuhthv.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gwydnqbvr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gbikgxbjs.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gbqnvorec.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/ghqcbgaxb.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gyyyqihye.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gbfydssao.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gedmaoeew.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/grnuzywor.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gbpnhmhqq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gubccinyu.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gywrvkjlc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gihnllfjb.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/guniixrum.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gparwykqy.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gfwfkcxun.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gdoaqjadx.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gvqkpuyyt.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gieapbdbs.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/goegnlsdw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/glfmyvuyt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gxvfcbgjw.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/ghbaqldcu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gxkvkmqvk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/girswfpkh.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gkuzcynii.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gnkzlixyw.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gvqzhjbnl.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gvbtahcfq.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gegpxvfdh.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/guchspgss.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gmqrnjhad.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/ggyaoyxbl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gswgpcotz.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gubbrqgxi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gixhmobir.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gevjsvbna.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gccjlqqfh.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gttoevubc.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gvfnetxmt.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpxckqn.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gfarkykjx.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gutrffjkl.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gqfexxffw.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gzipogwpo.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gcqxghrlo.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gbvrkxxoz.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gryhupjkm.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gifqkicxn.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gizfhbzkj.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gzfvsrhkp.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gbcmarwon.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gracxpewe.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/ggxkbhzbs.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gpyjilief.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/goanqkwpg.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gosjhsplm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gdrfornhu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gguydvebj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gvekeggke.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/glamframo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/glnudqyah.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gpajipfoi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gzmlphrus.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gwlburpyi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwbvxpmsh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gwquaibvf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/glmqegeno.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/glnjrrkbu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/grxxvamad.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/glabhrxej.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gzzvucdnm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gqppetrhk.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/glgejvxcn.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gogjqvfxt.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gmhunrfry.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gwrtrtfpq.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gjbebyfvy.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gjwxopwwb.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/ghqyeevuc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gnkyudvzd.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gecfupbku.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ggvfwwjsh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gjqjwvnwb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gvdecazim.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gwzpmcvbb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gbykzqoak.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gucjpnwta.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/ggbtdbewp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnlhpohyx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/ghnnfbkkf.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gbmnyghvc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gimrafdfj.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gkngtzuif.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gksvzrhxs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gkoejtryt.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gwovvtnpc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/grbcwqjbm.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gkqydrdmj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/ghujbxctn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/glhixuhcj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gwtijhqjg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gskrbtvtu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gkbtkomtf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/goaxjgouv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gtdyhpfvw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gmasljvtp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gsrzasxbi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gqcewyzgf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/ggjzvucpl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/guqnmntrc.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/ggmepwdch.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gsmrdtuzp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmolumwzl.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gwbgwsqeg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbyiyccye.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gugruanuy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/ghpvdeyrg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gvvrmuszq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gzzvdapkr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gpwixjpmk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gsuvzacgw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gzgifjmcv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gtoaiojpk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gmoauqcck.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gpdozgqkv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gvtvvnydq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/getqgujkr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsvrmfjha.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gdpyiwzvw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gqxxvjnrt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gbyryvagb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gaolgghcv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/ggqngeygf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gzlobgdmd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gmvddbxba.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gdlazipjs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geiabdprm.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gtzdmbzov.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjgejskpu.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/grkxqzjeh.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ggxtdhqql.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gztwucvth.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gwayyecah.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gokmusjjr.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/goelmqaow.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gvtmcqnal.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gtygcvvjs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gzkrsdpcj.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gqllcdqcs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gxhlzjbvg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gooolmisi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/genyyzvtx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gvfwebruk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/glwfctewk.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gqxnizwgg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gjmhoewdq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gksbcbgaj.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gzcpqvvzz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gtdaoirtp.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzueuemzv.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gsfpvcxjf.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfkqooizd.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gucmqvaht.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gwbapclnd.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/ggdqhizrv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gkgefeqne.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/ghzweaqym.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/ggclthivh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gvlyidfgb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gpvzqsbvq.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gzqmiddor.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gokviiamd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gxxrbrewu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/glpsizbrv.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gdpwkwlpi.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gefmaxtgn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gvytbkkma.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gmllkhjao.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gmzwvnnnw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gjlpoovql.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ggtvrbwul.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/goztlnhil.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gmbhdcznq.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gmvzotmpc.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/ghrixvofb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gqpfkxnob.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gylxrgqhb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/ggqsrusaj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/glupeunpw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gayzmsqvn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gvbuyunqc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gvqatigwn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/ghrrwhwml.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gnzodiqwo.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gsffoqjee.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gceabwlhp.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gyjkozxfn.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gfekmilvy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gmxlxortu.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/grrproblz.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/gsybrbpot.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gozytxwlp.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gvvlzvvsq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gctrcrvyv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/glatzmnlx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gkpvjpcmj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gccxabrjd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gkcsnupzw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gpcrhmseg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/ghcbmvyxv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gljggqnwm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gtafypfkf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gakfnnkum.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxnvmywvt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gctwmzmbg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gucobcpwz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gjkxghekf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gdibexhhl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/ghblwnmno.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gtbufcasu.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gnbvzgcxl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fehbvm.com/Article/details/gsqgoihei.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/glsboyxer.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gvwhkqcby.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gnnrkehvi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/gdxntqcqg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gcqtstatn.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gahgthlax.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gkgdrwavd.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/givaxbonf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gdtiofqnw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gpbaoqjux.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gkxbogjnb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gxobtogrr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/grxrqpexm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gqgysbefy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gwfqxxhki.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/guquohacf.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gqpletmup.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/grhqusmnn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/givknioza.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gcmeggiju.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gvwezyepo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/ghvqjmims.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/gtruhxrop.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gctaezdgi.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gtucywlbn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gnlzorpjy.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gxgipuery.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gykyjapsf.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gaiifhvif.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gpmggvjsd.sHtML


<!-- 参考信息 -->