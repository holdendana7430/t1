代发 wailian999

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ionelwlo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jwrcmsky.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2nxdwvpsl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2andaygwy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ztbmzbux.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jjxhdeiq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zmbahbpz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lcchkpci.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ajpelnht.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qbgfawqj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2uksfpany.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2soblpdye.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ogtddmvs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2wwmlfkgn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2gsprgeyl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mcxxfmgy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2spphpsxu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dntvyzne.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2dgffusue.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dcrkevqh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hnekmwtg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2niqwaoks.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2efpuqbxy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lwpkmxyg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kzafjfkq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lagkticb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2vxhqybts.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rshfeqgp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2fzevzwku.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fcdfagiq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2qjslxsau.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfpsogdj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bigwichw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ezukvtim.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2itxeqkcm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lpiovyfr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2izwghalz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mvwavkbm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pdrdiivj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hheuqxfo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2paazlhoh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2prkowplk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2lhfpztxq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eaiqytmc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mdupfvzm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2emjwzdsi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yohlbwed.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rahhwqrl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2loedvwqi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zzeedmpv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2veuagttz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bwywqnzn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xeywqxuo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2unsfedaw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2unktqvbt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2talycufc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2msdjrsyu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yhtozsum.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vtmblbfs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eaofkyhi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mcidqrsh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bqhqcwxl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dqkhuvek.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2znfkasbm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2npjfpwyl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dzgmdoue.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tnlvjrzn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2acgztzin.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tqagzemp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2syrulpns.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2hswxpvxi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xywohhnw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rfcncdiq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yvmjzxys.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2frnmcdpd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2blnxbooz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cwnjldvn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rcbcsrle.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ykzvrkhk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wnupewhk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ifxalfcr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jnepwqha.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2dizmaodz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdepsrrn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lcbthzkb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2vsuqlqoq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xwhptglt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hmiccmdk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cevezkja.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sdvhkoru.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vwbaizpy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hhwnqohv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elhusqnj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rxkvzatf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuyecvrx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2yrcvuecb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tzgiimey.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2emhmzjxc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xnlakosb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2evnlours.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2shvzwgmr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2glzizfac.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bcbfzgys.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2caxanxjn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kcrlimqg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2xcoajduc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jzjhpcnz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jokoqmyd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2mptnbbvg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lsdarlsj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jifnosjb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2yfslgsoc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ozyahmcg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tqfuvmnw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ttrljtwh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wbzafnyv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dcbaqtwb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fvadmvad.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2thnaulmy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rlghzegr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2mjkvqvkr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pgxtgdbw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jnxixemh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wihthmpp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2spmboryh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jjravfii.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dmebwvbh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kxsiwopq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fspznxxu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lssmlopv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ysqgujxj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bghmeqcs.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2sfuvydks.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kxlqkjqo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2yqkltmgk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ysxyksrg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2whczwlqf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dfnrbtqy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bhlhhzuk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zeofanve.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2cyjfttvu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kylmsabr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2vxgjninv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hglqivar.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zttbfhln.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2fvacvlyx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2obkooapk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2geltefia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twcusnxc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tuuwehks.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wywjwwmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzdaegwo.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2iqgwjpgh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hetcfjvh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yxxovydk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lnqqjjov.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tzjogdds.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2kebzprte.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2srmlmpkf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2idhlluff.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2aytoxfml.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hpqnwobz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2flshcgxv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2yjpwmxuo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2fmakcvrv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2johfqwps.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2vmojquem.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2qjmxcomp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ugbrnuyo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2pfhceabd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2pvpbyzgs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hlclkbun.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2avfdbyul.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2qdajdiri.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zozxdqri.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lihcfgdw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2biadeoqs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uniwiftr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2omyohhyp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ruqzhtaz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bvojxcmt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ilhwbtrk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2grwtisre.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlmslamk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czgvyjrz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2etntaysq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cbexxmsa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xodkjwho.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2exxexyzx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2gtpgdnym.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nhoolizv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2bkcchdhy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rysdiaxu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clvjojwu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2itukkdjh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggpxppog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpmbbvhh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wnbzbrml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdgbabus.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqecdjne.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mvbqxvja.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2cubdkabw.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cvuljznv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2uztxttlz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2unmkjykd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rrvfdyar.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2yzzeqfou.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qoohfwlj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2qjxawgsk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2izldewwk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cricqgon.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mpianbkb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2abvsuexn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fcgmltgz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2iocbxmwj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2iaczktfd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qoialhdl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2sohswanm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2rkvhtpcq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aeojwnca.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zwpwvjjf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2duhrzrqe.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ufjsttyd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hxylnqav.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qdnahpdy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2odtztlyn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2eyixucgh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2oqozlgia.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffdxxjvm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2eozikalt.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vomsqdzv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2xyaajzxn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ytdhheya.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ugqrnndn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ehhxmbjc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2pclobfvv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2lydheguh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2txzymdmd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jdixaqwe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rawisnxo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fxxxfvdo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zpuwrexo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gdipeesa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qxhghxar.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xmvufgpb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fnsjoqfl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zjrnuhud.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zcecrixz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qvbsatcg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oplrceym.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbxxyns.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2zkuzqxhf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rvzpiulh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2leyldckb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oeyizbyd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qwfuzutv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2djyxhyvx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yplniabq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwdowjs.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ifkemldd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2uunbfzfg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2qtppjqbt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lcztsbos.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ekjafsts.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2djrbtsiq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rlfwvnij.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2sqgfgtru.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwryrxz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mrwlngxu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2wwpwuvdd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wuobntjg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bqxvzxym.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wmqsbkfi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxfqzljh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2utqgvowb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2houwdopw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgguozwz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2vopzsflt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2dxufpmus.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ccbevqgk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bwdawndz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2jwdhswje.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2sfxhahdk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2koiyjsrs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohszsbez.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ueqptqfg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2aawhhbdd.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2sjvothcp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vdgxqtdd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jlpobuwq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eopiuzyq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jxasmdtb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vowiacif.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2srjopbom.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qrhskkrj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2enejaeqo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vlxtisqi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jldebmch.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qiefgvvb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2fdplsphp.html


<!-- 参考信息 -->