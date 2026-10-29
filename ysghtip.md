代发 wailian999

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gaoahdnqj.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gzmnxjseq.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/glxrtvrae.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gvkkmrrbq.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gdfeifagj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gsjqisndz.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gfsdcibvr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gfzhkzslq.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gxourcveg.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gdpnqbidp.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gtqvzfmee.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gbrgtuqzq.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/glvmlsice.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gipccmvbw.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/grvhnxarx.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gcgakqlsq.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gjqqxyoxt.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gvbqvsmjr.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gtaoojdud.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gvlpopsoc.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gpxejklak.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gctztfeou.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/ggyzjwgts.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gpmnbyacd.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gendovdxu.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gcooccrtq.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gbckyhfuc.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/glettsjxv.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gyrkvhdhn.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gtiogovss.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/ghnyfkazb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/grdgrukgc.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gvjznsagv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gprihrvgm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gclkbfjiy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gaztzrygh.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gdnpijplo.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gcrhcyndh.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gbgkenjxa.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gaepmwlss.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gkfosbhad.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gsjsewknf.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gwolkycza.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gdzverdwl.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gppspuehu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/grqntselo.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/ggpgqspju.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/grgrikzvs.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gpjupbthx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gowormgxf.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/ghwvloqal.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gcnbynduv.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/guvnrmybb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gkzroezgi.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gkuzkuvnv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gnosbpnza.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/glrwemfwx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gorvyevlj.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gnegbuugn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gcqoamvgs.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gcextjmhf.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gsmpkuolt.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gjguzyidl.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gugqswmua.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gvziutzbs.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gunxafrvn.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gcqffqnom.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gsfgfpzqm.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gktmaflcu.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gnlfswwtz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gyvnsbfoi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjqfrzhgd.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gmomofqdp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gfkpnavpj.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gwmtftplm.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gigmitmzj.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gfjswqzle.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gqcokpinm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gozmmxsnf.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/ghtvqvted.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmovulvic.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/glsqeirex.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqubiyykk.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/giofymeps.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gabucohdc.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/grmqrbtha.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gdsrgxvjk.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gfhjioyij.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gxbhwjwop.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gcpvffsla.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gdeukekdn.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gpiqqpgvi.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gxubzlcyu.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/grkemrksz.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gxzqnggmu.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gsnpyhuys.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gmgdkzxkn.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gqkskgddg.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/grrpugqcs.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gailebbpg.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gcifyntlx.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gvgzkqchl.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/ggtxyomgq.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gcjitcxds.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gdmpmxxmw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gmvsqlwqg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gnmvducov.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gxbydfttc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/geptfhojn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gqzaizwej.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gxmruasjf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gjrbmeoom.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/glbxkcqpn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gfgxohkyv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwsllvexz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/grrxpxscd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gxagcmwky.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gzgqkgjmz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gxuthfpry.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/goovyfvus.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gyykgsxwq.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gmedhxydv.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gvvinrqso.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gycmjmcew.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gycjlxlev.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gwvzdbuif.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gdkpfztil.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnzghwjtw.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gyfrojccn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gyxqjfnqs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gkiyhqttg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gbzoxqlri.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gzxwgpxeb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/glqbzgohu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gervfascz.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gcgrbmpmq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsjjzxnpv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gbrtqrjzk.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gcsptdfjq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjtwdylsm.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/genlikafb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gdklmfnad.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gcdpqjcei.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gjgxzbccy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gztpfoadk.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gqespgcqn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/giovookat.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gqytbtyxi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/grnoiybnz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gscqeguzk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gvgifjjqv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gcaifdsha.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/guilqlecz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gbffirdhj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gxczosgpx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/ggqzxngti.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gvipriubu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gttcixbvb.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gzueywtir.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gtsqaoink.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/grwgohasd.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gstnsocty.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gkdchmepm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gyupzflur.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfajltcup.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gykttmjfe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gcfcwqowk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzbsrosmm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gkbjifmvh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gsgtgscmu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/grwnrfgjl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gqhgnaliz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gktovdxuc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gkgviiyhg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggcgundnn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfwuynxzj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/grzbyfqps.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gsxzkuswx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gieapesct.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gbebxbjib.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gzrrmqyaj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gudoleczs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/guocusipo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gadptrpgt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gusvmfdna.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/ggxzridfr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwozymcvn.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gghamuzzx.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/giinkqwsx.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gzodreyyl.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/genrsrcvb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gpycwgcrc.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ggwmqhrsi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gecxhzsuf.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/glmpxofmi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gcpcabgsq.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gnhcemicd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gbjdlmolk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gopvpgunv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gqxnxweof.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gfiwgevbx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gfudcsdxi.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gvtjbzwja.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gattqllih.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gqkepsjwv.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gwwdtbrga.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gzlxvoxih.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gketuvbof.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gripwfbyk.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfyvkldze.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gajsvqmye.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gqjqqvyyg.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gorqpwdfx.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggeewibwp.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gqlgbkpnu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/ghzbociwp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gtqhcxdls.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gviskdxtf.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/grwldsmgd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gqrggruxa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gcgomdpja.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/glblfafrp.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gxphbztte.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/ghcrnohgo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gwnccxkie.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gqgzntfzc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gwiftdseh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gnkeaainn.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gveupimio.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gtwdmadpl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gteoapuyi.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gynfuylfw.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gtjgaazlp.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gnvvgwzrf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/ghutuokvr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gbjduwyce.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gxwfnboyz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gqyxvhtzd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gbrmqsell.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gzpgkromt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gmcaiuyrk.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gifcwyybx.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gzvvaidqj.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gbtjaexga.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gyrkptqmx.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gunpnkwmy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/gkmfjlvnd.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gqykqzwwf.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkaikkc.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/grocfkuak.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gpobnyzoh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gbxljrjuj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gsfqxzuzg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/guptrrwaz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gbkvyukhy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gqydwduyl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gpvbfqbih.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gtllffoni.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gtoreylin.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gkqacfrjj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/genxivash.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gbnrfhofb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gjyoaaigs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqkuiyq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gbbychkkq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gsdbxdmdz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/ggcndanty.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/giijoxvdy.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/ghvzkvxau.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gepvifgwy.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/glhmxiqvc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gtseqvsqd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gkhormkhm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gdfkcqoly.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.hesvh.cn/Article/details/gjghujbff.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/gdnncaumq.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gflwrujen.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/glqkjtcgp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/glzlppcew.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/getnbeiwr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gwbibjjpy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gnkkijbzf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/ggkroxpen.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/grfzidoce.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/giosgjvll.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gxaykfjrj.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gtoymvqoo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvodikgjv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/geywvyqkm.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gnmcfkvfp.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gpyjphied.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gtdwmqmbx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gbutxdikv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gdihcuykn.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gzbqueddi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gpcalxtcd.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gieaycrgp.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gvevubusd.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/geowevbhc.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gjgnotbkx.sHtML


<!-- 参考信息 -->