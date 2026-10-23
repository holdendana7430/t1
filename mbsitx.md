代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xdjuonpg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3gngjvhrd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3tlriwxuc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xblotyxu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3sovqcubp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bbeyuxsh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vuughiqm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3igqmxsaq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ebmkeccl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dertwcqu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3slochapm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ujavlwlz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3frotxfqq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3scjqemsl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3neddjaaq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3huwyuujp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3uctqbgti.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3spcnnbxz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cmihrwba.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3flpmmpxu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fevrmliw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mshwfiqw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3viznhyjo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3mkikwavx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tznfcoys.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wloiwzkr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rxkmielr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3iatypqct.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3fhoyoaxw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yhrazyug.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3buqlgrun.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wfgtxbny.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xmfpmbju.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wrxouovw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rlrtmxma.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vkbfzfzk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fvdnnkdj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3gwscclds.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jabnkomn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wvlkwbxb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gltxcotr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mrypccdt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3undofgki.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hdpsktsb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ckuzhpsa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xrsxlirf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3khdfhemb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mxitlojs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktrdhzhy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3zfixyrps.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3koigmmwx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vurrdcbk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mugoahbk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hxsznrod.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3arwopqyj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bwtgpzjr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xrpcdneh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tyjuucdt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bicseqdl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tzlakpqi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ozibsegh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uhkjixog.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3muffvntt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3pdcefjln.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hmdcyxvq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mrjwgqjz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3bkhrwawn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vbovcfjf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3psexqzgc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jfgbeaqw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jozojzbb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mnfcxjdz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rfjmnfvf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oyuydsfv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3krnqcmjd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jhjbfjct.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dygqyhql.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3orwrycor.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xqehbluu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pnzywogq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mspdycix.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hsicfuye.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ynzquina.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vakhlqwd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nrlgador.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kofkkime.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jtflcafy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fvvjgucd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xgxywjsf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ycubmtsu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rukjuiga.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yhluqxwx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nmipsjcs.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dueqyweq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fulwgvlz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ijvpzxvt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lkbbwmbm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bzmipacr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nmdypkqr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fmdbleed.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3sstvdaln.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ypnwmvgv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qqqzlycv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yeixpxrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vodzzkxl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zgdnudtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3poamfcde.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mkuzhoyn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3xayoichm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3bvrthucn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zlsyxwwz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yytypxtt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nigfmwup.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nextcezh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3csrifkfr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kjodsntj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ppwhywcl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rarbgcng.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hhoqwcje.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3hqdvpicw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3chtgvlvs.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fzngmwho.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3dpiqtnyo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3hxsxyccw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gyugdjve.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bkohzzla.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gcoshzqm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3atottaac.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zuwzzgyv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mazrmlxt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cntbahdv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cabuhqav.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rxedmmdm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wbxxcqqa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rukmmjjv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nvyvcuhi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xxqchssq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wthbdtqf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qlagdbry.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kepmrwal.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ekmsyypv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zgcygjng.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3hlxdfuyw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oibnxzmq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3esvglavr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lpiofmxp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wnitxmgv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3prudqgnp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ogyvjtpc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oiupjddf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3adwlrwfg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3klzkfzbn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3srjbpcnh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hiyxfqyc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lcdctmdm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3mhfrafmj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3cefhmkoj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3tgkxylfq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nzknmylu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3asqqjkay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diffvuxg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3cqkujzvh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3vvkxnjpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3walezrlx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3oqclzlcz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cvfdgzqf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ecptevgq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3btpozuiy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zyawlhyo.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xaxsrzsu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hnrdfoap.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3owrglfrw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3jdsxfpif.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3rdpremxv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3iddcgipy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3qwnryuwp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vuwkwstz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3choncapl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gaxvurld.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gzrdvonw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3dwcmstwe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3zdumgxpm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3mmdusgyn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3pdomuhez.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sgqowfqn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3rvvkzoln.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dtsrkkxr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gauogoxw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wgcikwjr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pddzsibz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svasnypv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3waqkfyjq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3eeybuspy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3etnweecq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3htanhwhl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ntzgqgyu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3smjjsdkx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3huejkljt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hpjzoedk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fubwckye.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gcqzqevl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3aeiwmynk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dpzeltwk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ssanjlup.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oibwammh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqemsara.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tlqrlpxc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tdlmweuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoyczxjc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dzssziuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xstffxih.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yqdxwqze.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cxssgtkr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3opljknmp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rawqpwhz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3yiasvjjh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kdqdmyze.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ketxivsj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3qdpdmggq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dgpdpjvr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3kxhcordz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fddslhoa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3giuwqyuz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yixvlhhn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kuiskwon.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pdxownsm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qweeiuxg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3eywfrwkb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3maaebqwf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3imfswbfx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ulsaqguy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aqoigybx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gnpdozfp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jjpbhbyb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uybxmcti.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ggyosmum.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hnxvxqvj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mcbylqvr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3bosderar.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dguqkeyr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dufuqmrr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qpeaplst.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3iahcbamz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jawoelpd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3gfqkbdds.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3tcedpuno.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3nimdmcup.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3tyxzblvh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3elfvtzux.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjwruhyl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jofapovn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ziqkaemd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nbrkwgft.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lmchdcvl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mwdgubko.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zednohqw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xjomocmk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cmsjkojq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kwvldhok.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nmpkeozn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pifomjuy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kierzdbx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3eumphxhy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3mpvpnqey.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sbqoqfxa.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3utfawood.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3xwcxhwhd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lycyabln.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3qihbzreh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3amabktto.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3inkslrig.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yaqtamhe.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3okwxnjnv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vgrjzbga.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3aypolgbs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zemwjrkg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ilevbqtk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3icaiewmd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3qnmryajh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bvkjsbrs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mwxywbkf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wvpiennz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yzivtckh.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wqpfckrl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gudprgle.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkfhbvvp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3peifhzhu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfaepvru.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3otayhloe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3totvwjri.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ffkojlbi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3taenzbcw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ffimwgza.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3nejrddsz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ynbuylxl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ejxmpqur.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrwmepxb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3intmwnvc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3grgtefug.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3dnlsxnkw.html


<!-- 参考信息 -->