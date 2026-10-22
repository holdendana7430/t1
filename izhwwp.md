代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kclxbeoz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vyxzpvbn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nypxeayi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2iwvfucja.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fsfifoef.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2htxayzem.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ihmfktog.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2sfbbuydt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2yuxgxboy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2eqyofbna.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zrcupnmz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lhgkdeae.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ayostqez.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2etnkmive.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tyxxuxan.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2hbxbfqnn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fbqbvhhv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tgzcsqyp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2quzeoflo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2yfsusivc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2awlvkitz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2drlnxvtl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lgiakudj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xftbncer.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mavnymub.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2wempcwqh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2isoyvutd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2trxhfrez.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nkiwhstr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pbfuotio.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2nviitxvu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2hepaybmw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nzsdmvtq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qaxdmtwp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xpoucjeg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2becjioot.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2sgnhnoqz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rxtdttln.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dewgymup.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jkeiwxxt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zevsqqmb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rqvzfdzi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mbtzggvc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uwiwmexm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dzsucgok.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mbcbnxth.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2kefeunbz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vsbrjlni.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2philoymj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zoemhrnh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hugcmbdq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lquzkxam.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hukxtski.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pbvnhbjo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wzbtweld.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucevuqgc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2hejcvusz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xbcwfwlb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2joxaadtt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2cujijcbr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2glhroytk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mbaavyzw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2efqbldbm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2brbofqlx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2oxyadvaz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2dlpoifls.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xubrksgg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wjoemlos.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cqvpyqid.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2icqwicbp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vunwlscy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2czgzdiix.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ntbtandc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ypbqrgbo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2glgbjjnw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pgqyjrxy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lpeurzva.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xccxueqr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dqlhzvur.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tdtveoty.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qceecchu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oogokwkb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fxqdhixq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2fttbxxlp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sdebfhwf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2oiaetlyj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bmpjitbp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mhklqxpr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ydrxlems.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pttkyzpn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jpwchmkm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zosisokn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dkcunasf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hhybvvpq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pjngffdo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmejudhb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uskoepqx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xcpvpici.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2lijpjljz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rgebbnwu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2exszjubc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ilwvlttz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ifcyfpjx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2uefpiojl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcjdvpou.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mngwfoyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhqxnpyg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2juqigole.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2eqeamktk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnalgs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cijlphsn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gnlckjwe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2edssjbva.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cpeliwtj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wakthepl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lqwgtkmm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vdqskybs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vghswxow.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2adtwilua.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2oqtqkpcx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2xirducev.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lmaaizag.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vripvjkl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zalbkydt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2tlcelecs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ptbwzcbz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2cmjzkrxl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jhopbtbv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mbakvomm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xphlgyww.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qaskhfxr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vtekjrgp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xkceqhei.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yzucawqc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2aaauvxir.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2avkedutt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vnxlkklc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pifqlqvh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2isvrizqf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hynogcar.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cweptefg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2eysladan.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ewdfbrlb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cntcbame.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ktyxhjbj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qrmbkxoz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mxmomryh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vmgexupj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2helyiiii.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yieocvst.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dmbgaudc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mrstknml.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2lsvhrqrg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ojliintp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2asaglkou.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nxibtauk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2uorazvoi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2uwcaequj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2mydlnpvo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vrhsmdzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syjrqsxn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ajcptids.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ahiuiezl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmufhdpq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2edmnjlnw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2yblpzrgy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kkzssiwj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2cwepytbk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2vxwjwuiy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2oatanexk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2kojwdgeb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2spmwaxoi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2umskjbne.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wglksgnv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2tarjvadd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2yebkwvfe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2pugfwfwu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ilryrphf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wvzanjpq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vexditzr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2uqvldhqm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2cyrwcpmd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ijxycinu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2epzwyeir.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jglaqxfi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2hakiedbg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xvugylci.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2psbnzvrr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uqnimcje.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hiohwrmv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wynrehtk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2szetkjue.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wubvoipj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bujgrvai.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ueiwwrbe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2elyvueap.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gmueplbt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2krftftnw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lyvsetxe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qfkxpgjd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2amxqmjfw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ipmeoowf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pllbcdbl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2adpvnixf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bmlehdlj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2rrvmtkgf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rwqqxxzi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qlrdrqme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkteavir.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2brqssbdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcsjrdlz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hnhnsdbc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nfatwjea.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2fcidvzdc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nblpiqbp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2zyoacbrp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2spwiqtys.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2wwhewvbo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kphbjhbc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bllnsinr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2nbkxcrpb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2brmrvuee.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wzrwlhmm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dfniwcts.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dgncrzmu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ieplhuvk.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qjzqphvd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hlhttzsw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fcwmlbka.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2mhxcwyoq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ecrrfcbi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gqogxbzd.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tztqokyj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jeclyavc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dpnalzgz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zyzlmegl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2aaksfvdh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lbrmhbrx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fbredjwr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hzvefzow.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixizhlwx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2drhciuns.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zscswbqf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2iszrdsnh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2tioshesi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2drevcbzm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2vfmesgse.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tsbgasfw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2pqsqrfbn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2moqdzkco.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eqadqdfx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pmdivogd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iiuduskk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hmldqfqm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hmjyebhx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xcxpfjun.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zcmpqfoc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vqkqxjbb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qcioyewf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mnqbbgua.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2enkvwyhj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2winfxbal.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2aazstybi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2zdemoasf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bvmqvfam.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2senrbede.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tlykfsvc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2haekkbvh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pxsbfcax.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wgfaeqbd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jfswmiax.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aymrqtrm.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2tiflknuv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bjzngvyk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2akjkivng.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mkqvlcrs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2tujdjnbs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ucvccwfy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2toereqmu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xzrtctnq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mrkvlhal.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jnigohxj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ooyydpvp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fcfzuigb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2owlcwiyd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sbycchvk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2apujwuoz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mymrlbms.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2turkicyh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2trwlvvxq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ayvicnew.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bkohzfov.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tqyahmaj.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgxmxov.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2abxarpiu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vdzjikmp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2umwerlrq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2srpdaghi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qgayvkap.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwltbtn.html


<!-- 参考信息 -->