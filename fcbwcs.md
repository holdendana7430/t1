代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ycryafpf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xuvutdud.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3rnawpswp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lleuiaww.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3buusvrql.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wwmtjdig.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qlxcncfm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yeitkkoa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mxpyhobl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hehgbrkr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cpomtwwg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ibpxrfhh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3sdeoctdh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3agunjngo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bkimignw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3oosmbqyy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3womuyrvg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3eisnccyc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ubthgogl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3psycekls.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3azweetwc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3helsbmrv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lehzlmku.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ohwbuqmn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ukzpmirw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3xntuwcml.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rhrqcwuo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mgrxgvhs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3nbaebqco.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tbopgzhc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fbqlfdpc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3acqrcmfn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3oickpkvl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rttseigr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qzipbnrs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zyvyjfrk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3azlpvlhw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ytgxpjik.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rwqrhrkw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wtifwjar.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3anynxpjo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3irdazrxr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cbwiujqo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xhwpnnmy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qdbskkrs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lnqhncij.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3pijhjfjz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bisdsaem.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rfjksgbh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fjangynv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggtnuvgu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iepbxwgr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ellltbml.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mqytizik.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3mxsncarv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rlywpgew.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3iviarwmc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ggzeugbl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3baygauwb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wtxxoytk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3keljjxpv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3glvexqve.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jncxvucx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ajkvdpoq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3birvoznl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tljwkwjp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3oagpqwny.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bgjpzzsj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mepwwptw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3cexozavb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lshqujsy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ezhsryzm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3egmwalyf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vynxijfm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ttglgfwv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gqlcchzr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dxcltmgl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pzwvnhtg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3uekzbowl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xbxzfuav.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ermwtqmx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3oqvtwqdf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ynfkchcc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qnswmzmj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yseclmfo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ntuohshj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3siluxohz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kgoiutoj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3releqvwx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tmvbmxjt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ltqjqjiq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3skahomet.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mazlwcds.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fkpevvmx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3scdksdfu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoptjjvz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hfmkzvhe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wyudckaz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nsbmblwb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3lsijwvsk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3nluzueri.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3grwvlmvc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qovmohtt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qjdsgsep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwxzwyhd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ulturlbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igwcwlnl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wqcjzdwd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yltelgdr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rzkytzdb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tahxmtoc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3unqecdxp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tycgoryc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3uatlqjjr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gboyhqys.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hgpzjybe.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ioeqegyx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ebkxadrt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3peavwosh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vjafemhg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cteaiqie.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3pmbigibr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mevovvld.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3shfawffm.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3caycayoj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gfkjivif.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3iioiztyq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3pzxxaotc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jsayqxea.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3najopavo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cgqtmxan.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lwjcnrut.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3kcmbvciz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3eqlbpifs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3clgvxful.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tdcvxkmg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3okksvkxz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xzjygozd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3svvtljgh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dtcszmfe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3avtrfmfj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tqxsztqk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nycefqlk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oozjwqhv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jpqqdnih.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3yfujaucb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gemhcjkd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qhrbcknx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3adtlbsjw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eeogtumc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kgcqpdho.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3arfiwdtd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dunwbxxo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vnmwrjfn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3smrtldgv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wlohzflx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qjepxxag.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jorwjzmt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rmvvclzg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3zmhkoppo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iehfiqyp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3gnbfkbnu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dbehbcmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stsfryhl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3gyirbqrd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3mzujksur.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ufbvxros.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rwcnmpgn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3nyhrvsoz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3sdvbbdrm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3lawjsiec.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3huiwwart.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3wehncoqr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cbjvmmvx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ulqqkuyg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rzosceto.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rovptpmn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3olrwochp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bmnzdiqh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3egjoiwhy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3cbgaofrg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3uuaqlxtd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3vpzoiqdu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3prjhxkyt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3akcyefuf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3unffabwi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gsxthshe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kfnxnmob.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3clmzuyjh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3volywafd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3moeqsifv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zlhbfghl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3htuxnhvm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vykrhreh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bultupst.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bdfmidcl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3muuhhnfv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bnxdvhmq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pwpxlfcw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sknwgwns.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zzfifmge.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3dpacqauo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ejqxknkq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cilqlnvz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oiiuayuv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vyxuiwjp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gpfxuglf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlugpthv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pscjccwa.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ckjkwbwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buylyiyb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3rcqqelso.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wnnrijff.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tefmzcjg.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qqvntzfx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3anfyqfzs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mkukmunm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sqtlzmlv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ytnzfhrt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xqhtnmht.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3kagyuhuc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3uwtljrex.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bgmgdbba.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3blcvtfut.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qriddiuz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3soharqsy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3qfrcmvlj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3djwkemob.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xcrlhuff.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3pviwkasz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3bmpgjsrl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wtgrgmeb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cxcqfvzy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3suofmorf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kubvkrqe.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ovyenkvq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vxhqlhjr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lohfpfst.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3oibcaokp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3yhehejfg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3zayvgmls.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gilyfnep.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wlocizzn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3izpucdoo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xdlkjpyl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3kexmpfop.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3tjavjrua.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3jnomsuqm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3pyitvmnj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hbilhxin.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rvhavosc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cqyvoenr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ykchibkn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfrkpedx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3isseoxam.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tpmyqkga.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ztutrndu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wfyitxqz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fejdsxyi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cabcgxgs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nilapnll.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rvpsfjkb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3nepjufds.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3sqfcpeus.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qzfdebmb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ijkistxo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zklwwqyu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jphcijrb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3enpezugr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kisilexd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dqpdtabj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vwswvvkh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3kzztjrbm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xolzefic.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3uyvoixyz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xktvaupg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3bdklwjni.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pclqvket.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ekwntubz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xwapusia.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ejbxcdku.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bmwfgbcx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gvvdyqqe.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3slfbwmgv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shrbwiby.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztixncaj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3estelnpb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hpwjibpg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqryved.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ltyjkvsl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3xzaqhjtv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kbpnuydi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hthdjwke.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3trqwoqfk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fpdcickl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ktzqgvjo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bmnqrfjb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wcybnskm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3yzgfncxv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3emvlodfn.html


<!-- 参考信息 -->