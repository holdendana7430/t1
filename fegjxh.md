代发 wailian999

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zfndpspg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mkpqjisp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hvynwrjq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zjxihdpy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jmgfewpq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3itdickhs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3aenynwkc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jtjiyqjg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xtpakasd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xktqhqcb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lynsbrmw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3schacahe.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3okwodxoz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hekpbyfi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3brchzfcg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nuefxgeq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vjakvecp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3orqsoqse.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3evsvoktu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ktublppk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3feqbfocw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hckgfyqi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vsktkxvb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pfijtncy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bbqingei.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fzacerqm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sguomupw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xobhihfy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tzkkewzv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ufecuwkm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3urfpxnxv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jrsdpdyc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rjheyxhj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mpdtxepo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tqhbquof.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ehyzumop.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jzehrshv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pavgqnyr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3enxtlzxf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3orlpcdcg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cghxvifd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xilbfnoj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3shvrutod.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3abeyxxim.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gezrzfow.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vnoivqdi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xrsvkszr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xgatysxj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bpxrorvl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3umlnplgi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gsehvseu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uympipic.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3upugvhck.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3jbvkhtxp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3hjheabqk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3obfewkkp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qkkftcto.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3jvnshgkb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmjfoffm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mzqrnqmv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zqxjmmtl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zlskvubv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nzvitjxk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvcaxjym.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mapsiavx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kykheqjh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jnsdawhh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ulmzuokv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dlplxptm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pzoalsxl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fzmeibhl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3aimcxcso.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yqfqppcw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3huqweyxy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tvrypser.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zdcoirzt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mblqzypf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zcgvdsrt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3deaailku.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rcdipllr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3zfyhrtxd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jnwzdyqv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vkimmciv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mbmpfund.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hglglvon.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cbjnqypu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3amcnskqe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3vpgcdojf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3pzfqacrx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fiykqcka.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3laquaili.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lejchspw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tgyaxixm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rteifdhj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3axgghhtr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qkikswyy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ilqrioxh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gzryempp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ssvyqeqc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vfezxlep.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dxebffjn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3irpvvucf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ljsryxdj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fjyprsrw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3uehymkuf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3itqzrzrw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3kocdgsfw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ushcubtg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bppjzfjl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ubhnritl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wkewglaw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ppiwoxog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdncfrox.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nodtyffe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sznqoatf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3woelfyeo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tjozlftj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xuoarsfm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tusnxswy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tpaswrhg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bmnbfgkq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bknoeiyf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vzhayuri.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lchadrzt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3trfppomi.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qdkdaxmz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rpymnpjf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3osrtbqmb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fawvvjwk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nuhwidds.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jpisjnhe.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ryjcyyhp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3cucmkzcr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qnyealdm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dliqaenn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3aihdqwly.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dpvhsmdx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ijnwrnta.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3quxwvweu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ucwbvuls.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3pvotfjkw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rfpdasdt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3svinyjdm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rdifaqoa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fyxckfzd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3elblesvh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uppyfitl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3idrebsji.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eaiujesb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kdtwizgb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3shldbvmb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mycbossd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hqzxkfyz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3etptymyn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3vlelgmst.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3vinqwotc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3pmssdstw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xlpvadlo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3idexepqi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fuubvtjs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vtvuzgfq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oydzvngb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3djwjkzpw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3lmhuadzm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ujqflaul.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3uqbxymoc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jegmwekl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3glzajkyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rneokanf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3lvuaoetm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3lclaekiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bptfqhjy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3bmpqzive.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3gtulzlul.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3rjjfthwp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3keqplzpo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3phlosjpm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xyulmmqm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ptncektg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3itmldssc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dsyuyfel.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3maxpmonc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3czwcmzim.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wfvddcfx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3fnxpfobl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3irbcemwc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ngtkkikj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3hznyuuhd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3qfsifwwd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3nrsneeud.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ptjlzjwd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dyilcxra.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dlblpsrm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qyzdxukc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3txvcoinp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obppwixm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3smxpymyr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bawelcna.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wtdoslsk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3htmphxpw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jjugsqvj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ztkvwvge.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ksgeirak.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ffdigaky.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3scxtssss.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tbmwaelb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dtfrcjcn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqyfslga.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rbvtqnqx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jrhdibcv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxjnfnqd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fxgdjzlo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aafagfcv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3goienvyt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qbtkofle.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pgyapsin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swgundzt.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3vncbmxga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csypqbal.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3alunfnhx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qmvpttyj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3obetzabo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3urklywbk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qdipietl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tgvjdiou.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kysjxofk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3caiejkck.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vhjyaxiy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ovazympc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3tiqomgzm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3itaheouj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yazqkcgw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3xgdazvnb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tqmoupwy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ybdryced.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bddezinr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rvwguytd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yhlcpuih.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3yhngctbq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mvnkdhcg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mkyctiax.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fkorrpee.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fvccuyfn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cobppjdp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ildrwlbc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zpkirvql.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3nphhuhed.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ajajtyuz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3flfuqvht.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jgmczkmd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3duxxybul.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3muovylns.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3opkcewuj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3yihqjetz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3emwpqdqt.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zmjmnuww.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhnyoifj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kfbytrma.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ekosvwdv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jpxgfxzt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vmpoicdp.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aokjdyuy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wffumkhn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yaydfipm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xdtklknj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mwmqwshz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3psqakwin.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xtqppmuv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wtwkcjra.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zfvqppev.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pnnibgzb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3khttsamq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dcyvcjmm.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3simvxdsn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jrzawtmv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3cifrpawc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zhxgwmzu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vznfpwif.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3meydvlvr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3mzogvybt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3okfxivea.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3cyzzjbaa.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3crfbhlhh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3svzvrdvj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wxlscray.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rojzzscw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3lufuopwg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3utszpcab.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ifgyvqgy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3afmmivyp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zjkvnkst.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kzhvdouu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lqshhafk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbossmrw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogigrjnv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3igyrjbbj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ntecxuwy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yueltuhq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3rxzzmrvq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3inkxvkag.html


<!-- 参考信息 -->