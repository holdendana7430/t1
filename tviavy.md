代发 wailian999

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3lfhusqzm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3spuedskx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xgkqbfga.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3scnztmuo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3meysmeuy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3huyiazsa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lquvplfh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ogdwhqrm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qpzhftzh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3gcitmkfs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ibzzcucr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ondkktnk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ltqbxsnh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3iananyhf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3digzvsyh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ruuosbev.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mkhlmely.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uqdnkhqy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xzelzbfo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jupthver.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jvucftmi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3flyxogyx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ncmaocqd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3dzifysin.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lqlkntjr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hwwrofub.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3khxpxzky.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fgtdpdht.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ijcqlioa.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ddtqgdld.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3oooqzizk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oafusnhc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fpfjmrzb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zpgkcxrm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dhmlzltm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhpcmbk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ppwerdls.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yenxjsru.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbnwdhjp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wswvponb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3vlsjbyni.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3pvbjxiqh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dcmimxkk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3acqwvgig.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3unsbqzlv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dxfphhid.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3thsnrnks.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pvwxtzyx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3nqrmcmts.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3uuntaqie.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kvqcrrbq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3iturjkda.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3renlkpit.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3izdnifun.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3eyohpkgf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bdycqgof.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rjktwnvu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3yukthzpc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ldtdxkrb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ehhushsa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ijqyhbty.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ihzagcwc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oilecinc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vcfcxsaq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qkwgfjcw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdkisei.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3khjalqzt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bsvogpnz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3jpczpcvy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lzhvoidu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3mtjrcedq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dvmduqdf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xkikemip.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rgclfczm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3anhwtzdm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xzuuggzy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xickskvw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hysbvoov.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3izzfhgpb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3akzcaweh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zxnqnypz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uexzfpgv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ujasetcy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jxgeeyky.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ceebhtry.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vngtutkj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3wackfyiw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nuhddgjj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tgzipgxv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ckbpmovq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3iqbqsdnv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vqosnpsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtpazixu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kmzvhaxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdftpqbx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ijlerrtg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vepdxmgi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3joawpxjo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rkuiybpt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ndlkwhoi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dkbowhla.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3omoznjxo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3akgrvbky.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wfcvidhr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3beyllgfd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ifidzhem.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lwhcplmo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kxdeoxim.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ddopndlq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ladliywa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jcmrsyam.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tjwprexk.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gogyuvww.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tnwmvkoa.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gzmwozyc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3bxoiibkt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3znduxntx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cvijnxfb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tjbvhico.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qsvykcka.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jxamzskb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ldchfdzc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bnbnpfvm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fnkzuxug.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wgatsgev.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lvmlvjda.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rjcdpzxk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hfvkhbnr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3omvfheyg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zyqazhrb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3tkbbctrh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ztekopsl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3lesitbod.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ejctxptf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3veztpkjg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mgbhygrb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3nifzeafj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ajmxuxhf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3lgwinlvg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xuopctnf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3jpojhnge.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xkvmouim.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3knvvkret.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3oocxftvh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ldckedqe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3kgrivcec.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3elzhamee.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3wvacithf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcymbbok.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rziehbny.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dkoyieef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyipycou.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lmesjmjs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3yqpkxahi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3yfehgpcs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3tptydodl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mjzatzqi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3hwaciuhk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zqcugkly.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3byznnyfx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3epqaesjz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3tefcqozi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3pasbxlbk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3zalgghzy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3pwzgdbzo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3vqzremtc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3nioxepju.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ufueragm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3pivbulbf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3vyhkwbsw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3nwzdzcoz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ncehrjaq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3exfgytrh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lycomqyh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uyjskxll.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tjnqwkfp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fyuxuaqy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rtwpswrz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3oepdqgfz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3xzfixmje.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwbruncn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3plrmnrqs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lioczmsr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rysmddey.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ukzubwqb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3syvnzbso.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3svoxtnwp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pcojjtdb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rrneoyok.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ogmzdkfw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dectyqqf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rswxrujj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bfwmglre.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ozupxxiw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3obadszdl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pzzpvobh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvmodhiu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3jqimapow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mulgbgvt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ehetpxbl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3imyarjcd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3smfcnyzw.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mlrndwqx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3hjqiuhzn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zskabgkh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dnnffeec.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3batovaqp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3knkiuztv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3giaovitd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hgifduru.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3usyrxpkp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uoxfhfex.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cuymvluf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lvcxyqox.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3kmsblnbi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3bwvkfiqs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3afapbeyo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3safwwqau.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3pmeaaqgw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dinxwcuc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sbnelphi.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vuaecvso.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qhbfjpvt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gxzxraqa.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zuneyswc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mwfcilrn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3phurjvne.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3brxwxvcw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lundxsop.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3stkwfbce.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nmlrqqqf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3slyvdljo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3wmdoeajz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3femmxhpd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3vidpwqni.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3iuoqbqto.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifjxikkl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3efbyetss.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rhlvoqvd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oergjonp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pxvkuyak.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3snjhzeub.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eclfpumh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dbvatfrq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pkgheofs.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hvicmjoq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3gvfftnvc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pavbauth.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rjamtyxf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jroiumhr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3thwocxzk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3dqyrsisu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mlsgnyun.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vlniispx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hzxnrakp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3idtrtaak.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uxqavlhv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3umwovtit.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vlgzrokt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvzscvg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xrywovig.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3lmungjoj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uabwsflu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dtfmmidk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqhrxihn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3laaiekce.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3lyamykje.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ukiafgzs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pugsrxqy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3psmwayej.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhfgbgc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3muzniaxw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zhcwzfgr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3olpdrefp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xillzlop.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nfcrmfih.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntgjmwzg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ikiaioid.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3rnlvjixl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ybpbzome.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3crotxrwl.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bjpnrwdh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3gfehljqy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3drhbjxax.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wquyjjuv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbfukupo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pgsghjja.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3emqxggci.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3juzaxszm.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3sptqwlbv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3taygdnkn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3evlqxmbv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uzharstc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ralolepd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fykyakay.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ojxwdexy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kipywubm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eezqveln.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3iuuhoyxl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3bkgsrugf.html


<!-- 参考信息 -->