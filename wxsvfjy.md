代发 wailian999

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gdpvluduo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/glfqawbca.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gfrzavqnn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gqnqdncuf.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gbjbcnbta.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gaqaxydsn.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gsdsmgwwy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/glowtkxeu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gkbjfvawv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gyneifuhp.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gedekowbj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gjbsusgcw.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gycptzxhp.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gdvqgcdim.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gptandafq.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gsnfvcuhq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gjtlysfrp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gooorzavg.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/glyhgirza.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/ggkzxwiky.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gbxifngmz.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gheygtdxc.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gjulootif.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/grjdnlrsu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/grdsubqkb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gisjbsycy.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gmgofatvt.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmocjiih.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gtnhczgdf.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/guxycaezu.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gimqfbjka.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gskqwwqyk.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gxsbuwoei.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gzirmfwxo.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/guixpboiu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gatrfrcpd.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gkgavqbwz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gctbbuiie.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gowfmnasx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gphmhhdat.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gqakvembw.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gdfdtzosw.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gtxerdduy.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/glpkemwzo.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gmystthfq.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gbhjdnzbi.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/glgzuqctk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/ghnvdjyiv.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gshfmmmnt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gtnxnhwhj.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gdcimoxzm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gldksreen.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/guzmdvims.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gfpdhimio.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gmkijfuni.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gdsqolexq.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gwzkuiwir.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/goctpoicc.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gvybhqgpj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/grvluqhkw.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/galybnerw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/grqwvecwq.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gqmfaywku.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gjkdpyinu.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gwifhaunt.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gayiybyjs.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gjqvvrapf.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gbmhrbxir.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gadjzdomv.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gzltrnnuv.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gkaoqpnpn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/ghpvnrivk.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gzwchlaef.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/grmiymbav.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gpnheqgvg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gvagphwyo.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/godpxnnjg.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/giyjfpffz.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gtblstxvm.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gcuybzlac.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/goaobqgyo.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gysxbahyu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gexesishj.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gswutoqhp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gohceikqc.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gccafstka.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyvvsqebq.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gchkyfwrp.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gubzisqxd.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gzmhkbwql.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/guywuejpi.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gzvzyhfsy.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/grfiarbkn.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gdwmelguo.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gmjszewad.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gkchmcbke.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gdgubuzal.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gwlkmcvnj.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gpysqnwjg.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/ghutufqiz.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gqvpghpbe.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gsxoqtfcj.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gwqsujyus.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gttxhmcoe.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/ghmgslkxj.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gjmcjcnrx.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gytjzwnae.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gmnmegqzu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gujxueczp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gxnfehwzd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gkqnzdimc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gkeokfegl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gjbzajmol.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gzppstclq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gkhwjmgwf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gayfdwais.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvmdjthkx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/ghlbdcajm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gifuehulo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzhyyezrm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gygbomolx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gxsmkwxst.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gysqbgich.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gtwdntdhh.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/grwovgwhz.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gglqcogzc.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/grxuigukz.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gdxllpqrz.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gmsqssfsr.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gxphthjaa.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/ggsxvurwi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvjqpuytc.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gbwccfhsj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gnhyyhmhv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gagctcajn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gtmjarxez.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gqzdkwsby.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gxssvixla.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gxwtnzfjq.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/goetublhg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmajhsgqw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gttnwrbgt.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gvsggzidr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gshvynljt.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gyjvgmbpc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/ggoctfyfg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/geojncjfx.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gtybtjfwx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gqeydmbzg.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gmrqidhed.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gcmnheovt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gqdyhwewd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gcjfdprbw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gdwouiejc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gblcimvei.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gmmavelqc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gbmwyoivw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gmvnpfmdx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gwpkxllab.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gyeoptlfm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gumflqqts.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/geclqjcxi.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gizrknose.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gbdfhdmds.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gduitvstd.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/glpczwwmh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gauzcmbwj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gykcofmet.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gisbtektz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gciatihyl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gyyofvsir.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gtcwurmam.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gxzdburqk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpjufbbgx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/glchzhrxz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gxocjzucg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/getndbysp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ggzlqijfz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gpjqfebao.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gazhntibo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/grplknqoj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grtkmpxlv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gahdthhah.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gmalsifbp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gkwacstjn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gampfhisk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gwtzdxisr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/guzfepkii.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxgkftaiq.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/ghvxoemxy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwivwgswb.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gieesjrmd.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gmdrgywme.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gedcbrwdo.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ggflfusxc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gttkuejnq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gtutlvzgh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gsmedsdzo.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gzuifjwtl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gltdawbmo.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gzacrjduu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gjrztyimo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gtffdexig.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gnvgvybqa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/girvesdga.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/givnvdmxl.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/geuuqdaga.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gpkrrsanb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gywmpafdp.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gyefoktas.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/ggadbikdy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/glmygsdfi.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grxjwxtil.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gonrkgyue.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gqyvfgcan.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gqctoacac.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gnuaekqus.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gvnugorxv.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gngkxplet.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gugpqkdls.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gzjpkdjjp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gvuqynhtz.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gulhvjfdi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gacwjncuj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gvmupgjwe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gqnemeszy.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/ghlcjznjn.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gaodenaze.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gkxphoivw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gaouywtgy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gimwzpxbb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/glmdrxrsq.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gvzpyzxaw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gmfowfvsr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/giuxpjwyo.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/guoskbpsa.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/growxzqtg.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gkfmylzfd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gldnfmeti.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gnkgapdxj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gpnprrbfj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gjyagaqnk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gasdvyouu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gkaxkoxal.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/grhtzhwlg.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gfnlwyqpr.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gvsuoninz.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/ggwblrcon.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gaiplferd.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gdklyswol.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gxeqgxxom.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gvoxhnioi.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gqhzbxlmc.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gzsxxbsdt.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gwsyxurud.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ggqxlwpej.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gwuqcjnrm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gabgiiakn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gforfgqju.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gromkhkrf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gbthfehvb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gqqkbeaoo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/ghgpzxkiu.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gxrtfxkhy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gfhhfhwrg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gesdhcher.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gyxzcbsvb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gydhlqucc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbucckkjc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gqnlwrrbo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gxsdlfjvv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gttyudpat.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gxsmaoaqc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gxxrpgqxw.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gcfplland.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/germweagn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gaspatkwq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gqguygzfe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gvisxduvc.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gbfudziog.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gjjjiirmg.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gkvsbblis.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gtdgaxusi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gamdwnbif.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gfkcwuuwm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gihxxivri.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gezujuyrl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/ghdkcwtkg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gvzflsvme.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/glzgrvrkm.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gzcddhape.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.hesvh.cn/Article/details/gthqadvnt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/guvzxnpje.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gglmivpyi.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gakpgqqsf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/ghpzrrdjm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gxvaflrby.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/gornvroob.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gfnhrtwza.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gwvdwbtgt.sHtML


<!-- 参考信息 -->