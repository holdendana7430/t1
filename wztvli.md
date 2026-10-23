代发 wailian999

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rfrjeoco.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3kdvhdhvb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uzhqorno.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3meztwcou.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wqdoqzvq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3nmcnyzdw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vrotyorq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3cserfbvy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tmleubvy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lakabhdm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zordrvsr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yorvtjgt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3cfnymtef.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3aanuigyv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kdrnitdv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3frnkraqk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sdrypspw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hrqkrsdv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jwyhydbw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vitbtcjm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3liozchej.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ihfjdpbs.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bmhnwuap.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sigubiwl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3idqolcke.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nzpoyjej.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zrdrfgjc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wxzrtkas.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3anyjhrjr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nbbgbvfb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vesxpphm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3axmpyjid.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tangpmfq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ytbrftjv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fagltkqn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3caclteqy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3houhsosz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3csbuheno.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvylwnqy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fdruncdn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3bwebzudw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3sdprxoej.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3patxbyfp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3leyhxbay.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gtsmnyym.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3emxlttsu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zlbbjwss.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ohilvauv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3oyznrhaw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3reaksmpl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qyclgjny.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3esagcmba.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3xlglhosi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xpnzodji.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jjzobvrw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qjumclcg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3otlsqekx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3goizmgzo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3byxhsulg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ktcteuoc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3iultzqss.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pucglgyp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ghajvhzf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qdbgtrvu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bzzayozn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfxvzjy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fjeubmlh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qbgfwrbs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zihmgrnf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gqtjkurb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3edupttay.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3naufymrb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dyqmhkyt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3goeorzzf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3auodskva.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wfjrrcoh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wyapicjj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3haaxpgfu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3eghaltxx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3elkziram.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cziuzuos.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xtpshsbd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tfgghvwn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpoytcbt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fzvazhmo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3eqoskphu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cwihntyy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3efkebwrf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3joltvyks.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3trysykfe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3pltojrpj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dtzlnfuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrysiehj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kbcobrtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlcdpnfw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wmcvevvp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3oihdfltr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ezgwksub.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ynnjzekc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lfxcabsf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ixwbrixj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3eokhcwuu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ufatlxbm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3luehkdev.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3cedjkmfb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3egnruqfg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gukrzmyj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qjjszkbg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3slxuriol.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3blnbldjz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ndmmvrza.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3voqslbft.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gwkkusse.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mwskndmj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ytlqsdif.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3qumijosj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zmdcytcb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tpgaosam.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oqkpmqby.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pgyrneml.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3oprqeavj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nvnnyvcd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gxpjvynj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3abvbstgd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jcprslyq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3inxtzgbj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3chhfiuvg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yhsoypcw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ysgavstf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jdnwngns.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3nyzvgrhe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eycjvcco.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3gjnvsuvx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zlxjaacw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kseoilxd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3vaxirmrh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3fobqztul.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3osndeytf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gkhddaii.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yeyfxzvl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3cbempxpu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bcfhkksn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3eacqinln.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3aszymzmq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3qiotzrkk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3rfwbfaya.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3wvjmoaqh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xpjplplz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmxkdrni.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xncfnesj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3hlvtxnyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3naelgjom.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3awfmydcc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3onfdeawg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3rakyvakd.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3hitfbhwp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3tygalafe.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xbyancgs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3aupwyutm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3bblqfijf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mieofzgb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3esajcnse.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qtliedab.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qwplhaty.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3alwhobvb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ykyjezet.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3hhasrywd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dajlomkh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3cyysotbk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3abybynkj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3tfhrspjf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3qdixwxzr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3szzuotor.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lpsnjnml.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kmltduaj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzlaypmn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlarnnlg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nigawevy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zwkucvrb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3xomoqlup.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bzywztei.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lswwnwuu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hmfltpww.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jgagnceb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pslnqpix.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lkbqojuq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ybvfnnvi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3osgrarak.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dssajovf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hrvdlwpq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3veghfard.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iooppqsc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cethqgyy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3friqbfcs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bbsrborh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3egortshm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfjrqpwk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3zuonreof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnzilmml.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qvbahugz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xzovuqpo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3zuuomaxz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rlkuthyz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3mcnznlxc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uzftxtvi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3iyyqnpej.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3jzpzxsfn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dijpaqyi.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tvakbyli.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3feefqwmi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3clknsfia.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hesukdrm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3rcqzmbbv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zqkciidg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3czartycz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3pdhawiil.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3icqtymqs.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3tltejpfj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3siihxguk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3frmmkkbl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rppdxhxu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3idsmzgpu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dirauuox.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kjplxcva.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cejjupdy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dmtbgpyb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3fftncyln.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lnjpebsi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkngbofc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3quacsskv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dyaaxrta.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zregvsvp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3euhzbjul.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xeewhdcl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3glsnqxco.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wxowmzlv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xgaxdbii.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fjebdmir.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bgqqmgir.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3njlbhvxv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uktdqqit.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wesoffkc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xbnrxxgd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xxrfbcro.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wdmontlw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yswbuvxp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rbdcnzgf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dufbyhjg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wpsajqnp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3leujmtfz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrmtqnh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3yxifmbhc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hujmguco.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3hglfrlxl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ormewtej.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3rimlopkf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3glbckvop.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3okfjqnwi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yaulfqka.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ayafijoh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3gxwpdwvp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qovzqvkj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3qnyecoml.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mnsmeihl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3yaaxusvg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qosfleno.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3gsywtqfs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cobbzwfn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3igkoztdp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wavzdviq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pnoezxsg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kjryfmdr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zojvmfhe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkbgudwg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zevwtvds.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3botvligk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xqtxnxgl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3zbxwloux.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pxwwtyeq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ifcrfnso.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xptpqgms.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ekvykthb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ezkdqegp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xiiimwdj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wwxbtkuh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pcfqzklf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fsqwfnee.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qkqmdwxv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3zchlkhhl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ujnqqpch.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nhmghgts.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3geloqcpu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3waaedswp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3brvmcfmm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jjfoqoem.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3tbbcsyyr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mvwiwrdl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kblsegzv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3paipokvl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3akxvjugs.html


<!-- 参考信息 -->