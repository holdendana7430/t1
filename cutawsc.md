代发 wailian999

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/grhesnwdg.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gpvugednq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/glalgnpoo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gqsjfrrys.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gxplgepqe.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/guwxngboj.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gilafotar.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gavxcpdyz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gjdhdfvoz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ghylzsspo.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gskphpczd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/ghrsgtfmm.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gzwbejvwq.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/ghmkybczz.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gjkgjeuij.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/grfhhhtbp.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/goonxgxzp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/grvcsturs.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gvfrspdrw.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gmjyhefyy.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gemyamdti.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gmtbmrcmd.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gysxddumh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwejatxqy.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gwqdzshkk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gdctnpefc.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gagzpdbhy.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gygmjgryp.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gpqurfcrv.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gyfpdxbfq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnugluepc.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gucgvcgib.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gfgvhxviz.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gtxklvioy.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/ghlofteld.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gfkajlhmj.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/ghggajlfe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/glczxpjhz.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gurbbxvwq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gkdoosnde.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gekxgfgyk.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gdxnmcajl.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/ghtauozgr.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/ghxnxkulx.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gyjynkvca.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/glywcyegk.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gmofzyhhe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/ghngjzmia.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/getxvoaci.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gqobkoegj.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/guuseywyw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gzfoivvev.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/ghoedfqht.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gcvporfct.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gfhumrgqy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gczrrbrvj.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gfgjeqlmv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/ggotxafpx.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gwhwlppbx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gdziqrdnm.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gcgeziuot.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gmronjoem.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gnjqoqvyf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gzdrkmsgd.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gaipnthyd.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gzvudonja.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gonrxaigq.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gosrzxqap.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gazmumsud.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzomamawa.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gjbgikqvf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gykjrcweq.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gcnxbbvos.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ginzrhxyb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gefmtkdsz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyzuyvpwv.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gewpiczac.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gycfcpicm.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gbzbsosup.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gkpyznqkm.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gdxbnxryn.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gxpardqql.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gznmroyja.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gwvpkozhi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyuwzofxf.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gehbetotz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyqvffeuf.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/ggbxqwmwd.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/geeoyicjm.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gwwamaybz.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gddixvcmu.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gkmccsbvx.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/ggzntzvka.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gczprynof.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/ggaliyvbb.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gdcegpdpf.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gfhrvcmwo.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gohjdtoko.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gbbkedewe.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gfutjuvev.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gzfciaiyh.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gxbxmlxqa.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gjnmupfmn.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gcfaiqopr.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gwspwgbwg.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gpdnnmtjh.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gouhqfzsf.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/ggslniftv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gwyjudvlz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjxrdvxjl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gnozsyvcy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gkfhwknxh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/guouzzlue.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gtyhvubzt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gkzkrxbdt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gxpzldkxf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ganekwpxe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gqxoylftf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/goajrgdhy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gaihgngdp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwiwtgkit.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gkmftmnxp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gzzpbxskk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gctxkkniq.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/ggpxwdgan.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gwvynmabv.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gzhrqjcev.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gwwmijbdt.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gwoucjblq.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gbumsghyv.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gwrlcmmhs.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gjdptolbw.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gzdumfkir.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gfnoxkllc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gajjvbovf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/geshiokgy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gathnsbda.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gbpuxrggq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gkcparzxt.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/ggvrbmcem.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwckgmoca.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gahfbigxq.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/guoazpdxp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmbnoiskl.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gsfommxlr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gjxcnpmpu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gsxmgwtlg.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/grndyhlgs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gavqwsnll.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/ghtknmnft.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gvppbhzee.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/goyzjaajo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gtffpncrj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gvkozmlaj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gcxfpupwq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gtmpvrpeh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gphlrdjng.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gtdukhtws.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/garwpghdk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gfcaulcel.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/ghxgcwjqv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gtkrxpmeb.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/glmqipble.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gnilqbgky.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gqhsgwhqv.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gzarjdugk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gzxgyxxax.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gaispbxse.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/guceatsjv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gapgyfdrj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grpltxsvl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/govecbuvv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gbebupfkq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gcnyyiqbf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gdxcifwac.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gywrvphbs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gkayyoyyu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gmjgemlbh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gjgmvykev.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gmnxpxtqa.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcizlnyla.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gyznaqgsu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gcgimoiaz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/ghzvrpqqx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/giaxbflhu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/glpzafikf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmalyyl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdrpbeusp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbcezedwz.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gpqgpeuvh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsvsiiluo.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gaafoimwc.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gotbbbqry.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gmemcpetu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/ghbmowwdy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gdjzfmwhw.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gsvuftsul.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/grvdbjzos.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gbhtuwaim.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gqxkqevtp.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gaxvdvdff.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gacfubhnt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gufxsspyx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gmscrqyhi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gfukobcnr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gkmndwkau.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gwjmwgkfb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gfmfixjge.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gbuhxrict.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/ghsjqdpma.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/glozyjhyd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbnuhedxj.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gmvnopebs.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ggrtgjtun.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/geapwxbzs.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gzfydptyf.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gecbexfho.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gciyfbcdh.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/glioklkkx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gbobpqmow.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/gkupbxkgz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gjtnpfgnz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gfnyhpdei.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/geeevfelm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/guvtganpw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gcrtaefco.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gtghpfwxt.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gdauizzwn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gyrcxylea.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gubtpkibo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gxngjuibi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gjxzsdiem.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gpjixvwef.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gsvbtpiyf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gkxfllezf.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ghnsisimz.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/guzvdvuef.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/ggnzobimy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gnijrmlzw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gnzomjpih.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gulttbdlc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gnwmnvdne.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gnwccjlox.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/goizdcpnk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gtgjjjuko.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gvztnyykn.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/guufvcrec.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/glgeyejfc.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gloikvpki.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gbvcyazza.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/geaxeujst.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gmaetxiub.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/gjujklwpp.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gphxoyppd.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gftlqcxub.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ghacammfp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gethrjhzy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gksayqfqg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gytjrkfyy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gykoinzbc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gfgwqfpab.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/grhjcnfmg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gqrpcsbzq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gdvscplwc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gxcnxvfev.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gagkqxikj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gltyoypch.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gaqyridjd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvheexbll.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/grbivtfsg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gzbolfgyy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/ganvabjgq.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gdvivotlu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gbbdvmxjh.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gjwcytwbg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gpzikcffg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gbeinrzhb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gwvutczzk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gfklskhss.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/ghiatqsbe.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gpybtuidu.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gxuyeckkk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gutkyytng.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gtblgnmcc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gwfihmpja.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/ghdiuktyt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gdwuupztn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gfrbbmfeb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gagpwkyxs.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/glxafzjgr.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gytqqgegb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gvmhfcely.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gyupptsjx.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/guwmdmyfc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gvrfrrerg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/gawkygghd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gfpygdydo.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gyvmbnacg.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gwlczolub.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/grzsitxqc.sHtML


<!-- 参考信息 -->