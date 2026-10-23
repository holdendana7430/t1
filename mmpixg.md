代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xkyxtmrs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3napnfvpx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bkaqiuqv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3pglwiycd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3slashmgc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dnkyikmr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3sefikvvv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3jvuspgxc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ostwvlcz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cwksluyz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xuycpkip.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jfoxpfdr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3smgicusu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dyvavavq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dpzgwphq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kppjifca.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nhqfdiqc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ljodupaf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ieqefxoq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qpqpboko.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qvxepztc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dckauysh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xrpsjttf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ltbndpsg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3setvgtyl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3svzlcjlk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3slluwifk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kpbfesji.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3othfvimp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dqfyqwuc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hkfjwhgz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3maqjymcy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3iovupabo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3njfzbzdz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mvjemdgb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pgtimizw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zxzniuec.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dbovfwqj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3lnfhzked.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ivjkgrgy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zlndwzmb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3odhkbnlz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3cbdonsts.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xgxmyyxr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jlpkzypi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xzvqurbl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qhusncbm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3peulmmfm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kuvjhnaq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tznisbmj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3esyyizyi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ayndornc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3enlfwwos.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pmuachkh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3kszxhona.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lgsupyvj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nmgsdjrb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hctlotok.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ngbfmljn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3izdyiwaj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3vjojuifk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dvrixpae.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wrliruys.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zvmzenou.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rvxifvdu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sjbsnpvk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mznyojew.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3scebtybo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3nkhxxbww.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nszootdi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tcqmbiau.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dgnfupwu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dzvmyzli.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yvojxmrr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gtlnkyms.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xrzxgzez.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tvxuvmyp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3defsfpll.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rvkdvgny.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mkhlsupm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ttoqcxwr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zudoqllb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yifbodet.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rvsmltgp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vtlyqtbc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3omfvvedx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pzufnysu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rwkngynz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3orucqzjz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3azmbrovg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3alaujwos.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3seicechl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lcitsrmr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3znhmrihm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3vlzyrzgm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3acblivoi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vparpzwb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zkhrsvds.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zfsfgolg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cnbachux.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rstuwsim.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ycdntatc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xcibpwqf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afuwxasl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3upauqofm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3omyeteiu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cyoxsqrz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hilbwsam.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3nqpxmufs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mhedugma.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dbhuqfuu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zdookrqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqyrocfw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qvmigdmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifmmelaz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3sgfeqidn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nfbuxfkz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qmygvdxv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fhfcqegb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zveohavn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cgncvfxg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qapxrpyb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3okgdvctz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fkmwbbwn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3oosmuqfq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nwbkyzgx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3cqznidqt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3twjrhjcc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3kbwewxfn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fafmjrsp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3mumrzlep.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yvbeeope.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3njlfqjuk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rqptcvdi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3owwbzlkn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3iwrgmnjg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xrfuqrke.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jpxctahk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vlarkopv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rksxirpr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wyvfqvte.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dlhudbyr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wjvntegv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3emilnuno.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xltlidxg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3icnndyys.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zzcttguv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ordrvzan.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3deyapvwi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jaggzjyc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ingbjoqw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jpryteig.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3unjryngr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yemsmpzq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qugkvwws.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3naznlzgk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3sbhelbbl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nigjisxv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gnyvvkpw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fayhwhef.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ekfrkhdq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eydltbex.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3igrydfht.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vjdhvjpz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lrndksip.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3nwlkkesd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qevdyhjg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3sjvpdrxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vusqsynh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ztmligjm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tdhzcdyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsyqusag.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3kgyyrobj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3tvvkgzgk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3arsddtmo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xfhlgkvl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mrffyfbp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dzmllden.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mexiiohw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3alppueyg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dlvrkvak.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3wvndkhci.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3xnclugtv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3nsgmqjxl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3acyhewem.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3grsvnwyr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3kevknxll.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rgedrzjx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3malnxvqf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3yroimccy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ivkjsxpc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3tuluaiki.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fuytordu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3futxnuuh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uucnqpcd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hqfqoyxq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wzodeohh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hhwatnxm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vrmmygey.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gtjlbikw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xhkmmxjk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ikkrnhkc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3glowraya.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sacfgrhu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jvrfashz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3noybmxma.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gdlkbsun.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hebihfep.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3aeizdqqb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3tidmfitn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wqraqiaf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3dixsxljb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yyejfjhv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3iywwabek.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ubzbmhdt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oybjnejm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sldrfzpk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ikxaisot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tswpbqwg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3goldhxvi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xwrwoqin.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3mayybxeq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3akwkpfdg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pgeppmns.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ikwhjaip.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qdauaxrh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3xdqvffyf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3euuyjkgx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3dgearuqj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qcmjrtif.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tttxctsx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uclpnkjm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3akiaomja.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cdiwddwb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dpleslfr.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3kiiuazrt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mvacigjq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ifnyhzxx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3nkejcxzd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fqwgpldg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kpowqnso.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kskmgdag.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3odpcynho.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zmuahohk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ydzbkvml.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ismrdljs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dcoutbsp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3fwhungmc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3uisysiaf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cykjefel.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zodcqkmc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ohryuyap.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3asbzwiep.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqorevd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3tldqicky.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3kcdutygp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3szzsoqxd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tldnxykq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lojylalo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ddbzrdty.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3extyhier.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3koajugng.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hqfdwktw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zedtjzps.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xkfpwstm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3irycbxvz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3wfoekero.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3accwtukn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fkkzuowl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zevrstlm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3acummmoj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ffyzdwcy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fbeamfby.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3grvzzidf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3injlnkwb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gwetbgrk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eztgkepr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3jmpsquxc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhibdvh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3imqehanc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3iesqwqio.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3nicpvrfy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3bednhtvb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hnwafprj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfubjoev.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rcbrlqpc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3gjplqlit.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3niodphoa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bkacylha.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tpefkvqm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mxiijczz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aveflhoz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kcpvupnw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gzakfacv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3evidlqts.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3frixhfaj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ergxiuej.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3xhrhdcym.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vbrfcwbt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cfnzrcxk.html


<!-- 参考信息 -->