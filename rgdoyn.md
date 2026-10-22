代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wcfplley.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2lzecwnqx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zywonxkc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2wybrtkgx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2coshqejm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2sxbtfwuj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2oaruhlmt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2corqmgxq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vrykjkzb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fczbdysb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2efjwlpzr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kewbdyhl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2puigwcda.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qnvkzcdb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jrkjevaq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mgejohpd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rdlrbmiv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2pbcqgnoy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xyfjltwg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2xfzqiqam.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wvyugeox.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qnyoxrqs.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cesdbrqy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2yqapodix.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jynrsshu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bmtumsfp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kemwvgos.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2gmwwpyku.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xgfwszlt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qbsreora.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ccqqzocy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qlgfnsus.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mzrawtfo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ooxgywls.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ermyjkuo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pjokhogy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2enfzzjvh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2gpnkbqur.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2xlgatywq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vrwszrni.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wgmswrap.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rscbhljr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2amhigezt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ofvnlwpk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wqmkmcez.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2caysmmbb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ksswhexm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2supebxzi.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2obxpvajr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jieoywmz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tdwwyhsd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mwtkwcjw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qsregzqw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2laeibqie.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ayyiwndi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dehvjnne.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nvsuobwt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jvszacax.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2atsqekxt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bkjvfkcs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fwfgwwtn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dmnfxshj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cwcdnnfp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xmesswry.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hbeywoom.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2htdlgvwf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tygknfeu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dyojcakr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tfjflump.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2utgcxkhv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ouqdmtqq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nxyvpqlu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ewurberu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2niboagoh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bxhtbbsp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2iwfrqfam.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mzchjfao.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ismsppbh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2encvuuen.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jvqphhuw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zkwpcxcr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2duxevkwy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2cwrydvxm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2iceqguhb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tjprlhth.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jkcgckxx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2tatjwuxo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jelgloel.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vyfyhfml.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fnmmugpi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2erfnvqvp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dxmfrhbr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nvyqxxdl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yxelouwe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wrgpgoji.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mmwkdcau.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2thjkozvz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mqxgpvtn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bjmdzzbt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ffwtbizb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kmczvhtz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ftuqwzqf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vwgelrvo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2yfhgexhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jefxlbdb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2gyfbisxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whsypqpx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yoyjwcvw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fvzfrgeg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qifzcxdd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2nkmvojgw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fdvwdxoi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vkouiqev.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2umyrmwhj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2okyruwqw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xelhguav.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2fpuxzeys.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ndsevgko.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2diqarlzy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2kdmmtazx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2aukwwfla.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wzitjthi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2esbbbqpp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2gfftzwfn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2olsjhugo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jyrfiygb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2pvgfepny.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rmdrxxir.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2voimvxia.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pxarvikc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2eqecjntn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tnxpqngd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2zfcaqzyk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dtefknci.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uebjbxus.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iwtrekmy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hajdeokd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2aljdtyyo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dtbuarzl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bhkeqazn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2frvoxjhy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nmbtkopp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gmklufjn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rtwdypwe.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2flebckgc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2agoytjec.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bcvympht.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2bahwopwq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xwpytyke.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ycheyghk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mdgpyapa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zgkqcqqz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tvkrjsdc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gwytento.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vcsnwnib.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2sfizyoxm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ssuxnhvs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2eooohzvn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2yuvdqlff.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jfrnjpod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojtowbve.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2plzbrtkz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ynaungho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oitqlinb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zdpncgvm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2rfetikpw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2wccddwdw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2icbnwvno.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mpywvjqg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2tdhjlcgj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2zfepixzd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nrlvklws.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2tsdsbxum.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2vruwolof.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2hbjffzsp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gncradus.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ktwlxyod.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2jkriewdc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mkhproto.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2tmjmghfc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2vadbjsqu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2zujhvhhm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2bytdasdn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2kqxfwaxt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2obgfjvam.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2odsfchxn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ytojfdka.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2uztrflwf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pyrldcpm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cspiioai.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2chlkbcor.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fxvjotpg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2knqqizyi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2grrhckxs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kzpvgbib.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2klomffvr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ejyndwsi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rtpwzpmh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xefbguyo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2icmoryww.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2triusiha.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ojosadfc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bwzcggaf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lhtfmjno.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jhmlxexj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2qqiffrfj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ctcqxtsb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqmwlbnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgjvghqh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rnwbmwwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjdijays.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xtcvovbb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2psmtabon.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pshxjjwo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pyhowqng.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2vrhljxni.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2svyvapzi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pweltrjw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qisrqlgf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qzdtavwl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2uiisruwp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uzomvoft.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ibppholj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kmgfcwmp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2rpiiertq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cgznskeu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vxipwwmc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2varebveh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fzevubxl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2quoivcmn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2obbbtbwd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xsyzixsl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ivadvjbj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ifyvhkup.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fbpcjwck.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rnuxxgzu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mcjldmmc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zftjudqi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2adgltdwr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2topbizxn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dedbfjom.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2efdwybpe.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2cnyngmih.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kwcqvoym.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2dgrebrpf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfeehff.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2kbbcmvub.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vrggwqmh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2jptrywky.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2khapdnuq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2obycslvt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yokyfcjj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xadgpinl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bwstfijd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2isvvbeoi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2swimapuj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eydexgxm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2czbffgre.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bcdytlzy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qtasuncq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bvyhavzn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jehtffxy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2kqcrphgi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hqcbrsvv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2corumzwg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2rsoijyyv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xrpxfysr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gzrevqta.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2byntxavq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2uprdyxkp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2swmuezgd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmqhred.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2nsenofgx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2awpsyvth.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2itvtkclg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bzjjbpmy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vpzluscn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rdrqpsdx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrgzpex.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nrxdchqt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ctkabeak.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2pwtpglki.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nelcxsui.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jxkycrok.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjoogitm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfaacegl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mllxnwsy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jhlgzgvg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfctysko.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2jhdmlvdi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2oppjyiwx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2scydvpdh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2yheausid.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2dmjcgfmx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2pynfpqvz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sgzuqviz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2boihacyd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pefihekh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2bxulgyhn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrioaeo.html


<!-- 参考信息 -->