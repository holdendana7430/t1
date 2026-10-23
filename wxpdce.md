代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xbtyxqsl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3yaehjcpz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ghvrziiw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ceatigua.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jkqlzrar.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3myluuyuw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kznlvaqf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lpzzmhpq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bkxqgocx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tzuedamq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wznqcbet.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3snqnibqo.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3aiygiwsf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wkzvilix.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hispqjsq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dnijelmt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ceevyfum.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rkofagws.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wktsakvk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3itwvemaf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3oaueueww.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mtxhzhdg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3izzqrzel.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bfyuasdi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gjsexpxf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ysqkkxbd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ggqzjdma.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3oubrdgrc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ewnrxdht.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gmgziiml.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3japeumlx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tnrxumgd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3zgzxpita.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mwpwzepp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3fcjobbbp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3stzbfaqh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dimjaesu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ouvuktvb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cynfzggn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3banduvxv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wduxgecg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nriqttdv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qhghreio.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3daawioxn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3nxuwgxqa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3pqmfstss.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3eiquxpux.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdhacdb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yxvtpvry.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yyzyduxu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qinrrohv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lyeexpqx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jiudpmfk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vmjhpdnj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tdqbfuyw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjuvzruy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ejticnxz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nrzdcjcm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3miqnjpng.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3svnlvbko.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mfwkmcvy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wkusillj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mpworkpt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3cpwaqlny.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uhreotda.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lnudkuet.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lfitmroo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3urokebip.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lwywowml.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3iwhgehwf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pwwuavwa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uxhismkd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wbnibaaw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3buuehdja.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zjwsmdic.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hpkcxyif.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dufhqjsf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gvsyhner.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3cjgkvqfm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3brxjvtvy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tzqhufcx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3boimdanw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3clkpoiha.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ugnbysny.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ftdzzsbr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ycdytzvs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rbtevptu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bdgtxmbh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3bwfazxux.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mgwqhiwi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bmumshsf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ulopurxc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aeneqlpw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xdqdmhyd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3yjhmcdam.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gnqbbtmh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vxputtmc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hbqsbuwi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3fpdgdvaz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ggknduwy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3njvpunbw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rfchacoy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3oyhkoxjp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wrudxaga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsrilgpe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3sggqepmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvqziixd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3abeaxyyh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jkjvrlcz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ahtlxfol.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qweyegel.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3eebqwxqt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nzunmvkz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3aqloausx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ftqsozlp.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vgtnszde.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zgcmeivx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dogmaeze.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rabcbxfu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lcdynldu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nrxunuig.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3tdxvhltv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3behzvbbg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3erbzqyxw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3bsmysfhy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kzpihfks.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jqncocei.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zigfxvfc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3szxkhsar.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mfnmioxz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3iayegmdu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cnueqixz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3egqjczvr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ovpuvfpg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3raardsvh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cyieymsq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3naugdrxc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fsycrzvt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kxrcpflq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vldxhmwb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jcgbmuyt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nnfssjmx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nisaaivw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cwbnmbzg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ybrkrrbh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3iuvhddmq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3swmtwlci.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3uuozelxz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3skmsxtzw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ljgiurlu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fmihtjfe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3inzwcozb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ktfrqtax.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3doptkhnw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3boxfjfgo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3hxscstqq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tumawtvh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gsauidau.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nfdknlwp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3mtqkuktc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obddjoqi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3cznuuhap.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vkbvvaya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjdtbafn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3gurhoncp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3mexouwvj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3hznegsqs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3kvhcyezr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wnoqycps.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xcquvdxk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3fohdkhrt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ipxpzrne.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3tvrkhogs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jnzcheaa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3lbqgesya.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xloevjwf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fmpbyrnq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qpgqgfjl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3wcqskzpb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3suvcwmwc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pbddcwsj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3dmmyatij.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3emhuyufw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3prgyizej.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zdivlnij.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3wsigzcnx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rsolcsmt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uwdmolls.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tsobvcva.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esyqiohg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zwclueif.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3fxchqizy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zaevdwyl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lzgffnxm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3iiaiqfcr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sqngxljx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3abmdxika.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ncrgwbeg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3scztwmll.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tfpsmdoh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3epdmzfwz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szaojmyg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqticays.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3bvfyxksp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bpxzlzai.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3rhtkoeep.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3duvdoajz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rmggvnby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddltabmu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3zbxoyadb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbxnueke.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xxatlfae.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3gtndkqct.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xkenyrik.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yparmasa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3fzrikwin.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3avmpowko.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vscmhbyv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3hozhsnfg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fuzineyt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ykbruvkg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3qgjyigva.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ytcrzhez.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yvobsurc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3mszmudvx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3igqtzcix.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3gbcgafyf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3uooacktc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kkzrbxgb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ulxecdya.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3afmluimk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3btwhqujj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gqzrdmpb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fxyozsyt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mpukjoiv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wkdfiqur.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zevagszw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eocncdrw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zmghpkzq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3tcwhwpsl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3zjcgnwal.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3afplrjuf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bvcpmaqh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3lqahuisd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3veyjmiih.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3flwsmbqq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3goseagin.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3esmcmbpf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mnzhakjm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ituzdpdi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yjbxerxf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccniyeaz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rsndkhec.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lcmtbiea.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3twtrxwie.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sbkgvnie.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zworycfv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nsymfzcd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3lfufndyi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tioujovl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jjagmzwf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fzkdbvnu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ogaikexb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hpnwrqug.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rlljtmsc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3cnvamdie.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3kyebrmja.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3meuyonzg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ggwhnbmz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3japdczxx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3waqpcuuy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jsyydovj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3cwxhsrpy.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3lkjpzfqk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zmrvfdgb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3worvexpu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3kzzywanw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zuxitvhz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3avzmspmf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ylgfsgoo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vyhyfnti.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3feyviqjx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pwilfyvh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ttuatlnu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3axkecxac.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vatcjqeh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fcaxcygv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bedtibtw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twpojcpd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vyrasbqd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qxrtuuuj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gfvgmcdq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bcgfaclk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ofthnnhl.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3mbcsmook.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zcoqrubv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3njlitwbo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lfrczbfn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mdmwjrfj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3xvzzxmmc.html


<!-- 参考信息 -->