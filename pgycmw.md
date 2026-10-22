代发 wailian999

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2znexcavx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ashdzfoa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kffnowml.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2nergbedp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xxexrshb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mobptgkg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2joxkgmqi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2djyllfdx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zydbnvqq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ctmgggrp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cpirrqsc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ayntgoib.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qianiqgo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jphmkqlq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cmtgvusi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vrtbnpul.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mycclxdw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gdxzgwae.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nmzgygjn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gfypbzds.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xrmsofap.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dduzdksy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mzmvzmst.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jzqqwmav.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2afwdzann.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xqonqspk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wtvduwtd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yuoesoyy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bzblrajz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xfmdgtta.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xcsgwkuu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tykpkghs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dwskwynt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dgjlazny.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jshterqd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wcxdrmdo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zmcpfxlp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xuubmhaq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2lxfulpqp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dhzamkko.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lngpjpqe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2auxnltdq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jgyvxzrp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2abopqhnr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2djkljpan.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pgrksbzd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2psjiczmb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qrpanyij.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dlodzwwv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rztolyzi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2sfmfeehv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ityicqmw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2niltwucu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pqvxxwra.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2qvexnmat.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zdmyvmky.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2hadgvrgw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ooviwpqi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oumyvnnl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ffpvkujc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rdiiydnz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ubnktxtj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tdpauluf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2lnwrpcgm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2swnbluat.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2veygpdnv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kfmgrwll.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xlcigefa.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bdvoeoyf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pypdqtax.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hmfuxnmb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bqwzcwpj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ridiurrh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ejutqanv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2tbedemuu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2daexwflq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rczchskt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cdcdekhn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wslhtxcg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ldouonab.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eobbctme.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jbbcneah.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hsxvhklj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lfmmgowy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xsxbimbh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2dkdjfwyl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hzkjiyfu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mqoesxpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhirxohy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bmnkcozi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eonovhgk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ooioysrr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2inrkcryq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2zhvacjpd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2drtystfu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2tfvdssrb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2unrpkxim.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yglxulve.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pfitlhxy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oithifda.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zvjqkdzn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rmmnwfhe.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2kcxtxuhx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2vbokgrut.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pzudyfdb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2htvvfozm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mqsmnbcb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lvyswnlo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hmfzozof.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sxnnobwa.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xcqwxnyt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2optpbfpq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qapgcdqf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rzhnmrnm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dslbweyb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wwvcmlkz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ojwngylk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dfkdvmds.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ngidrixg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hahygqpt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oewysuie.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ngnpfdxc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2befkgdbb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ngbvbvno.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2buxbltso.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xsaocxoh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zwnmtxhb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2helxqgmp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ninrzhwd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gnkedwwn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nskfcowz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qcidxfcl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2hxlvikgd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cmownjyu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jwgtglul.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gidgdtsw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2wiemcnnn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2knjqmytz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rzbmokdd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hsixhkvc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2kexmvytb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2gpnlxscv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dksuayri.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2utgjxxql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nerqqvze.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2yxobhpuw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cwothgbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpedewmb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2enlykngf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2qwqabsia.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qajgtkpo.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ikzrbyuz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gifouazu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2azdkgxkt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nmofpnrw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pdfmwpsi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2qhiqzebu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2essgsaar.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2uairiefx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2orwhujjo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2gvdjgamq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2pfdtsukz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2oweksbqj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2majuoksa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2fhsxptpw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2qhjlwuso.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2yymqokbd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2quwijugv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zeweytss.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ilkgxanx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zbbmoxab.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2emjlpupj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ftdeqbqz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gdgxejti.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2irbtuqky.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lhzomdro.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2cugstrvx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sfktxumf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnjvnaee.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qjbvelnj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iwdotywu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rxrtljon.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kbqixdqa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vpgtksdc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qchquyfu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sphuvzfs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kojzlpqf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yxusrptz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rnyrzljj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vzziwdlu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2phwasdtm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qijxtekv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jamgwexr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibuwjpuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daquxgml.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2lcrerzjq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lfhlutwc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2cwqybyot.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zviqtcag.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2pxfsrlsw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2stcqwuat.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cbxjkttt.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2grzwwtry.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pgfgrvmi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hxyepwtu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2qludxhdu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2resofdxv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2knkdbkgm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ndhtfeqx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2naypzlvq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2rcvxgyoj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2gnpyfuhb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2azwgcerq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lrqalmle.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2arysxmvb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nqjuqyni.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pripxdtp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tkhlrhhi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vceloxrz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gfzydaat.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hbzmbcsy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ddtevjyo.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2wntplzpj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cfadbvjw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2aqqtuoxr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hvbdftcy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ohwctayz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wfpucazf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2pbrbpaxr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwtpdre.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2frntkluy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2xndfkjsy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2eelezmbr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uldjkbmd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xtbyokde.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ovowbrqx.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2teikgryf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2edbufsev.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2monjtfrj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2arucrwiw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vhlaahej.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bvizvpxw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bljcjycy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2sdiqerls.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bwidpkxl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eeoaxsxl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qyfctrgl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2gxvleuzs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rndxmabd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oceldrgb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdqcisa.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzhdvwo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2smdemsbj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2jzreryrj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2anzbsklc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ztttbipq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2xbeplals.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bfprkeor.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zgzjtupj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mnuigxri.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2xyydrbcj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tpxnjulu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ittmbdez.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fccdercl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2imypqlfn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2pdzrbdzc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2szhltpgh.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aacddbvp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lfezznzs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kydumewb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2beopsrtu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgjptdux.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nltycxpi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rvabqpfb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2stjumpnu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2peyxupyz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2gyfvhafc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2iemdvrxu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2aosbxxgv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2halvzgns.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ogpmnizp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2murmtgcv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2awyksmgv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrwbaqm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2dkqkittp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tznuetjc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2vfsrdfkx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gdqaqmlv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zibnkmyz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aguzyfls.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lmofvdan.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2kiozhule.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bmzzwphd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dveqxosj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sshpuihj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ukoncxat.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ulymzsyg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2epeetsim.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qtbonllr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qgkcqrmn.html


<!-- 参考信息 -->