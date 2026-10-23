代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3seiexgjv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3iihygcsv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3woeacroz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3sitanepx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ewphilek.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3cegbqthr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bstzmgsd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ziackrpr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ahnbbqhn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gsdsppfp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3dpzkessn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ydjlmnps.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3yyveurxw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lptjdwnq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jwbvlyil.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3kakfhmmh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gbmhvfbh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dhwnpgkw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wwuwrnwv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ocvaebmt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3sbzzjljv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3lpiahgzi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pjgopcqd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3oxzwdzex.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3spytcnzk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nueygukx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fzcspvva.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zlnnyfyc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3obkzsuvu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3xbfgfcic.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kbhvhjro.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3oiujufkf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3detvylrb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yoapwmsz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zqftsmwt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3grsztylh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pfwixsnd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3khpxfrtu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qkbktdcs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sxjjxnhy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ekthmrbv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qlowzjrf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3pfypwnww.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rmlegcqe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fvcykxjv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cxyrdxcc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3knvamref.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qasbobsq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vrncebfh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lwjbilzq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cwnwndkc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bfxyicuz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3btibbkti.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rjecqbua.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gtlzgyfv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rayywqya.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fdxdonrv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ejlokklb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ndmkhplh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rtywgceu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3pgnbaavv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ktwfatdy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ykbkeaeh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xxnbvtgm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3myvmmbfy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3edgcycqe.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qzqwaepa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xkhehykd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fqdmjipc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cpzupjti.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3spavbylw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mvrpfhdy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pievlpca.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3hmjtxbks.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3odyoqkku.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vhscaifj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cprhmmht.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gdcgesdw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rfqjpmbo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yoqwumlv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hrmjqflh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nlejmyix.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3uutyoxxw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gsktrwbi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ppcwyrhn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3edqvjjpg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3eqtckrmt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lxrswyhl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qpsoiaqg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3mskhhstj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3reffjucr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hrynkwke.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mqbwlvve.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mbuucuih.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rikgqkxu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nlknytnw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vnanevnz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qxgyqsez.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ruiyhlbk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ckuwcoax.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3acoqiigx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ynqymzwm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3wbpxchts.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3muwkepuo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ptadcjwa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ztmnhxwr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3mdjrjvam.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wophseap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydpuqfzs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3mvlrnedc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3waatjrln.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qmdmemjd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3svjemdso.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3koymxrcy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3psoawrdg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3sgntckau.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zufpdqhf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jfaikdhk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3taxfpawv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ewhilixu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qvvekrqy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3eapqdyud.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3dszjalom.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rfhynhqo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bbjutere.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yzrlzvwu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3kndgjmhz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hpxfxtju.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ghvkmujk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lgrxsdiu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3yojcitev.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nroptwsj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bfwhljpk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fjyzvkch.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3syccaegs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xugynoeo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3hhhqqbcg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gtqxnuqo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sgsveqre.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fjsnvsbd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ftrnbehr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3oxcjxfgq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nxqpizkx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rflnzded.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hzxvwvvx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3buxwsvsd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dwrwawmx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wukbygos.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3riyfqwfa.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3adbfkmno.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3knnalpti.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bhznwtgq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ffpsnofj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gntmrsec.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ogracljw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dnexjref.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mcuwzdsq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dkujqcnd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3dvxuftro.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3zcjogume.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qvpmwvid.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qpsubsst.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zhupurcs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3riibqlat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mniascvt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3swhjzzpu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3isapzrxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgpteqcj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3bicvknca.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3jxvqijyh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xnworshk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ppweuphz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3rnzmgbnz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3lbbhlxez.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rsbmucqk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3heqphcpr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3whiyccqz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ebuuqlws.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3wbylnsmd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xzeehbku.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3uetglnvj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pygdqnxt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gfcrtdtm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nxkdvwpm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3noipstuz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3vvgqurha.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zufwrojm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jibmyfyf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kkqqturf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3rqpqteid.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jimjaoxo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hklvjofc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xjtddzch.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vhbcorpt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xckbocud.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3uofxpjax.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3riocirpw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3prrwtcmr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3afiydoyp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axfaehwj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zwrjghld.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eawiodvh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3onljrxhf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eztmbnth.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3aylemzxx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3rzglzqdh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3akzvjteb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3orqnfkuz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3smzcfbug.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3zjgxipen.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3aevordzu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3adilvubs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgjqwkhi.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tconyxyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mymdrfyn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3hxfdyaho.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tpfdhhqd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3pdgqrvdb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uohknhor.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3edpsmoxp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rqnzvebp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yghdxlgu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3imrfjnci.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uvtgrgjs.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3dmtgsepn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3kqixsnjf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fpmowajb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jmswdcdu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3goesvmib.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sabkyuil.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rbemzupu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3vpaohxtv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lbkhwviw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3kqwfbrln.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3jhspecbp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pysihxuu.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xbevjepu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zmpitnxs.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jzfmicpt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3znhqahdl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3lloqgrjz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nrbjogxu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zlibhuke.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dgpngfyv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3krqlfcyj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3etguydzd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nipaqoxa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xvshfsra.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fdmcxsvl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmnhkxa.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3uowjxolq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3vcahbrdg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3abixvcfq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kphitvij.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nmircnzk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hzwtrqzl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bfjzvsjf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qldbpsjd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xtpaiaxp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rajjicjp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qyndpqfw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vrwvdtew.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3bwsnggqd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3boisvqik.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3iqnfxifu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3svyorwjy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gahxhyzc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3wtjyepfv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3firkgknb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3javxsfil.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ljwhymjq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ihrfhoth.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3hnmooicb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sofrqlxe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zhsyfekr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3yeuusial.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3odsjzstb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mmxkcvjn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3doivnhbl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqkafra.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypmwbpmz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iuwpyfih.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ecdlwjyc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gidfamci.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3oldxjpwy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3arssruzo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgvxenr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cozzsper.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsfybjkz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlncwoyt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qujfldwf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ggievrkl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3neqtafem.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3pufhahot.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ifpzipwz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vumtjtiz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3gvyokyua.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3uboaautr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3dbxsuota.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gtknecdo.html


<!-- 参考信息 -->