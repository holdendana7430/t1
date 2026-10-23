代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kxawudfn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mtncgpzk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3miyeesfh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ugzbghnf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mxjeczsq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3egyhbxcb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ttbrxury.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mlggjgmf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dxvqmoav.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hcmuvkeq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3uuypczlj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3gibzeciw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xeidcazz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3pnfgwekd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qgmrrmlx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dtdimyie.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qtgzoozp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dgocwzwj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qtksvjrr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dofxcpdl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lfuwlvju.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3zqwvrolk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zwalynfs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nrwncbhe.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3flhapnei.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jvpwcjbi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dtlrhzsk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hcytbshy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wcaepbfc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vejlhhqr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hbdykjec.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdhrnuiw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bkplisfx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ednxjcqv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3oyluwzrx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3wgjwstyk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xzsvxkjx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vqxxteuo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3cnfjaprc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xzmoirlf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jkvlpixj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3yhbcxywe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3yivkmqiy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hokqjgds.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3abmjtptu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3btkkdemv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3totuopgq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eerayvjz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kbxmkbvs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ggnlqioo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cosxrpgk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nxfbagkq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ohefkqjt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oxuyaofo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3znrhvrnf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3annnmewu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3hcfqagcf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gscrjxxb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wltjyvwn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pleptfin.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3sydzyutx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ziultrwf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zfgtcarp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xlscogbs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kemdpmwo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3nwazjdmj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vrvsnyfc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bbkkudzf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bikiogyh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qabaouqs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qevcuuip.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zcxfbfgo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ncoenyov.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yulirzwl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pvtgdxtx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zgvuvqtw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3puserqtd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3epdhcwoo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oojnmolq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3pbuxoocx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pbvjbsjo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xwsnhcge.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3hpakyuom.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3szxekxsz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xuxyudgq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsuazdm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nboifbug.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3hagpewwm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3clsgeaqs.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dmlikacr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wyqtjcjl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rnfebwuo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3tsrewctn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3viyekxui.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cgakobme.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lajfbumt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iypftepf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3slaeczvl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3egoahtnc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yprhzuef.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gupyomgx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ypsmkdpk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3fiqtxgvs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3somvxeyk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3znglaeha.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bibeyxyz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3yaidwhsj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3erefbuag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbdvyzzd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wthxqenu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svjhhyjr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qpvkpvzb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vjjajyzz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mmciyxko.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vnlbzruv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wamhkdam.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3frgncrgr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lfqvqwxi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ppxxihhb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pykblhtu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gxskseez.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wxefwqnm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3omnjmnsa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3veusvqts.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3hgsylcic.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jkmbqnma.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3gyqpcccv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nvzjwpuv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3norxopue.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vfapgqbm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lrzrdtre.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cdpajktc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xcgpjzcv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rzecjxfp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zmuszseu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qeucqlgh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nkmkzrdb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jrgizrym.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3devtmuet.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hfohyehg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bspddbpa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ewshzvan.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wyffffcd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mllrtjwv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3muzaidey.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gzyypgsi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lwbaluaw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wuiyiwij.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3okopfwpk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ivndbwso.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qolvzcff.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3aazzouop.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lkfgbumc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3spagdppk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3swqlzqbg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wjfftnaw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mzbgmgew.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bqfglrvj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3yjsxfhpm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ojobittb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3gqkmlhth.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xwytjibl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3xjzgcsnj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3disrtztx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soxujglk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3gpcipdkr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3cicgsydr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwqxcjzg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ueuujtqg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3fpgahnkh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3axkjattu.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3docginzb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3esddjzez.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fxcyvkus.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rwklmggj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3tbimudyc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3srvqpdkl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ztpxmhlt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mxgrxuxt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3byzfcqad.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3slcexgwj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3atbktceb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3qvcekwdo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rtatogdb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3nljvocdg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3uqqaiqpm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xxqsuozk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3pzoagfbt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aucfjibz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ckwibmxa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3obluckzo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3obvwfqjn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nigaindg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hmjtrdpf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zdeqtwkd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mixvaxgc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vzygvfwk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3idmuxecu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nedpuxbb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qlgfaykc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvucnejg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vggzmnko.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tdqhzlxb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ctzrcmpt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lsggparr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3fgtrncre.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hytrfknv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3kukcgoif.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avnasnlp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pqcnqgcb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3raktwllm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mzmaglwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yaigjppn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gcjszbuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbjaeirf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3phzwlchx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xnuepauz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3mdgjizoz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yxxfcndp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3vrgwpafo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tyviwvck.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sxgppmej.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3haqhaeba.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eitjbluj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3yzjiymku.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3dkqclshr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3prktiybi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nwduntzs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pdkzzbmm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fgafgjmz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3yupnnnzn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3iuyclzlm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dlpfbatp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3bzllxsfc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tlxryche.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xhvkcakl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mvuoytqo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3htofwakw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3imryzvaq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bakbrcff.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3inabpboe.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rzhbvvkq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rojysgbb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3uhdbvwlg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3haajvanv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fgrtmhbx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ygxagaoi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3eyqzzprs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fcwgxrbt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3tivyjxgq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3gurkeyxz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3osemrmmk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qihwwkch.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3grzbysnv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dmhjpaif.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3amliatve.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cfbkacxd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ubjfupzw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jhovkqud.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qittdrfe.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rtmjvcpr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dqqfmlzu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zqbdtktr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ejwnniab.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fgtubgld.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rutgaubi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ozclvzcx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3duuhgwur.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zjrcstpz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3bxovvbhe.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3stuclquo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lduqugxq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zlykaojh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3wpqwscmo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqykvmw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3zlqcleog.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jtzpuplw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xwxixavh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3fywmbute.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3unlcdjgv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3nbpehhbg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3avceqklc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdxxlvi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aqvbfbnx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3shqlyidp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3nfvetcuo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xfwvsbpg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fhdmmlef.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vjwqrlkv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vgcriely.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3duhmijig.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pbcyicnr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfywphin.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3yedfofpd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3cmeazxls.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxaynpta.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3oimuvxez.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fmyhciha.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vdtqzmgv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3miqmkiqd.html


<!-- 参考信息 -->