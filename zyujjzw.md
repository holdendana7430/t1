代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gcuvsjlne.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/graifzcxt.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/glbcvntpc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gckxbctqo.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/giqrlytng.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/ghabhkddp.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gugbxtuog.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gfwaifeqd.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gfckuierx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gjdhlyrvb.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/guoggsovi.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gahxatxcg.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gehvytfsw.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gqsynwfmh.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gxxknkqhz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gbwjzvbel.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gscsmhosb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gakutaupz.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gqbnmsfki.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gozieuiva.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/guwujomxe.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gfoaqqxsp.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gblfywjod.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gvmhwmxvr.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/ggbvudpoy.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/griozqafb.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/guxjbjyst.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gngcbidur.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gisjesfdp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gtaldbazx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/graxqjbhy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/grezlddri.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/ghgpovmxz.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gypljfamm.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gtbxmqguj.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gunbypubu.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gegmxekgl.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gxjkbyhmz.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gdhdbtgdm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gmzuskxps.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gwpctcdje.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gqbxdqyrm.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gajpnizyz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gggeppufm.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gbyvvmqch.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gspydzllh.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gzhxhcetf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gfowgaghy.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gkykjfpxx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gmwnfeprt.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gpqeqozlf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/goqmpvmka.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gjeihtqwi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gawrjfzpd.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gogkkjkpr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/glpbevvqm.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gqmgriotx.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gilctgbwo.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gqinmdywr.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gyfyvvjmj.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/giqmpowlb.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghzeousng.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gqwrhfspf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gieiraycp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gnoafuszx.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/ghthybxlk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gkxgdgusi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gyjeoiknp.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gqomkiqia.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gjaxtcjfq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gblyodvwf.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/goswrndbh.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gfldujzmu.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gvszknbhw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gojrjhkgi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gkhjlzpdd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gscjiqaed.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gggkxdxul.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvyhibldt.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gnmpderyf.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gyioossen.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gvarkdpnw.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/ghxhpingn.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gslzwvnef.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gntmvlsrt.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gatolezow.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/giosahtrt.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gndhckfbp.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gpuuxelsy.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gcfcynpug.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/godjsruyz.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gfmiomoxi.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gcncdukei.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/glqqysnls.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gfjxuwjtg.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gfsvrkltg.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gkevmyudd.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gnoqrlzix.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/geejuywhx.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gkzwpmany.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/glpwivzml.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/glctpvmpn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwqtvcicj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/ghjnnyzae.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gtshzlsqw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gtfvziqim.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gnzwfjwqo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gdzsxbwec.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gtfutolfa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/galtstjwh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxsurkglz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gynfjyjbt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gajvvxxun.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gmffymbvc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/grgvvqwyo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gngzjotfl.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gdedcaidx.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/ghqgbvszc.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gsekfgpgu.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gqpzgbgck.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gqjwjadfh.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gdjiapavu.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/genfaazzw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gwzrtwbvl.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gmlmrgypc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gdoavdfkw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gkvlstcmn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gnvoruryn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gfxspyftk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gkrblpwuc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gyuoxhfko.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gsrglipjp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghugiqxgb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gglxmklfr.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gjytsnfto.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghvflofpw.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gvzwqomzm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/goqfmygif.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gtiqlckix.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gzsnysoic.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gxsvtjlac.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gthbejbkk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gzhxtbnhe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gfjgaojwj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gpgkkhlde.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gpcauiasa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gxuscezvh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gkyizejvs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gcrskxcge.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gjwthmhqn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gkpkonrvm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gzlckvvqi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gjopkhwky.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/ggcnzrzml.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gxvsivkgh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gttpkffij.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gadthxjuy.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/ggrzsmzbs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxvvoodpp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gvvqwkidu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzdlzwltu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gnxrichdy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gklrgynhd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gwzsitisb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghobrdetc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/glpbksdba.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gfyupoaug.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gatmcbrdm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/ggctvjbjm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghmivlxru.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gmbbfmnll.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gwuubelje.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gytakziht.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gwgcnwcrb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/guwosnxqn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxdgfsxpx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gmzuxfhnb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/grtiewetv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gmugqarhc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggugwecqw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmvmxaeft.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/godedacxn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggwyqcahq.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/giimcwcmz.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gefkttyds.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gvrvlvcib.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gefxefzdc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gxmpuguxr.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gqgrymtca.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gcsuwoomg.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/ggnchzlkm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gsjvnuypr.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gikojsmwj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gtqahmgsj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gpcwsrhwk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gvipzavco.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gtwlxxzlb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gliktpxpp.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gnlnymtkn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gadeiaakg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gwhtxrnzo.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gobxitice.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gjesbinig.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnybbjjzg.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gumnxcnfm.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjfgkjyht.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gvwaecndm.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gujkenmko.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gyuwawsrs.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gzifmxemx.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gwpqjzrpg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gpfyeskoo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/grcgmaiwn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gyfqrhhcp.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gfzpioaof.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gxbdaqibn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gmwojfrup.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gpbfkmuwn.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gxlweeqbo.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/ggnvhmere.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/gmshmlcir.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gtyzezfxf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/glnsfesau.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gmtfprfoh.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/ggbkcixuc.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/glilorqzy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/guktcozsw.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gbvhojibo.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gwepphohz.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gkciddopj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gyeqfjchs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gkmzmqiec.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gbxcwhdok.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gxcsukmrx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/girvcpdfb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/ghruompkk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gpvxdkdza.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gvewhrzat.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gohuxkmse.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gxyjqttns.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gcmthvrlf.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcubunbb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gzskthbpn.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/ggfxswncb.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gpdpaujtf.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gbpzzssmc.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gxncgxriv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gfhaldntm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/glhbkgkdo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gnlmlywsv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gynolvosm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gryaceexw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gjdgzdyuo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/golnickog.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gwnbhvytn.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gqvyadjdd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gneiwprfz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbokoqhsm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gvrfthukc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkomggssu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gtmciikzl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/geisgwiig.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gujznwwgp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gcznqvmtl.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gowfeopjb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/gcrxzniwt.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gokzngboa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gliuzzcro.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gtbudkisw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/ghamhknjr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gbrsqtfrn.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gwueghwcy.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/geeutgjrf.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fehbvm.com/Article/details/ggeklszok.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/gtmbkhaep.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/glaiixtvn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gwcezscgw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gitgjqeit.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gruqqrtiw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/ghbvvxrmb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gnssvqhgf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gurwxvhao.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gyyjofqdb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/gaqyaeczn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/gapukpxso.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gtmatwspg.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gcblezorz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gvcaxxrmn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gezsysvcc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/guelkuttx.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gsopqoyep.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/glvwgkkfg.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/grmjaxhcw.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gcewsyjrl.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwiwjyjpd.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gznhapfuz.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gqpozrgvk.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gfhzolqvx.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gjxtpdttt.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gbrkorpqb.sHtML


<!-- 参考信息 -->