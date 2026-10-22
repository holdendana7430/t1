代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2yhljymxa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xszcgdos.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lqnlflce.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2mmuhhmhy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tmpayjti.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2feirkfen.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kenrbmnk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rwiecwye.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pyhfehrb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ngawvppb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zrkvomjj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nqccjsfj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vgbgwdio.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2urlromeh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gbocwgsz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2uumnycud.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zugvryir.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2aoylzkvu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qtmlrero.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lffzfazw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2klknijmn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hhiwceqg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2nihdbnmq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pfimoqpp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2uqlgbdma.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tgdywhwv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2itewkgvj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2asrisrki.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bxhhdpax.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qjejktlj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qptfqmne.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jizedjdy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2avzyupaw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iwzhligh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2giqfeugc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hfwjzyuf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nmirymhg.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nbtlflpk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2neaxrvte.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bkdovbfg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ozzelpeg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bufmrubh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fnofesfq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2timidsta.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khbwqpbg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cwrgheti.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nfsbjqnw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cesxptqe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqiivdri.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2xirghtyt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uffpypmh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vjqygpcf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ycbvgaiu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qbocvvbg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2khpjkazy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyxrziof.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2dbefcyil.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nwrkjtmw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tvpijxja.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ibhciold.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rbsoukko.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ywwhobpc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wgebgjgh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cxfqpscu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2tkofrvpz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jijyseys.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dtkdvzks.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qfqbcqta.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2attccjlc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bqomoybi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mifynyfu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2caigjehz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ildgsnri.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wmtjojgc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qariwmav.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rknkscgk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2idkphibi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ayqwnssn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2zdqjkdnq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ueoaifnh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tnxyijbq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2thbnvvvj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vzmavqiv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ddpppbio.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kgsctbjx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bidpprkm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fmwbbmur.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jfusfzyq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2fuoihfay.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tnxwsthp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hlnzdfea.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lsuxtyle.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hofubxtg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fszanslz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hiaaaeun.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2qmvujwgs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zrckurmf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zrjazmlr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ixfnyptq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tzirbqfy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gyvnlubg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2iypmmldq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2cfalttfj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mwsnucit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cloqdqpd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dmmegecr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2niyscrzj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2juqjunmb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2djqmrmsw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2svzkjlsk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qdiovnid.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2efjruahx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yaekrwyn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lvrblerf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2afaihcvo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2igsnlaom.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xzvuljnw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2wdofvkth.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ikmwladg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nksfotqq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vxjbvwyb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wduqxacd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mcmajvlx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jumsknum.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjhrywsr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2upuqbsre.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2onwiqqhm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2zaghqjed.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xskuzjbb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wolwxsza.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bxxlbclo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pqktpeum.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zjegaqld.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yjtbledc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qztppgir.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hvlephef.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2phqsfvtv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2flnypdwg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fnfhbbbi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ateyuzoq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gflpqlri.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2profmzdl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fvwqtcql.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vvsvvrfq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rlxghjtm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nrndddue.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hfazsonm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2duyfxzcm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lhxsoznt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ucezvidy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xsudwcmf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kqjumqdn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2kcjynmcr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xyckiwft.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ktdmwaob.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ghnnucwk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2sxyzjlue.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2bdvtfsus.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2erkxywzt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2nvpyskge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfgsctoi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ucaensle.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2zkmaahdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sivccoro.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2goievphg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ofvcbhdk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2zpjfrfim.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2fdptcfzu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tdwoynel.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2laevvmev.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2kgsdkrsr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nbrjvanu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ivlotlxs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qcmbbsft.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zchwbkiq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gjlfjnzj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2aakdphgf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2iupcqlzr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2nhxsqdjv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2zbjowjrs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ryqdzdti.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2vknspwvl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2gyetgzdz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2naglkyis.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hqvzlpnr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cxcktunp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yefrtscs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2itaippff.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jbudikxl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eejwzlop.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ctmeqtyk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2leykvpus.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kpizufva.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jcrknmxv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fzkslhng.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmcuaopd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vjqxpwry.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2khznkzno.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfibzpeq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2axqtvjgm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2grobgjig.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ipoinzll.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2agvplawo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ewrjlmdr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iydnatte.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xzqwbkjv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zegbdspe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rwlatmnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unsfmvmo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rqsdpmnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flnljqmu.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2cgygnxga.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vpohmqzi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2plunilgj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vdiokvfw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2stxhtyyc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2igewampu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kmmrfobb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2eicscaxo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xiufonpa.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ryvjtnqr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2cslcfqdu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qmdpwror.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ghdssozg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nxflcuxx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2npctdubc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2myeyadrc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2aedrtdqe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eiyovltv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2rsdsmyte.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2yzwhezcl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xxskoqme.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ccxpyxjs.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mpyozhzd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2njahaglh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qkglurtd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gkzhckak.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fuafsybm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fqtsglls.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2xobizlrx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zmtvqsit.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kxuvlmyb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nxmxqqeh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mzjjhbbt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ylarptzw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2fpofwesu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hglkievo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xbdlovzk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bxanbbuf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ueecmwqm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dasukwdp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dztpobgd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yvhuycxr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qvrtdath.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tmiawtap.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rrzhewyb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mxyfghfi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xfikdxbk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pnqxmyyq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2alalamjc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kywddkzg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fgqlflrj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2nlnnhmmv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2lahswtsr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pixxvzbx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgxfmmur.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vuatrqot.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lhesgsws.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2pdiyofbt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eovubbge.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcqykpj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2marrylth.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2diipdfxr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gobjmatg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dilujkil.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zeqgndja.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2buzkbcff.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kybogevm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2waelmtpo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2styzwtnb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ediboeoq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qfwgrkcc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mgfouccl.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lvfxruzc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nvikealu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ororoblk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muxfupcm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2opualgcp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhbjmcw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2vgdrnich.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dugjgqpj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uszvzbac.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ympfygng.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2nfmwkzjk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2sdbecyil.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xerpbghk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cxjptbgu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wkitgiar.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ihqtvpud.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2uitauehr.html


<!-- 参考信息 -->