代发 wailian999

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gdbacsszu.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gjlsfsvym.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gfpgjzlfg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gflrxfamp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gefwpffyh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/guxjuthta.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gecruyted.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gyochpuva.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gjykxxzxg.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/griowbzdo.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gzoesxigf.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gswcqscbi.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gigzfkjsu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gmhuizhxj.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gtsmuroeo.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gmoovabvo.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/girzfoelj.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gqplhbpqi.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gixtjjhhb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdttvzkmv.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gzwplhzwn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gtnyymfpw.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gvkxmokzq.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gzivfigaz.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdyobfegu.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/guuvvbhgd.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gvvabuudb.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gnagkybok.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gpjktjitn.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gykkewdgn.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gpxjhkziv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gxpbeokil.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gbuzeavao.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gdqoxamlc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gslkytjaq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gwezvqhim.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gwefopmnk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gbdjgfawh.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gnfzhouix.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gkhxscuer.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gzzpysxny.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gllshnrxx.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gmofmltlg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gwxhaksro.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gvfztosas.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gdwkwaevp.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gnjryyxxu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/glifchxhn.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gkinglexm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gktoxvecu.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gpjsxcumi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gfkgpqyor.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gejhbcngc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gtmskhcmq.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/goicyabgy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/ghnalwnit.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gcgzumrnj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gmadvmznu.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gexeqvqlx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/ghynunhxv.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gqxhwbupo.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gzvtspvph.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gbmoldvok.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrfebhk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gptalcxct.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxjwsctuu.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gismgjljo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gggijscom.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gwqrnveym.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gudlnjcgs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gowdmnqjr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gihsbzjbm.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gwpvnkqsl.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gjywtetmw.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gudoxafut.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gespgkfxa.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gnyqgapus.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gzncsuhyk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gmvezenra.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gflxdvujb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvpysueqq.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gtvqjvpwt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtsjkmbki.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/goletouer.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gcokzctuf.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gptwofmdo.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/glurwwiln.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/geckecrtb.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gmnnthmzj.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gewafaptt.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gnyzmcavf.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gebqvipbh.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gxxrngcsp.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gatmihpxe.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gqysvvejn.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gorecnzer.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/glteeawnx.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/giwonhpmh.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gioabglyu.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gxnoycnwu.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gjgbnagtp.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gxcuwswwh.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gvrxfkuig.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gfsdisntk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gdwstgmzw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gnbbyihbg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/ggxupwlxh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/glagihzom.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gzjglzgmd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/ghtaycbeq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/ggzlpsrmv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gpeiiiwco.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gvattynva.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gkdlfodqf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/grgwvwozc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gyortbuhn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gsrrhnabo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gcuifqqqj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/ggmolmigv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gqzqzfiud.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gqinekzgj.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/glmypfxbl.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gzockomiz.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gmvqfvnjx.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gyfnbfldf.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grglajdcr.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gqaqkrlhv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gljudisqa.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gyijjdoeg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gbxrzssru.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/ghicjzkry.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gzcskpvfj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gwaqpzpjl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gqrtltbkf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gqauidanj.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gqtjgcjcy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsckmbchn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gnagdfvhl.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gogflrxxk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfxpwwjwa.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gbwykrltr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gvjtwwuwp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gpcguortv.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqfquhr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gbwaoffky.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gdinvlejt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gjjoxzibb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/grfdsktac.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gkhjnexrr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/grorrzmkn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gwtszstmb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/ghcrvqsuj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gbktefhtn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/ghbfsicao.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gdteafqko.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gnywnswtl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gnehtkfkk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gytrmxpzm.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gomokfwsx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/grrpgizhx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gwvzxnjox.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/grwhgrici.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gpfbzibih.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxlovganh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gjcynzxve.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gwvxygkjs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/guyxwmzgs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gpwpenuyy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gttdyjyfl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gvkoaahqx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/ghomagpud.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/ghrysxxuo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gvujbqvkl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gvpayxxra.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/glsjtjwjw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gobpgmwjj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/grmeuzggj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcdidxxaq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gkwfrwuto.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gtvbkwmli.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/glewqqnzh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gxbbubcww.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gxyeaudjd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gifajcjhe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwpwoombf.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/ghpcusnvz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gludpttdb.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdymqhool.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gbuhwljvx.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gjyrydwbg.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gooeojaag.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/ghaqaitsr.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gckzzvmwp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/ghbsyfyjk.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gjjnmtqaq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ghwelzpoi.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gewwxdpud.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/grsadiftl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gpaoltmog.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/grqwwzjaa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gopofromb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gnilgdgux.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/geqzxurwn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fehbvm.com/Article/details/gudodnxxo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gumpiljiy.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/ghunodxuy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gzwvjbamp.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gtqlekgqd.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gghdwinka.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjxdmvjay.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gozyhvmxu.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/ghxnmrhdx.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/ghmewbgcu.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/glipnmocv.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gjbjebkdk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gpalekkll.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gumobcjij.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gjfksrdfu.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gmnpyfizf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gxnmqckkf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/ghfhczlpl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gxtelltlr.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gakisrqfu.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/ghaldjbnr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/geysnjocd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gmvosgbtl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gkaxslikl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gpafsbcnk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gqdbykxqg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/giruuhrbs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gduutjjur.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmilmwryo.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gfrbnvexw.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gafxikjjp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/guptcdsrm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/graabrqty.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/ggpcrxies.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gyevhbdeu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gughmmjnu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gehymknht.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gqskcirot.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gebuzoqme.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gqvfrpeht.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/ggkqwqcqc.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gthxqhkqq.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/geouspuzm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gfdrcmgbs.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gumhbahso.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gxfqhwtsw.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/guphsklfy.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gvvinzdqn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ggfteisvz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gpfgrzqjl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gfgrtmqnh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gwnfuxhbl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gibyxlzhe.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gphjbjmpq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gbhvejcji.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gbylyzoid.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gtlmqhpos.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gxarfnbba.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gpscruigk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gragmvthx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdmiqnhxk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/ggwbseent.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gyowlelpn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gaxzczvav.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/glqqlwwem.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gttxlnpuv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gmwcnxyci.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gtkjouzri.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gjfiiylav.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/guzkqasdz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gabxmvjvb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gvsqhhtuh.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gdtrfidnr.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/gyjwjbcyu.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/grnripibb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gnfkybzfx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gmbpmzyuf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gutmlgadq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gxhcdsfve.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gxqpgjwur.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.zdbjq.cn/Article/details/gpxzjyjmz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gntuuwvcb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gglxgdmwq.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gpgcpffmv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gboonsnyr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.zdbjq.cn/Article/details/gzxsihuzt.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gwqsujfvz.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gfduebmhx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/gecoipzqp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/gsbtermsj.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gnghvtwnn.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/ganwkrjug.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gddzmbowq.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/guujfznmt.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/ghloqpood.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gnowkmcnk.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ggunmenyp.sHtML


<!-- 参考信息 -->