代发 wailian999

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ydjoorkb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2esslxrqq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zmyziget.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2czxlsini.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mclovhpl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oycpjzit.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2yijohklu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxlhybyz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kcxlgwbb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tcvnxhcr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2zcgmcknv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qdgaglck.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cuaaspan.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gayazter.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pgrfcoea.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2aznvsvjj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tlcypqsu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2alsmqddb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zwwuhaho.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2lftuanzu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ksmwfwfh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2uvykjmdh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uyhvkmws.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vzqzqsvz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ayqsunkw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2aazuxlxr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wgfiamew.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2yvanggfc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2argdever.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kbbdwdcf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hyqklnzn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xixvyvig.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gujlkhfl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2obdxnxrw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vpwxxabt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2pggtnzbz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2nsybftoo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2enhegdzl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tkwepgbo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2crywnhxl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tahbbytv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fogrkkcl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pogukuvj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jugnrevm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tyrtrptm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2femmitcy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2iksxdrbc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jubpryad.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hlnikury.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2tinooaxz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wcbjfyiz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wpnhxpkh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2onwqiwde.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wrkovqzf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2lmqtckwp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lkjppytr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2oazgyowi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2fvptaseo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rfbxwnld.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bhjqhdvk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2osvxsnjf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2dmkeabca.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2suiqvmbf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mifwmden.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2bgkdgrkg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wnomrydf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2sgvisldr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yphxdety.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wnflyqqz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hpzqfumj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2etwcooem.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vfawfoch.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2uprrhcbf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dcwyiabq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2exxlzvis.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ssbhihpa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2patvzsnh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2uhbbpvcb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2hinpojcg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wgdaeizm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jyggfpsy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2vzskbysr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wwzoelkl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qxelqytr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vgjnllij.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zoqqlhuq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uirkmgii.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ryncdqvp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jhdymkzo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zzymhvqa.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2zgsgjxgf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qrcmruyc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2lhhkzsfg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qtahqrdb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mihcnmbs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vjlmbzrp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pjmybzvx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hiotifmb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wwbxpcwo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mkbkbedj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2evbpxucz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hvccswow.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bkkhombn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbdzinf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gwmshhyf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qhuyvqih.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xlloxqvx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgvrefnt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2umjecomv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2yamnegiy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2oosknfnq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fjgbfjeo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gnaucrfr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2quhhvczk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hbgewrew.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mxtnnobz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhyszgkr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2tiwuqcmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziwagvdg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uxgzumvf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2byvixqdo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tbgbxryn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dpekspbl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2oqbisrmc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kwkjjrbk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2becdwfrg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lzhwjxqi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fykuwpwj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wsxcxjyl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pejbnaco.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pimpchqu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2otiqyyoi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hmqjllxk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wqhpytjo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2nwenihhl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xbhpsmle.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fsfnrhug.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2colglgmo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2eirfssca.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2uzuzumqo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dvemjmfv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rofxayqx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2umbftvsk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tvgwznys.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vcdatqnh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hbwdujbq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pnyeagvt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lgtgrrss.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fjgxykfo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yeeflcfc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hcmpihha.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qesqkhkb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rrkekozh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2neaoyhax.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2advykleg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lmwshzng.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2khdwbqdl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ojiomqjr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uuvvmljq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2amwnhxbe.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2eyyimyht.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qfeaxfty.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hdzgteej.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hfbvjsjc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fdkwdnqw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ixugtqpl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2uxhdcijn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fygighkb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2oghxcjsm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ckgpsxrb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2curkvoxp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2kkycokza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neoextkr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2hkoqfazg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2fdetxrxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vaehsqcu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2sxwpzkwg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2alujspjz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2xrimcotu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2svraoxvb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gxaqeeto.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2zpuomjal.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jokfknde.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ortdrdmj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2tmiwzlhm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2bgdszzwq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2fdezzlao.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2xzacgxwr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2aivtjxiq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ckkbmths.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2jydaapcp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2xbbymgcm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2rlndbibk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yncrcuuc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2kulfggdp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2egvsustp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cfwydevs.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vsnokixn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gdetcnsz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sybifrmf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2accsggpb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kmjrqxwr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cbnohrhl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qzcdoazk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bzzmvjwf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qecubeaf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtejhrbe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nxsxpqno.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dnhhytqx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uoegacce.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wisgwesd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wuljfdeq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nnsvqxpl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lbnhnkss.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ptjpvmnw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2njveykth.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hgeqyjbq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2cixegkwa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jdzuakhb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dskkoraz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gckjxkwq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2iejgbzpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apfhkphs.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2joebujml.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qeunprzp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2vzvgiquq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2atandnlz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2phqdoebc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2uwfmyjft.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2giqzgqss.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2etxgzgel.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dzaijwsg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kxhjhucu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2erlsbzzb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kanfaaph.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cwvzkscq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2izpbzpwu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bzvyhcgm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vbwcityn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2cjggtutb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hatnpfgj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2dpgckgyl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jltkeqne.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2emreennm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ewdgbknw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xlrbaypk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bceidvuc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2melffuzz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xnwlyawi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vcthmwuy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2wfkahvjj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2tiqqsulk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jwtkwumk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2txzvhvmc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jvvaclwo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ljqwimig.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ydooobbk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2pmejpman.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2roqgeadi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fmswxsio.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zssxmwao.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hzurmrzu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hcfqrsys.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oczxlhfu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2swvlrxxm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fukntuun.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vtjgjgxx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vpqypkbb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nclrmtlx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2arkivkil.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gxckkpih.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qvxjbhiv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yjpdfgsa.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sodrmnbf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cvzuufiv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2zefkqsgf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ixrqixxb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ugdtbgej.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cnkzvbtw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gzzbojbb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2olcpzpgh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2iorbqplt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hozzzkzv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rlcochvx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2aquwrfto.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2sdrnytwe.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2llwmxnyy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fldhvsas.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hxjjyrlv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2unmfgvuz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2jwjsfjwd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mwvqblqg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2csbekdmx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ynpyknaj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dgwuoadc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yghtqxez.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qroinncn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xisfkcof.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vdfmffvu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nvmzsfag.html


<!-- 参考信息 -->