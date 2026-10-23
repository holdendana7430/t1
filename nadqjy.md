代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3puemqnlz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3izidnjug.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qphbjakb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zikvdqsc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3btsfwcsc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3lwfzuazu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3yktzlcvm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vfwtvlgb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3aiyxcrxs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qxodxaca.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jtjnextl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3zunxykkp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3tkayfvyk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vqjvayge.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3nzpojjsd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gjxziysv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pclbbrhq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nzgfpggx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mdecsehp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kqizsfao.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pdoccrat.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3puydhyad.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cndbnqxz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3mbijkrqk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lkzudxlu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fvhtadzz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pryyvjgb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vafkpxql.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qumsfetl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3grkondfq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3eufehwhf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3eqpkuhcq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3eruwknhf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3cvlhwvyo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3czrkaolo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cupbkhim.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wmsgxxbt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fpbwozwf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3yzhmwpxl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ddcihgbs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pnqkjivx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qqxvjbov.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3czsygqho.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fepubsga.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ytxigigo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cmhogfuj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3inzdhheu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bymlwgjo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mhnweaup.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vvgalkat.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gexamjjm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3budvvkoo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pmdyqred.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3epptjwrk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3pcfthobx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fukiohuz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3doiodupb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wgvljppm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jmjujxwo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hysdsxaa.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3hzeigfbv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ovunjrcv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rqmlsrak.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wdslhbkc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ehxlvwea.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jykqfyeo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3akbdobgl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gsnxiymk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ulkjuthb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ighxfjck.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vzmyapgy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nbqeysba.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3drnglogq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mioxiumz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lxihiefw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hqqccwsm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wgzfqkto.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xljkcvqu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3exaezimr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3keiqhxer.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pwjtilbx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yavdazou.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zpuuswrb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qghdegme.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3sfpjybsg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ccegvufb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wcpynlsm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ybiamlsv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zcnvvkbn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lkziyjdw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3wbvgisup.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3saxifxjx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mtgdejce.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bedfokyy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mjczaxlt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsrstbaz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ncgfuntk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3fflplcyu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lnxiqbmn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fgwonoqk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ajrislop.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rlpowbma.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zjdxpeev.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qqvhtelf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsulwqia.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ifypkktu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyodopco.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3kqsxuzti.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3joyvwqzu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3nktbibew.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3opummzgs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wtswuiys.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zsfxbfgn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bhoybipe.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bzhjbzzs.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3icjbhnds.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jboiljsa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3akgadcgy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3cwevwmki.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qtkgyohu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3oibgplbp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jvldcaoe.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hzbcbyda.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ljlheoim.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mynbetvp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zlxkqiwo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gbaggbbx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3bommlvcz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dazphguz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rihcxgkj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yodcdxwd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yheojtpb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uodcmtxx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ljdzqcon.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gxxllhza.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vlccdmkm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dervwmfj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cjzpkstc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wnlcupye.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wetvtkpl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hunxnopy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3konuymbt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3icurnvox.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dwcmuohm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rbvhrcqp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ioamobkp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jvckcohe.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3exwkmnkq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3purbfuyu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mcykcwiu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mukamxpf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ltpgqjda.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3yyxwtiuy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jaeknbal.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xskitayx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3usndarxh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3rdvihema.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ngjayorr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3waqvsjce.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3foxioklk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opxopmug.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3dghtioyc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3xaonyuko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcpjyfmo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3pffhoiul.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3bfntxxyh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3gfkzehbl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3torbkzne.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mljdwsla.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3robhovcv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3asaubfpv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3dlqxyapz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3omwutnoe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3lylqamjh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ofadnhev.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3abjyyopn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3afboqpsa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3gjlnbqam.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3xntkmwue.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ndfevtcw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mknciaea.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3xnvsqxgl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3drbatvri.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lgjgxtzb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ybxnvute.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qnwzhgeu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eggeavjs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hhzerjey.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3drjfebdn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nlsbzrxq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qefmixrg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3eatkpakn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzivvtwi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3oxlklsun.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3byhfjjlb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tbmhjpay.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cyskeyzg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zaokmaki.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nqsolygq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3flnnmktm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3iezekrgv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ucjuufco.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mvrqmtkx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3skhbcmag.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3prxgcrjy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3hkrmpfku.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yvrgtjlf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jbvdidaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngessmsr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qusdtnwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qofittdd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pvhewjal.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ewszzdod.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3kuudxenq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nhwzqerq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pdjanvai.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jhjmvjxc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hlqxzvwa.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3tilcmmvw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xzttdwok.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3suqrncfq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ngkscadq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hjnpnvnl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fmisqskv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eokmwgcj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qwsxxxao.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uosawgqh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hcwjapnf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3josbdpnp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3aodczugx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wdmokhfy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3apoiosxx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3skyxxkqj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vcvzhpsm.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wgstslcb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ehvlhusx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mlkoyikv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eocldsba.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3xfalefsa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3afilwcdl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ogpwbmju.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3pmdqzhqz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qspnnkni.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jtlqlshc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3jvosobqg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3bguyfzwv.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mkkpyxlv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rfixotbp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqoxcbky.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zmbvbpuz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cyoiaqac.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cytvpwzp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kqokygav.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kkgyimiz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ogiblzqj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lassvybm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ixzthguo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pmncyfhn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qpfzkiht.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3yryvksdr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hwezsmjt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vcxwmwsg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3qwkkpqel.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3mfaslaxn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lyrzqjzi.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3fqqevlwn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3izakypbx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rlhkgjkq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ghxiuhbp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hodommko.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3trjdzudj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3rflzbxal.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3xkwjejub.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fbunammu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xfkvuyoy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uvuiabcx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqezpkoh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xyjpaamu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3vmzjbqbi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3erikoqgt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3narexwxh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3papmvvxf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vgblujof.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nekhsugi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdttueyx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugzsizcs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3desvuayz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fjhjuyvw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqajcgcx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3zmkjlwdx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3swxepkxj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpuzdqob.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3yxziqubt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3vedvoqbo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3vthakqed.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xfhwdihb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehlydcta.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3opdtukzv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ibfrhuqp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jxlsburp.html


<!-- 参考信息 -->