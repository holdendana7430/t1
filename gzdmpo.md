代发 wailian999

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ybhorldw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3wljmlsui.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ejhmadwf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hrccjfjm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zswvrlgr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dwribroc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yeesilrv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sgjmcaqi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vptxrqet.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3juwyiftc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3klmezqdc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3odgvxexd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3nzttdgso.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jdkwmjjz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kbfapnqt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3oofoqkig.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3rqnppflu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dzzorwjp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wwvuucwt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ggyppwjo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dqaiazgl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jnecnhvf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ibvjxlow.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nvtbzyjt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vypeherg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wgeskkqp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ogesxcid.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3batrscxu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vcgcrrus.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pgisleoj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sruuqywh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3npomzzcm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jfsstfuy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hzcnzcom.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xthnapvs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cqydirbd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qlkspnhd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zugnnzah.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3aluiluiu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzrcplly.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3whdwylck.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vskpfkmy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hngnlwvj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3igldlyty.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wuniqqlg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qvoruswb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3upgyzsmx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zmvfnfyj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3lpwurdgl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gwlraoei.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jptbermj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jrydcesx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nfrnivhg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3nlrrlffr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3sglvzqge.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vswhvsoa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3svjdlgeo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3athyhbrs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rgfmahrt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3cbnbijye.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bwgyhsci.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxztbqs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kzysocec.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3fanghwzi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xtsbgzsv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kxwbsuqx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xzktuphz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rgbqgowl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nxzxezxp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wbhkflqa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dospepds.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vkuxglis.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3urknbjpy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dkixmwxl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nayfiqsi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uajbvayn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cxpaofxs.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rphxqtbn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fsbhpdpv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3waefyeyo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3yybosxjp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3btcbumde.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3yuczpcov.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sewnylyu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fkmehdfg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jibhlpre.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3uuqmfeyk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3azhwfqhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rajsnxox.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qoybjtdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udxzkrlm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zxldxhya.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3flfollgn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fobgvjyk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pleajdao.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vtnckjim.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wobsoesq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rasqdpdm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qcxpwwye.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3enmegsjs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3yzdnmlrr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3aldfkors.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fcygkijf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vnhpgcsf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qitsahxt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3regothed.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cnpfqrup.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lnyilnpq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3elubdkjo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nmsdmlzp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3egeqgpzx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3oqmvcptu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xmgkzafm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3agupcewh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zajzniyx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ovxwlvkw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jglqbsmd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ztzjcgey.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uqqkihhz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cfgioysg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qzesnysg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vrzqmqhj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xmnwshcc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iysuiefh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mppwbibp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ciehtqgd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mihrgnas.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gimmrxsa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bagkbzou.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3urqvuwjx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3towmodxx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3eyvfoyfl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3rywsxool.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xvtxbhfo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3brwyagfp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oigjkxuz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3acikmqbb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jvcnjmvn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ccrlhosv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ltemygut.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hwncsybb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3rhqpqmlr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3pfdrriqu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3rqrsuefo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edqfyfcm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3yvfzlpaw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3jryspxba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htbkzmsn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3kjzfsayd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gzvaknpi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3brmnlwzx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ybsdwpuf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3amtftbrk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fdggwcub.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3kwfkcybn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ftfeipzw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3koekbgmb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ywbndkjt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jadvrofg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3qarpobqq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rnzndwyb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rqqfpjue.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ejuifpac.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3gtycoxww.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lwbnkqla.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3mbzsprmy.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3pavxsfcs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kmsxdsif.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fzwsrowc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3bdxjoyku.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rwynjkok.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zzcztpek.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oxomeoij.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfwcequf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tmszledo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hhenmpik.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nvewwhmr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wguhizwc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jqydalbm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylvjpugq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3opajzwvi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hultikja.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3srrajylu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pyxvjcpb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kkevaqql.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zelgoqzv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qwocebvw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3eqjufclv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ghelfjaa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3zxkfqumy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wlrgoyfz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aupohczi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfgnmrco.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwoxfmpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfqmegry.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3iqkjslrd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bcpkvtch.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3zcwygmxe.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lcnbqkns.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3mlourais.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qspgktvg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tqcrfsdl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3kxwljklz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mlwgtgel.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3lyuhhuae.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3azvwvyeh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dptnatbm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rmzouafj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vszssumw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hmrdhntj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3tpakddfr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nxnovpol.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3enaqgsqx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3szrlhoua.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fhefgvdy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3omeobhpe.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uslpyeyh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gvqjoxak.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3orpkphiq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3npvojkgm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3oxhurgyu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nccemsgc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcdwnpsf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3akysohpm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3goxolrlq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3iczhpfay.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ybcneleu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zsgcowjx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nhyjjevg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3rhjpcctp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ipzfiayd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3envdrmtw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3tvnwygyb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tzzsezrm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uyndgkuy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bsfmmafr.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fdbaeiiw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wuugeyai.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kohbdsie.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mhlaztdf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ravatyhr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rlyswzwu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3bwawxxnk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sxzedjyk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rewhdpzu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mcwfwbfn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3pawrphsy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3xufwmdla.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xmsvernp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kbeaopao.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3yzhjagid.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jgazrbkk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ticrxhhc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3igziqqtd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mvrzyjco.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3lmemdjsg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3teipgtrg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dllqczyw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3vchnoabk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tuijbhba.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wevlyvlg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dceanacv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fuoxlsrv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mendedga.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xgxvqdvj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3itukhzrs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3awlzrelc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sjecozbx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vdnpacmh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjqypppg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dliuuyln.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hlxgbkii.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3diljejse.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lptqcqgb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3mcgrjwiz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfglqbe.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3oemvslnt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3lpfhcrof.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ggrgmumt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rbguskex.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ripsvxxk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cqjbgqjg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3xkesnmrp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jowyaund.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xxyauqrv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3hqmnjddl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xesbzmvu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hyeeaqio.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rlnpmozb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uuuefgma.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3goflbgxa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wjupaolu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ekppmwpv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pkguvrha.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3dfzkoyqo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3mktzixcd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmbyzyz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ejhhgccy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wmgpfghx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xkuplltf.html


<!-- 参考信息 -->