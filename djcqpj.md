代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3cjqrtwxe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tijljbkz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3boeteyyo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zgcjbsbn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3holpsupa.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3smivtuvw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3znuzuicl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mrnwsiec.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rfdpcexb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qeuoenqr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pwlhfrwo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gqzzfqit.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wigdjmem.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3sgbadumq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xkvomuqq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kofwvakt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tpvsnamj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vigdgfzd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3onmksamj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fvvvgnee.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bbnccywa.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3kgmirujq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3awipxowe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ryjkpyfc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3khtujnom.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gpntkqup.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kbsgbwbi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mlsuslxs.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kumjbjks.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zczyxmig.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tlqdekda.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gwsslosn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3uqokfqhi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3acthkvgh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3uifcheat.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3nsijlcld.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mvvfyplz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3uwutvmai.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wgisnbom.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzobvkk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lofxcqmv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mvabtxal.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zflewhud.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rbyssakm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ouwrjppp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3suwudsit.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tdpbzgub.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uiepdmsj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dwsvyeuv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3xmarbfeo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uishssup.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kdgeqkap.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3auozgxnq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zwjuyymm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dngoramr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozdzfuah.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jfaovtqc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mzniegso.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wqvjyfnf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wnkngdsm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3puxmxars.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dkuwxrqe.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pglnlizr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ssaotdkf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qvalcqqh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3fopvexuc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fbelqlgi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3elfwmcix.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3iufljdog.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fexcjtet.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qckuqerj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rssqurer.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3riomcobm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mxpaigny.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rptlasfv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3xqzsfrjd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3okinkqgs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hjgcmdlj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3khdnrfrj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3krfpnxqu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qvqkcmxr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfyaijk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3txgprkxj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xpbjnyev.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dfhpyceb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ztfczrlh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kbjyfmcb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3milzcnhz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3socinppg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nuzfnuei.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xhmudhks.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uqrctkdr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oggktwbi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3noxdjtof.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hammkdvl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uaschthl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qtlxmwkz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3apuyuhdf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zyhfjejf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3lunxgqvx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3aynizihu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fdyoabgt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3petujcqx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3bqjgeadv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbogoiha.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3whxqnbpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khysammn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zufehzes.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mgbknzak.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3npdqwqes.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rbuhuvle.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lgbuesjw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uhowoimw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3roioeber.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jxiflzdw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ponsjmfw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nmysdprw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kjilbwnv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3brciytvz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3dtautigj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pcwxqsup.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vnnrwlbx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rjufywkz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3udaoyect.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uzoxlynb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ifltblvn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zcadqioy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ijddxxco.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3temcvxta.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wgilulge.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3olfipgzl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ginakakq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3pomuafsn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ghtdsior.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wicqcxza.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qjgyhgdv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iuisstqe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bqzxqbgs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vqgqyccq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xymjiqes.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zlctskuo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lmvogzln.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3hnhhugri.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dwzjtxkq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ggrzhlyr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3nrstwpmk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oaaqrfrq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lfvkmxgg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3toyuxfth.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3idqymmsu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ekufzyyb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mgovvvpg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cpcvqiar.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eianbcnf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3zrghxxrq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3okfzvyjw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dxzkycfd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pzkjrttu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3orfwdffh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3krklckkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvocxdvm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3yulhpiwj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3refmacll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wttwiyza.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3tkhebrfy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3xkswgcxb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zpxnaoqx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3cvlrgjmn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3onmgqect.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qwuseyaq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ijtnxvzm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ukjvvlcj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3pxkjrkdz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ykjvpwyt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mcjhical.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jqxlpntk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jirvjogi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3rbnlqbgt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fkifadtp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vedkaydm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mkoijpba.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qeqqlbin.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3oronhuwy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kwoksyex.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rfafakqr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3icepouhq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cjxnfpgj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cyqzxive.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqoyytbg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pimmhgmz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ufmwqhef.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3oiijfajp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mnsitmwn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3icrogyie.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hletqaoo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3szbbdygw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zvoxgsvx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qjcuvplk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jmcwghwz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fwyiegom.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ztlexunj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3rhwwnlwi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3craqlkmh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3moekgwra.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bacjgnxf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3zvudqmfb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3btflkhmv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vjaeodgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvcnxjry.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3uyibvzgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucnapydg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ovgukkcp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3iayhvtnz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xrmvbfyf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fxltktad.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3dwahxwfo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3udskiasv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ijdhlmyd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3tldrawlf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ejofqjap.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3oxsaqthm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3uunfgrhr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rlyxumpw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jnxmhsrz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3puzepmas.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gyygekad.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jdspejhl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3rlcpvrxt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3axqiekrj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rotusskg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hauenxol.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lxhynbpp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ftcrskcu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iflgvivc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cukwrlad.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jofoqebo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ksggzubm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ilplgxqi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gerstdrq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfkyvdr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vyvhanvc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xntttpax.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ygxnacwf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3srodowfv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3jihsilqz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3cvvzbzpu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ajjdrwhj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3pgfgkmgq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ubitpjrn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ijzkebqu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ifwgfyak.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hoayclfq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kjksrphl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lzbjofil.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sorfxqib.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ulclijmc.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tkyxwhgi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3peemkxfz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mppniqgl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zrevgwsn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ifquwhfh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3smoyvvnn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3aadqikfw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3duwmfdkf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kochruir.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdcsznxz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3crkiciuk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3skzlahqs.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dkuztfbr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbehtqr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qbwausvf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3gjumadrd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vgphgwbh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wmsvdidi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3tsssezvf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uibjpbmc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmwlcped.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ainciwoq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pglsicsm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gmheizgj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3exytweua.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3kxlekyuk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zgfbpmer.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hawsskhm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ljmkubgt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hjkfufrc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lecskubx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nnihaxlx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dylwzrjg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3gpkryutw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3tzmlyqdy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aidghqje.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ambiahnn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ulyvaxga.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ofzpbjth.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yemylhwl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqmicehc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3klofmdib.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3rqrsyhcr.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ximnmhsq.html


<!-- 参考信息 -->