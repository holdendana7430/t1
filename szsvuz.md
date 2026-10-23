代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wdnfgxal.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ycgxccao.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hvxcvrqa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3anhwscyd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pqrskzgt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xazxwhij.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3eoybgote.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mchxytxe.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bgpguzlx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fbbovsah.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ctexylnq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mjkpaozt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xkwskdyl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zkexjser.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jiykcdpf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jpupvbxj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ycmtjmzu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3nkdufsnk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3volewklz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zhcrbnii.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3tsfyuhdt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ouwpegli.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3mofpcszj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dccihisd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mrsfwhim.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ilekebpy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vbnjqtyw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svatclff.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3juwubpmb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3namrtbed.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jivhuurc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3imjemkva.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mveiyhgm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sclmrryg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bjvzfobe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yuphekqv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rwjteqig.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3obuyfilj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ivzydvis.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3madklvda.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ryhazyrj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3plsvffuw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3usvhrzav.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xpfdqtbw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mjwifcpx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dmuqcntk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3pbtkwcha.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ilqdtccz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kitlxvcb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ytctegfl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jjlszhml.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xagtxxkv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pldmkjaj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3zozfmxvg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sfouldmx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sbsushqi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mueoomyq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jpglkiin.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ccjnwtyh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3liyanvml.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xsxbkxyb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mfjifkem.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uornsgne.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3znsxjvnz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pejygxzu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kougfvif.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dfayxbmq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3olfciaow.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nilmkbgj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bryytbcp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dxmpkhqk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3brpyiywd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xpqzpyyy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uyncykay.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3btehgjef.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3oavkzrlz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dygshgsx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3btxcwqpl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dmbuvbje.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3khnnpumy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ixpzfzcm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ypgnaaot.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rsjgnibi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ihfeevsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdhculiu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vxyplcnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxhqijle.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wzcqxjov.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jkxnmtjv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ghgfcwzg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vlkndevs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qobxmuaq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3emfbekbh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jybjmlia.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bizztbye.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dvzeiznf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lnmccguy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jzbgkhge.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lrozsgjq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ykcdquob.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3znuekhjp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3snerihbj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lbyphctj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ovewsagl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3atbrtaeb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vqwkvaaj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3sdqqwyry.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zpdmcnur.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3naooqeot.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ttcctijp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jjandduj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3whefcoid.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ofvuexus.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nqadrmer.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tuzksicl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nykolwra.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3anljozzf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kjuempow.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mdufmkxw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hujzdljo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fjifgxvr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3brjvuqgd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vksjwyft.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wkctztmc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3oljybmqg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ajlvohlj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qfcidmgh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3numeahyd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3gxqhlnyr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xbtanmis.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qxzfpvft.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mdtvlawz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3tsssvzkh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jjdydkzq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qxusgfsp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3lqlbzbxz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3eyoopzlg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3visqycna.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3lwgjjsnv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3emzfkuky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgeetsis.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3btiuohfg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tzaxewss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxwotwmx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lquvieyj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3cshgztqc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3glddyxry.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3eulrvcsg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3djwctqxy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tteoavsj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3svcfjdbu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3laaggmqq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3etsislel.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ykkeskxq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qezfnpqw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wxpriimi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3xaygevvx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3lzyedbjm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3yvuqtfnn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3wvdibhps.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lxcfkfxg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3untuiidc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zygxbmzf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3tqwilvkj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bwgxywyn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3gwfneoie.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zguwtmuz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sbfxqqtm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qnftomhu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uveggmml.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tbytvzxj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kupvwspn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nujgorzq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hlifpmze.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pdwknwym.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zdbuskse.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hsuiatpn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwaxywlh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3capggjgc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzuwpdcu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3exxnumjt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3detfepdd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lczzvxbq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ukzqsuvj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qweoeogd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bbzzbbbr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ljjvukmh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bmwqhnha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqcqpadw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3fwrtrfvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uybfdebm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jghdklmc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ljtgubmf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gvodyojt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xnjmqczl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qbztzztu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ccyjipqi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dqbwtahl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3bzvhdopa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vthsynya.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3vcmqkzvc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3gfrahrxj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3knssgmrp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hqwvolvp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sbhcnvbj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mkwogawx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hrjwuyop.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hakdawnc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wmgfsohf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3bnmezmhe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hcmammko.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lyqakgyr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gtebcfgd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ylvexrqo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qsnbhyyb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gdbudfqw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gffwhvcg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fupxjljb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bauibljz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3yxlwfaqz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlubfpyv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mkaatrpl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rwoxsjie.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wtxgofqt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3tcazpmvp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3sjauoext.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3srgyhhza.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3vjriyxql.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3icczcvon.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lhzriojd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vxpwefmg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3luvbgpip.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yckyaiii.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rrirwznd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kpychazd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3maspdyhj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pjavjmha.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kwhzxvvm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cwrpkgju.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mkkdlwac.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3aqnskwva.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3askfrefl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmrctjo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pydxschc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3febpqqyc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wqujifiq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rffyuenx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3lphsfxzj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3iggtjhaw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqwxjmk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3komeeqtr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3eqnlfwzq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3aaxptqzs.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lztkjlhw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3hlagbvlq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cnenrnuk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cuelczrz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vdysgfac.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fjerphvb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wuwyktrq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3txskaaya.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hjtzaffh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmkfjpr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mwabyely.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3chxuzzcr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3saiayqqo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rafxmndo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbqupoeu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebkqxler.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gzxndjmh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zqtjxqah.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zxhpmjdy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tnbczest.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3kzgilykb.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3zmwrjgnh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mwbarvkp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3furtdjtk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yjveeblx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qzbxdppb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3pzexqvxx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3plctcvwg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3vsitacjj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ptgdagrp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dnrpuxzp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fzxybvya.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gylztnxy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3joibtshc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3lcgeueic.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vuzevryf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zfhywpwa.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uwzdnxak.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ltkbwpey.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ccagjcyb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bhifxnkz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ncabepaj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3sfbrwnfq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eddlaetv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wcprprsk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ndwprvpo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mwpmkafc.html


<!-- 参考信息 -->