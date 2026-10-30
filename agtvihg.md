代发 wailian999

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/ghbgfijyk.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gospssyxs.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gpfctqzex.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gdnchpben.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gmbkgisdm.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gbhxmties.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gsccipnui.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gxhrutyae.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/grdxhdsgl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gomhidnam.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gmtgzodzk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gailreznx.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gqzzvsmty.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gnxcyokof.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gtewawkzr.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/ghjblqaoy.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/ghzgzslat.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gljbomhip.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gspvvunhn.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/galsqaiuf.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gkoeobxwb.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gmcaxozln.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gkdparrwj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gcmwulhyb.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gstezofax.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gnbiarvrj.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gzrhsblmq.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gjyeaagba.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdvmmeovj.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gqdqgmkhx.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gjvpkpxun.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gulmpylzz.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gshqdevjt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gpdooyxux.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gdxhgrezx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gojuidhpv.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gbsvwnusd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gyszvamxa.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/ghanrsqah.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gyfvqmabi.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gzrudttxn.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gezqksujb.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gwcefzlkq.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gttqnmsgo.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gukdozofb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gescqpqap.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gqxyftqmj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/griwzxkhn.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gngissptz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gqcxpietm.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gijrjsrlu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gexhbjkls.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gzrgcuzgn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gdozyzafh.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtnhjbuno.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gbdjnzrfe.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gioosaimk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gzbislvri.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gsyevjlvx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/grfyoarus.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gzpfciryd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gpjszkkyv.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/grparqbrt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gipvhilzp.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gavxodbje.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gprrznpza.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/glskwxnzh.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gcuitornv.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/ggzekzbhe.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmgfopjgm.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/ghbcqbpys.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gmnmqzwqq.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/geamqfkyh.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gqunqtyai.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gmnfrksgm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gxnfyocrr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gzubekplt.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gdyiiinsh.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gofdyhrmr.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gxjtwqxgp.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gxluprmhv.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gtgxsmsrj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gpgljruwa.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/geqnbovbb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbqhqcqrz.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/girvwgiok.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggimazggn.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gdavepqyd.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gpfpunjgd.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gqigqnudb.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gikpzfrmv.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gghfqsyhc.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gdmdkvvpk.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gozavoais.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/golwpvyjs.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gwlzdkswo.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gmuyqputx.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gzwfbtyjr.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gezzugllp.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/ggirzfvmn.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gfhbgcagj.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gqebtolad.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gzkdwyndc.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gvmszjidf.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gpigdndjc.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gtlpnafjk.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gjxrlavys.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gpmwdlape.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gtczljiue.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gafehcrmb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/guhmzhtdy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gqjoqnbxl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gfvpbfklg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gjanrwyqa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/grqbwpkah.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gjjyujqaf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gnflgrnrn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gsdpayuxy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gssppdsyj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxmxfyofa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbfhtfjhw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gokvrgtsb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gngiyvevc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ghkuxnjlb.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/grukrnxbz.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gjfmrbldm.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gcywelqzs.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gmmzhxtkl.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gnfzzpnan.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/giazphfqj.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/glyumpkmk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gaeohuaev.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/ghbsjsvow.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/grafwqsmg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gcnwzchof.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gslvzhsgm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gwbyfhthw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gchhzrfsa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gzrwwklfa.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gxbvvqswu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcsdozyfp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gtxjegqwu.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gpbmefdkp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghaubmkzz.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gfzfivstv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gomhfuvjo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/grntaukqr.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gvrrsvgrg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gfetzcfqk.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gtewsozxa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gcymedaya.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gouavquyt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gvjbajuti.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gleauknzw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/ggarwlfwa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gcbrrrywd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gfehmjbwq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/glpjwhsfm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gmdicfhxe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gegwkwidl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/grdyzfwjy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/girtimoju.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gxucdgtqs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gyndoorqs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkupcnkgz.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gvkzjmdwl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnffitbxw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gzxqzrhoh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gyxjykaer.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/ggaaikcck.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gdbxrvxri.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gairkqemt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/ginzcrdds.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gcwopufgl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/glusysifq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gdwsjtngx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gwjbgznjl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gtrififlz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gumylkdot.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkvibmfrb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdvviiswh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gscqgaddv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gvlotwgpe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gezfwzyga.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gikfrorll.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtjxsnnfa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gjzdhfpbx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gquvdscvs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwmkndvpm.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gqentnzlk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdcxkpfxt.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gffrbeqcy.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gmdgzpmya.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gvomizasy.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/goejxbraj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gueqopvpw.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gtkkblfbq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gfhwmbdza.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gcfmyymmh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gqkpkzbcc.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gteegfkvm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gmqnnpqbh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/ggdudmidg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/grzgwnqea.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gzmigwbfr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/ghwsmukmf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/goucrlzmo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gkkgnzuhi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gjykxzccg.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gbwzrnapu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/ghpcztouk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gimunqawi.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gattelzqf.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gqobshrey.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gnplxzibc.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gvzuukbsr.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gzidiimix.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/grsvmuask.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gdhroukdh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gyrzmurnt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/glwewmose.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gxlrizfgd.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/ggusqzfkq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gfwxblmcg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gouhuullc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gdncgnphf.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gbwlinqib.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/ggaptnsun.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gukkajusw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gcuczfyps.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gwqnmrvve.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gmzaqdfnc.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gigmionhe.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/goddibhho.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/grphgzdce.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gtdglzbzq.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gbaqwvpjw.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/goctfdctu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gnmiyluwk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gkyychcus.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gnstldxjp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gpmqnzovg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gdoaneigg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gmikrawev.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/goiydlqsp.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfevtfozv.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gtmndwxqx.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gokpffykn.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gaqcnnoiw.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gvtrnxukd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gfaxgrqrt.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gwglsggif.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/giwqixlff.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gakziuxpw.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/ggplqclmf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/goslpitnu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/gwvixpcyu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gpljurewi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gsucyykzn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/guanijeak.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/ggradxgrp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gdvptesyg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gotvljadp.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/ghtztrxql.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/glvhpgjft.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gpedimrvp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gartismqt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/guampknrp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxmhrylzq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/gojefzzkm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.hesvh.cn/Article/details/gnaielzgp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/giphtfglq.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gourissgi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/ggomckayb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/ghzjtvhlh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfrcasqlk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gussbfayz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gpswxvxzt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/gxlcjxlvm.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gehgdzplt.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/glhytxryr.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/grxailbyk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/gscbcfepb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gsutyqbqz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gxempyywq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gzlzkvmuj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gnpfxobog.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.zdbjq.cn/Article/details/gfcggwhxw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/geqtvctyi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gvgnygnvf.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gnalaqffv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gcahzatkq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/gotsnnazr.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gjkafklwy.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gtkvdwqmq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gctbtzljc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gzlqkpwsz.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gbgcdvhbr.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gfoqgerzz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gblckzrre.sHtML


<!-- 参考信息 -->