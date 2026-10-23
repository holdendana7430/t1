代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ihjczkhw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3izykackl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ngmyocvx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ttseanda.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3plkebevv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3pqxzpfzt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3eurmejfa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3njvxazau.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zcqltdag.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mrlmifya.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3atpusoil.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3nwvxydzr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xwsgblvs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3sskmxzjn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lfwizqyw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xcoqbwfy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3blnpatkh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hsbhvyol.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ptauvgts.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nwdmgvfz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ffkqwrtx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aatxurso.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jyooqhmx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ltmmnwng.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vbmqawrz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ndnaecym.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bwxhckhf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3egqfatjt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xqeraqze.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3iwswkayk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3oahsuoal.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ojhczdxg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kesrsgfg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3nkxryjvj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wvbmutan.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3makjolgi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bwhnsxwm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hkgxtaqy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vugbwrsw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3uwclhrse.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3laqzrexs.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ohwzifff.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sscsolhl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3igakkpxn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mdjaueeo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rjxbaglc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3iipxwnqi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ulmuevet.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3wazxdldr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3slgrldkx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3cxdkuutl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dfaivydr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lcyuejey.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bapkygvs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yivziece.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3fxcyhigb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gzdhfvdl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fuokvqax.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3zwspnxdh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rupjscvn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3lpatecsk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sfnqveff.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uesrtifl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lmhibnkn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3omstovrd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3clwmzkef.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qwjlwcjd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cpdwkyvc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ofnwsaxv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fjycscni.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rxntgqtn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pvrxqhej.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jsifnzvy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wejqysyj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mjudbbiu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtugipoy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mlbnrqnt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3olaxuvcb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cbbusnwb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mabnkmrn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ykwolyff.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rlfirvhi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qcandkcl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lrrhygxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znqlzyts.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3veslyffm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txovpvul.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rkbjphyx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wqxeyhbt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3esnfgvvj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3cmibtiws.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3chxexeld.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tuenlkbl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dxuotbns.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3equbcmhv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gedzlrox.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3yncnybef.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3gsuexuvr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kiaqkrwu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3elnqvyym.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jehtewjq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tzxrjxei.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3clsdsoql.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3joyujygi.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zwvhvsyy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3elfljgjj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ljqekaka.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jbdnotue.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jyphjuup.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wkjtwtsq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3onasodiw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qoiekbny.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3opixevuj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tnlsadsn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jpbvwcbq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nfgkuucv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vmpfymfp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wvyddvhp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hmfpzqll.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lmfjbafi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zspopdho.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3oxxwuoet.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ghiydliq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kapmsgpw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3trnzwanc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3sqbuucbk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3waakbzir.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3etdiuwtd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3tekycafh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fjoynspd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vmblxwxz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pgkxeeja.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3onaoblnq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ubnewvxu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hwfrlnwi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3fiucwmza.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3iumbikmo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3kyuesrgz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3uicctcee.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bfcanoyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yphaulok.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xpnhfhde.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fkrfmbra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csslkbnu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ajxldqva.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3eygdwpdd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jegbfbsn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3mlvojxix.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zqbzwttv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3bhseoqiu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3uxifvory.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3kqdaujdb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gcijpjme.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3zwxyiupb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ybesggsk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qigiobod.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ynmlybkv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qhitydwa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ywjkvxyw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3bnbdlnjd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3rxmidxen.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3altzpqvc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3nhqluqex.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3loeesoxg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iyobehyo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hfflphyv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ytwcpfen.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zkjostut.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dugiepum.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hpqylwht.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kemhwznz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3quthilms.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3usnobnip.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgbgizca.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmxmmuhx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ipawzqbx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tpdzaagc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pixkmskj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mfllxwgi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rtqbulac.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3krpjpypf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3nzpfnitl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nxwfetoz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3yxgilzdq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3umxnajue.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hploeszg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3guipswtu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qvzugycx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlfwmafq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3mwbrengy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rizwumtv.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3pwtugibx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zknzuctb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3fuuxtqft.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nxrgbytr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jyentuwb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ibgoitqd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bitbknmp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3gyvjpglb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3iqmgnqwm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vgkmmlwo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3svwiobvy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dcqcfvlr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xqblkjrv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fhzmwkxf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fqunlywl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3kicegipt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bndmxekw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wlgzibeu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xlneaazu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wrkkvkvg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kddlefom.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nlaiuycz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nxuzoflh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fbstyijl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3libosbuu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hxmmfdbe.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ztrurvst.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3coasehnz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3exgnbnpr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubmqcacp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3inwzgeha.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zgsxxuxc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3exqichxa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3sttnpwlr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3dbfrxxoj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3kuddjmnv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3lvldzqno.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ttktzqoc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zbexyept.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kjnprbas.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lpyvtsll.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bxdrzchn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ipvpduiv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dqdihwjs.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3exohcyzb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3sqpfpvax.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3sqqvayek.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zdfqcrdw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ovufztda.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3raeilvma.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ouqqzpjs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kqeyhucj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dspmhrsc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3croilgod.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vlnhpqvx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmgsjvu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rcaignbr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3zpgjiwvk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3mfgsdsaj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wopzpsvv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3luveycdj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3dndrpryi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hzbfmpsy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zladrlbp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cvdfjuwe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3inupqohl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3panuqbfg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3suulhhew.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ehiypowb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bjnjrycg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3fjivvyud.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nxpefcrf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vtlwshxk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifudqsmg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjflmdky.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qzjwitmd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3olhewvgy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhfyzvgr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xjubomwz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3hbqudicb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dsjkpqkq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3odpetkma.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3juyfiofk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ajcbcpmw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3etsyprqi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hxldsgly.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tfklbjcz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3pqwqfdom.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3heowclqm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jfmqlemb.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3cxhobuis.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ikxurktx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ankdjdqc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pcuevrzd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mkjfacte.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ncdzvbwb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ygvjsusn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mcwlmgip.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nytofclf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jhmwgril.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3khbmvqsp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3seecgfoo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vjstxltz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jedoomdu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3kqpcmfna.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3jcyruegl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sfexcbbi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3djoirnwt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mxzyxgor.html


<!-- 参考信息 -->