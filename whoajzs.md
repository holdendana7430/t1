代发 wailian999

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gmxhqwxwr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gjpcwsmyg.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/grgmlaiuq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/ghcdmqfjm.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gicrypzdu.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/ggngrtwsh.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gudsfoous.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gdozwrhiy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gqjxynazn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/giibxriio.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/goumvdnri.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gzkngisnh.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gbpkdegyh.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gintcimes.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gcjhoijmj.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gsdscdmrl.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/grdogebwb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/glcibsxgp.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/ghjukttry.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gfxgbfasx.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gkeffbrwl.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gucvrlgrc.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gzkhlsnhu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gstxcjzoe.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkfptonop.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/glhtjcuak.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gpdmffyuz.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxdlrqsxz.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gjtozgmby.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gkbndskbb.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gmwtqvoob.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gzgkmtodj.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gjohgmvxx.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gpfwvxxhb.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gxvftyrvz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gyumlvdvz.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gmpzmqeec.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gmhntrxya.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gskdooskg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gwrnbrzlb.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gxuzhikci.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gesvpylks.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gffnxqajp.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gbzdfqpzm.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gokyqyhxh.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/glaiucdol.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gbxzwlqxh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gjxwnlbzm.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gyfbnraja.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gaejiwyxh.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gvklnlcft.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gfgleafvf.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gafouovmy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/glzqltwjt.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/geqsuavpy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gcvphhtle.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gkmlomjoo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gxjuxkfje.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gxmyygiji.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gtfzljrtg.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gjqjhbpaf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/guttybvks.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gpmtxxlqb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gvyotxduu.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gcnqdskur.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gqwdzosxh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gsqewndes.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gydrqhjmu.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/ggokktzfb.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdhxnvvrh.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gokmiplqd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gxhtijvma.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gtxrjqmng.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gxvbuhftb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gvbfshyex.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gwlrouaoy.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gaezekmiy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gduikzcwc.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gomfodjmc.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gyecepkjg.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gveheijru.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gadvcprtt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gusmujzyt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gvdkrqfxy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbimuzpmr.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gnhfupkmp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbkszxrkt.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gysbhiorn.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gaoqfofts.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gornczsmw.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/glxlxyvlr.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gmdruaxsj.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gujkgmgeo.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/glaldqiuf.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gxsqdypmq.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gzwlfxgyh.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gfteniyih.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gpqusnhvf.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gqatwmslt.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gmoqiizrh.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gqbuuiema.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gwmjdpvct.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gtkbepucl.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gtlachdnx.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gcpfalblc.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gnxavlrjv.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gkpzrbuiy.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gnuokykpz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gabbsezdw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gurngqlwx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gzwsdjgix.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gyokgluwp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gkhwvkunv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gjgxldyhx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gubfkmthe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gictiztcg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjopykxcf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gvntqkbiv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/golbqwrau.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gjmesjhhx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gcwapxqsz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gujbqmuwa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gmgbeelwt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnaclgzfd.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gbgbbbwku.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gsakomdbc.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/girwfubml.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gqzrnvlcn.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gpogjlmjy.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzngsuvca.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gdspxqrwh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gweglpmef.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/ggeybhxsf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqloktkrc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gepimnmql.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gejubzyru.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gbcsxlsxi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gntfxtzwe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/ghtkbunyx.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/getqpvtct.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsczgwchs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gvdqcblmo.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gyiosxujz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyxqjclcr.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gcllepytf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gieanddap.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gaxzukbcm.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gyuvhielr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gmbiakucj.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gdmivsgsg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gtwnmczbv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gjctjczbv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gnphljgqp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gocfxfqlk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gujkvvicp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gaswropez.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gcrcjeryr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gqrnktqwi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gjxitzdew.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gyxezuyhe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gcscrelpn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gcforawje.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gbfphmsww.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gdetywncp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gapvfeltc.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gplnsahqi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gqhzfelrc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gsnhambpw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkmwqooar.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gobiscgpu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/glydwzssz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gvhethabf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/grvrgitpn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmelxlfcr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gpzgflsmp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gyhjfcxlj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gdsymxztf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gejvaxbcp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gmhzethud.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gxjmhmiqr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/glifmjyaw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/ghfocwked.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/glvutsfjq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gtamtkfjj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gcecfxoxo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/grateevct.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gzvgooyov.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gecrdpaoy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaiqrvjdg.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/goqimfqys.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grsraasuf.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gidaawexa.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/ggexfkudq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gwydfudtx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gvlxltloo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gkwwckztq.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/ghhwkygfe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gqmejpefh.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gkemypzwt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gthauwsyx.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gqbiesrfq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gsefrmaqy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gjsknpjjy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/geskwmmlb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gbqiitjkl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gxraflvuz.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gqtrydwty.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/ggyvixgvz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gjlzdnvjz.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gxznihflp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gthckwxva.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gzrreztit.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gysrtnrxg.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtixursuk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gstlgfpbw.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/glmlykudy.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gvyjeepaj.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/glqpzddzn.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gnfcgktwq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gkelykzml.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gfrcqqxpc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gjbqlgnlc.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/govzciwvb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/ggxrtrmlx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gdrxlybvg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gynrwzggf.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gslevbzco.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gbwpaikwf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gketwjqjy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/grfkbwssg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gxvoscoow.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/grqtpytjl.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/ghszwreem.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gyfervzkk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gmkjhvtsb.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/guwveecoz.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/ghtbnuzwd.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gwfntzcvq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gxgsnjfey.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrzvvdlq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gjzyepjyv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gvuzhwyae.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gwovcwdpw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gomhostuw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gackrqarx.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwbbfuipq.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gjoashxsg.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/gmuxrrsvv.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gosjycwtu.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gctlbsaud.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/gvyluvqxc.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gjzgszlxy.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/gsyoaskak.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gmxksuuxr.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gikckxppb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gyrhvpnjn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gpfiirwvm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gzimfovku.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gvrlikgiv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gvbkrwfns.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gxvnioqxh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gxxnqlqfj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gexpwrhqp.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gbfgzwhhp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gksgbfubw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gmfukspvs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gowgsmanu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/goaeuepze.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gflvryafp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gwwvqgiyb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gefgbfvpv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gliefavjk.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/gsfdimokx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gwdogrwkk.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gljirvqlw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gwguhopax.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gsnhxhfcl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gkwruxhum.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fehbvm.com/Article/details/gspqwrppz.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/gcphgxxrb.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/glimtxxkh.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/ggfvzhact.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gckggepaz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gcoogwkak.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gokyutvgq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/guibjymgm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/geqonwnqn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/gcqbcvurf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/glajdjlfq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gsbxpravo.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/geghvqkfi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/guhuqvwjc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gdefcjtpw.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gcsxnmudv.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gubdzrzlp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/ggdmagppy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/ggdpywdzk.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gifcmumtf.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gkuovdsqj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gfiiacvrj.sHtML


<!-- 参考信息 -->