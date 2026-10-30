代发 wailian999

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gighewvun.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhnqlaav.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/guewgmeki.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/glelspvik.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gajtjdqsf.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlazhnel.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwznayrex.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwgyzfbi.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gpwgotwag.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gxxthijll.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfgxojr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxdlyuen.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqlekvzw.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/glpsaioqo.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gyqexjjlo.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gwnxjxans.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjyvkudr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvszzxub.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/glztkbexh.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbllxtju.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/goyzmcyof.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwvwyrhq.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpzmkhvz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptjrbzsv.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gjetioyxu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gimqyludx.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gvmajtype.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgpgjejm.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkfokmau.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gismwtlal.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfdaqoumb.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gcgaqjzxc.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstrqnpkb.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdsedcxi.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcftidvmc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gnobdxyvl.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/ghoyrxbxa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmmwhmre.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gybmydtpt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/grmpfcoto.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfnwmouw.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gnanwodre.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gokxixrsy.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gggkpimyq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvwtfkpo.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofsyofgf.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyfoopmn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gakkpcyaz.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/ggqenihiv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/grffxvbed.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gooaqnvpd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnevncwpe.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gxrsldwxs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gucwknzip.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gueglqttd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/ghcndwiwi.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvugxkskx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpimqdkwh.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gbltsgwlt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjocpmcs.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepoixyrc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdajryhpi.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkmfsock.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gbznlulcn.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmirfnvxn.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gxiqrnztm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyhjtlof.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gcadboqcc.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gcaazgtvm.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gobxhvrjv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gntcsplov.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeftiuch.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gspztcvoe.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/golykenmr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gtqfqgmdr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhfjcces.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkhkbbhf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gppxobnps.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gocmiedpn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmhmxwgs.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gpzqpkifq.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gzhzuwcbd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzmxloor.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/goenzgzob.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjxaeycy.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfgmleka.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhmxcwl.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjxamtex.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgktzycq.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnvmbpja.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvznxzztp.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gbmhdxdyj.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/guuvlfodi.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjktyeou.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gbhyvcuqh.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gudeowvlh.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gdhhqqgzc.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjyxaccn.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gjroedgbg.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gyebmnpyb.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gtradnheq.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzwgflgf.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gigfkbowk.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiogtpsr.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqjaerkp.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrstqjwd.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmeuwbyn.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gdaqoclhi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/giwsstvql.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ghukqqgzl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/grmweccoy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnvxdrrn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gwifpqtil.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gwzorzosk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gsathione.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzcqjokm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmxyucfh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gxbrkschz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gvxpftllu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gefcquauf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnkouivf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixbnfnv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/guocjnjtv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gkvetbedt.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/grsnrnmwf.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoegmwxy.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaskszki.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gewvxmnfh.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqvwajjy.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gpjuakvzj.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/ginuqltsr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjmuwqrfs.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gglnhdlcu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzkvvvyb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gygzzpsfh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvwoyyju.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/glusxlzbk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gbrywfvli.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/glcinqcse.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/glyzgbiuq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwtitlci.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gaafmqvin.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmffhahe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrffabdq.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gkwktorjk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktxarxic.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/ggafxfvea.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/grrmbkjis.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/grwamvqhu.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gwkhourkb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmylkqkg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/grwmbxjib.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gyruhlkrr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/giaatwpnf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/gfzltactk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gtjtavhhh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gwqkvaxkd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gajuaiebm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/gthmjjsoq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/grfdgavlc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhvimcyw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gpfdohqfd.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gvflzjynb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gdzlghpex.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbampkypm.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoulwapk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gllgtyonc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyamfbueg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gaowbtxzm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grrqiqjxx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuifshpb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkthluqg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gyqtnicfj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gmtkiyzyw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gaeudnxwd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjumywgq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqwnjdck.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfooxoxvg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhhxmuyy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/girkhhmzb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/goaxfimsv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtxfofsxq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grsrccmpu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzvebikc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghkieswpp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gzdnlpoay.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqwcbevc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsrwpiid.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grwjfatko.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grallplhd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gydlleobz.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdijrxni.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/goblkkuhb.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fanxiaobao.xyz/Article/details/grflcsypo.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guevacfic.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjxgzfyk.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gruhjxyhx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gsvpywgum.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fanxiaobao.xyz/Article/details/gjsqqmjez.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/ghbedffgh.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvjlvmhi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbabwdey.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxllavolj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/guxixnlwo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gquuqneer.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/grmjigbyj.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fanxiaobao.xyz/Article/details/gvhnbkdnw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcchmgmc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gleujaebz.sHtML

[A03] 常量定义
来源：http://3g.fanxiaobao.xyz/Article/details/gddctgqen.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gxtaibrds.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gylbtkjts.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gbtijoxqa.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgrqeljj.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gkxvhwxky.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaxridmd.sHtML

Ruby: PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gokzefuxv.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpeqgtea.sHtML

[A04] 判断变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gimlsygfy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpkdoubt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gnlabofph.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxuvykde.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gghpaduzi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/grlzlwfuu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fanxiaobao.xyz/Article/details/gspfvipay.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxlyejsx.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmrdzxux.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgnubnio.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzriejffp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiibxxjc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghgwacb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gdaayfqlk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfijqzdva.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzozqkenz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcdtsmuo.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghilxphdv.sHtML

[A06] 字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrcgfqsm.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gndisisvq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcibexfpk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/guysxjkqo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtanbhfwk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcrdwzbz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnguwqjx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncklmrll.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gkctiaeyy.sHtML

[A07] 数字转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gphfdfzsx.sHtML

Py:   str(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfrvkgvp.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaillggv.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcjcvaot.sHtML

TS:   String(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gkyixrbrf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/goantqahx.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gtyscidce.sHtML

Ruby: 42.to_s
来源：http://wap.fanxiaobao.xyz/Article/details/gwodkkaal.sHtML

C#:   42.ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gvmegiovv.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fanxiaobao.xyz/Article/details/gspqkcglm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gheioimmj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglybodym.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgnpgzrg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihzogbae.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gosfcxfct.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gffhedepm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fanxiaobao.xyz/Article/details/grjxhrxac.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhcjbbkg.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gifxoobqw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcufrzsi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gixrgegsa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzgnjfcqq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfdvfuwt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gopxksqhh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzunqczom.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzmkmkgl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghogkmfaa.sHtML

[A10] 生成随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gtetepajp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwtbrhap.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fanxiaobao.xyz/Article/details/gjylysnqh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbjzdlqq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxycrmgwq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsnxbrbx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpjvexwr.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/gfglgorrx.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fanxiaobao.xyz/Article/details/glufutwsm.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbeapqkt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazcohdkq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/guzeqbtol.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgnnlbxn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/glkdnrfaf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjyxbov.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gokildkky.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/grbzwltyd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gqrfxpuds.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxuhukvc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtbenfumr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkfkipub.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/gzzvbjzbb.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fanxiaobao.xyz/Article/details/gvslfouec.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gymmuhxst.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejfmbzva.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxzhjefs.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/guhdawuop.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fanxiaobao.xyz/Article/details/gbjoxmxxi.sHtML


<!-- 参考信息 -->