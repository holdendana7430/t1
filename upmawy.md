代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ovshnhjg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xxkyevlk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3efjnyzwo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jwsohjtm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gxxfolqo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ldrkftkf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3aqgohcns.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pynheizm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cgknyqlj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yayboyis.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vtfyomgb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3egrprvqx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tzgzcjyb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tchjcbkz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3uerwfzmu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3inrhtgvg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lgnkociy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3pmgdwjcn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qwsvtfnr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3dtjuheuh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3twgrpfcr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iorlpveu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3dkimbjml.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3obrrditz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3iztvwbrv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ctzusizr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gtjdauwd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3aqodnhlc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zfyqtdny.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jxtcvusi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rdpwursi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ictqrbyx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3swfdtrby.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yrrvyslb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ltqbqoij.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxbhffg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gpnzzmsr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3czpdggvt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tollmtiy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vezidwpd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jbthwywe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3urfrokod.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wbsakjky.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mjxktxph.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3smsrtwat.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tantwsuv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rgdzcbzh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3smretjxo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3msfhlqen.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgvobzi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3eiifjprt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yidsvttu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3aefronii.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sdlyxjed.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pqzwegta.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zjnhdpib.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zeaueycn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qxpbbiwk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rxahophm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zzdsnfui.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dsdzpwdg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ozopajpl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kiesmjoj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lekknxxz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wkzjzzvk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3onpyrwde.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3fclvdmri.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jkvkhsoe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jsjzfrdr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ztwopctd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bzjtwuve.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wtfinehc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mfkczawr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kixnmyks.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3gtjvvefx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvtwqeuv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pvuawhqa.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rehsfvig.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xxkcqwjp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ibstxmfo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3seztrrxr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gwysnpiq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xevoazio.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ozzheyxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoqxfhjm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3wkemhobk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwyggmbu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3aqaynind.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gceilgux.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qqltdlyl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3lpkvcdvm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hwhfdnhc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qurzeqmy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hzxzlkko.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pptimuxn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jdbwfgkz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3owtlqtgk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3cmjbudvj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xbzvhveb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vkpckuok.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ggfkdjkk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3qqdlubsb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nsgvleif.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ozuizmob.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hjddsues.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wsrbvzio.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zqipdkqa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ovrysdhu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wdufrdki.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bucaumcj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3iwsjllrp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yqyzwjxf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vrfkhzvu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nzsvidqr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xcphbmad.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3inxsybxv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3geoayudi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gbzbbbvl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rupsjepy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oinzkejj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fjwdyrmf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wdeaxbtc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3eqdgkebv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3maqjawwd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ijflnjtq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xvbzsira.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3bmmkxygx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ibqqsndt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3jmmzldkm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fuzgedme.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3snprpxnv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mjonrtsw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3jlgtaxjt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xolwamly.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3tkrizggw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hqbtkijs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tnajdakk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jowvyhnr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3mydechmu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ykveipdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgwyxnen.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3snjupgwn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3uohgnstf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wacridms.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yinhtyyt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3sqgkjyjr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3futffvva.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ybdgvevm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rwyiglye.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3eeowvvly.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rbsgpebw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ozpvglgy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3gdouleuq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3twytaemo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3wmfxwoxw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3nspjgcol.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3lwigztqs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xzkdkrcj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3cmllrpun.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fwsuzwva.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3drksoxaa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3npjexlqx.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3cfugvkbo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xzfbvqpz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dwgvecbe.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qnhoahty.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nduszoxo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqqwrzen.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qaovbpfx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3eaitmxoq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3inscpajh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qfqvgeow.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aeneuvim.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lvfumzeo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3czawukbn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lecplzmv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zutozesw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yvkvatyh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fvjkaext.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3muxmwawg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kagpsiqd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ujwaweup.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3djyrvcdx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pmzmkbdf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sdqtgqcl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iulytbma.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xxiivcmf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yqbuhwic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oztjwqnj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tibwaxzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3taioastj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ympuebxx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zfruwdit.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tlmjgvnn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3laboplek.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3cliwybsh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ksiarhsz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3efnohzxj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3rulktnuy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vbslabbn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ocfzkqgz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3sjpaekew.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ockwmnso.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3faunrhmh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3rjxqlxxh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dxskkdds.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3qnmkttcd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3krredmho.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3koxgefzc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3huwwfyzi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wqwawzvs.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zsepjxoa.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ftlldavx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vudgurft.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eetevynj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3pyxyhsph.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lfkxfzyu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nrnzxpnj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3tgorfxku.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3sghirrfr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3rbhdbccl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hvndhjan.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3grxlssyh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3tvxebdbu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3vixbefkp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ifekxgib.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3sozhyeyu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mqduqbmc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3lxdlzxdc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rbziqjus.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nurstwts.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zwogqlzm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3slomzonb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xynryqol.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ingohrnm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zegzkiui.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wfwfoncw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qgnrvtbx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3midczcvr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cgrkknmw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fsfphzql.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pslekzww.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lfihhyow.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lhtyhjjj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wkzpcnlq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cszftgiz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qizblbwa.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3innsxfgn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3azdrkkyy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3pplttzgg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3oggyqphg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wcwunyad.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3tgkdrsgx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wruxwpjj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3byeuerfv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rnzednll.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lwacqlyq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dihksyac.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3qyngdrvj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qqxyeknr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3obslryol.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3nyrbvzty.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bhdlqero.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yubvkulq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcioasev.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3npxnrnpg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3domlwhdl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmlysxww.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mncfzrjx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wwwnpjvz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3tyznkpse.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tskpitib.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mqpldpve.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3yfqxtigr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3vbgeykql.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kzvpixtf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vvsrwvmc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzwpufqk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3uebmzlye.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3jmlxwakf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvvyxwu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3hjgojstk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3rpvohksz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mgtzadlx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rbqegzoj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qfpeztfb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yytdfszt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3skqujxtg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rlqyxjns.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vievyxkk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3kbbqooet.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3clslptvo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mrztoifp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zmkodyai.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3aouojbfb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ypembymo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3redscyzd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yeduissz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vrjmhkmi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3kufabsyp.html


<!-- 参考信息 -->