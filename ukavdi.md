代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2yetcqriy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2efzplfxi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2cyoimgdh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2xvlqnwoa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ljavjmwj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2umwnwscq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2svgwieli.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2luoaylpc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2yxlbfoeq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ytyuvqyv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kswjprpa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ctniivlb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ivkcuzfx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xcsneawv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mxrnsfvz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ugosezvu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2qlrgsuyo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2oxokdozf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2geufosek.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2glblcvyq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dkbwlnkq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2sbkptywi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bedpglhw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2kxrmbpbr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2idrnevzz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2etpbtljj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ywmqznto.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2srijsbss.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rpafmszk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ttwqxgpx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jgejygjo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ykmexvag.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2idcklqpu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qbkgignq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zjsvvgvl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fmcceagt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2izcowdsd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xlhvuivi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cansucnl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hfnyxlbc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2blhooycm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yyobkeea.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2yphojief.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2owexooio.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lfaomajm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2czoobwmp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vlxcvpdd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2warvhadr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkkhtdcb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jkhdtosu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qzojohmc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wmzzignq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qwakzxtc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2bmxxwynu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ubgvldkc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wmvgturp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zbondwbn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pcbtsqjn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ryhgswhh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fmbrhoqb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kcfxtxpc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hsrmypdb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2huoaafzh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2iavjqjum.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kdrxgvmm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2stfbriyp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ccdzpwny.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2moiytkbd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pmraplix.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2mmiowzka.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2oeotcgsf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jhdmancn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2iobfikov.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2eatywxmc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ejgocghf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tgbvauao.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ydrlrcir.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bddwyicz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ehhtkjzg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ycttknrx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ktncwwjd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bgbimvtf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bedjcbix.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qkbdbbsq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lvwksgmn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fqlvcstw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2bbtnhfvs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dtpzmbev.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2rdcndmsc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pipnsuzm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hetpbuss.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sxungprj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mxflqhcr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mkkddpgc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qmmieteg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2urbzkmhd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vtjetxxu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2lwcrlagv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nnfmlize.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2yftukvvd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dutkkaht.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xkplkmdp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hycufqdy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2lxzlzksr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owlgixlf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eijxwglz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygexrpkd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zjpvaqps.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tpxofzeb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2kuakmdqh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2gbjkuumc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2bwiftlpk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2prlibzok.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pfbairjs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dcbhyvvf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2thxpewwa.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ztevfvmc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2oxsnlrjc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2hsjmuahx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2tcqxfohc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2afskuhuk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kcsqeqzo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wryemjat.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vejumgwg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gbnactuy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cwnnjuqk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2clfkousq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xzawbhds.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gvaswxof.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vygxictt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fcebjbya.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aeuejmwd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2osxqtxtu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wrsqexvi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xwloomsx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2snsoxczc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vqclaleb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2djgymqct.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pokafjvw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zjrhirkh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2linsmbks.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2sqyataoy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ygndumir.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mdrtubky.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2womswcyu.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2lzguzfti.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gyhwdsum.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vyarbvto.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lrxmpkpf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mzzfwcyq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hiwyvwbb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gxnhfhvm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ufyyqxjg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iyigkhqd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2lqsizayz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2unssvzue.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2rajizqkg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2tcokrvbp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2gvrsanrv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fcdirkzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oraccvws.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2aqkvyuwx.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jjnijqjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tomgavmk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2dkyivsgi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ragfdepz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2goufybom.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2frfdmkhu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2exmldknx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2poqpbcre.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2cizbyzhu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2jfwomxxg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2mrzubsjz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2dhotknnv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2wyqmmzao.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2qunpzfjf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2eqyqxsdj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2tcrqijss.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2fqzbypel.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2cllvlqho.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2halodcuj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2fkcfbzlj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2kplmsfgq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qswmheav.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jeqxgarz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2mhebuhks.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pztqqpfj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pxvhxktd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2koxfhstt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxboaysu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zvyfbggh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uxduylkt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rugkbgwa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mwczspua.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xgtzcpks.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iuhpbgzo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rymmfrxw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2orddcugf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ipsfnfsx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ixyhmeod.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wsllyytc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wpsunvni.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2flgymxdz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ezjyolgl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ndwzvpow.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2etysxtjx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lpdmgfsi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hxvumtbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blnsjytf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2nsjwtqhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqzmljvj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2fnvggbyq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rgcajumu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2fvavnpbc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dmwniovz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2kfygwoah.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gtepzwqc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xoswaccn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mnzvtwpk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cqtttdas.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2qbbyabpm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2fovsbowy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zccwaokz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wtkibocw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ugvhhkqf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tjcvggbp.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2dgnvlxqv.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2buuqjpju.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2redhlepn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vklfswqx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2palmjemh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jvwwmwpf.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2grhaqizv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eroiqius.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qrnzzrbn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2friwrrhj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ziwyqskb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gitoqgqm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ppumomka.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sdvdeepv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2froswnsj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rtmuuuxg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hqbrwoub.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2xaouvhyv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ncopnkgo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2wgkkrpkf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2nzvwiihv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2sffjlcja.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2hwtlopso.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kbgdfxfv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kwueutpa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ttqfvdov.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xtsavkrg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xpjjpqtt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ggqnefny.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ucwymqvq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2sgytdmti.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uppgnzns.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lrcuxuxp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bxsmigfr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2gweffeux.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zrxhzpkd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2irlbvkqb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ljpaxmse.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xbtxobrq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2wuhqykuf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yfrpxxks.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kipabqfu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ppladzks.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2plbaaaki.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pulplkvr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2khgccqwm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ucwkwpnf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2phpvcnaz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qiulvfhf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vpcbduwt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bhyfrnrs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2foyvypiu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vppisysd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ihxkfdtg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hkyfxpof.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mcjtigxb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tiuujvrp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2blgychpp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ddavslih.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nknqnhdw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmokfpac.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tywjylmv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akwmuzgi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rzhjenno.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2koehahzj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dheohsyf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mqzkuvlu.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qwfeazsq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2gvoglawt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qkzjxcnr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gsmxglvl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2craluoke.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xsmlxamh.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2psardqvu.html


<!-- 参考信息 -->