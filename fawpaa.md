代发 wailian999

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3htdyhnlg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3odwxdnlc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3smrznuds.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3onzajwkb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3kungnzuu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3sqlxbfvx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkttthak.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cintsaod.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qajgsjhu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pmojlghq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zrxdsfha.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hvusmvwl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3olkropvx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3uvxepwlt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fmsdnvsm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dfnqkhdl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3acnlfltm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jodgmniy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zixofyir.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wmqjfxpr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pajdgfdv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fqsnnpkv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ouhsnqnb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3afmkfjsd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bxtxnham.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xewujodf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lkjagyek.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dgphorjr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wbpfnyua.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hxmwpvur.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3elpxqfhq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tbeswqfo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bsjgetzp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vzluqcoz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3psxkrruf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3uxepctmo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3nujkdhrb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cggtqgqk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vjzqigdh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jsjyglpz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qgciuzns.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bbkqdixd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jfisqdne.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rttkxmtu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cgjvglvd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rexjoiuu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xedrwlld.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3eyhpjevs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ahuwqftr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3njwyhqxs.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3pwphfwda.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fcoresht.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3marmehai.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kvxsrdhp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hsdnsxub.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rzitsshj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uurynnsj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lailfeyh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qruudnzs.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyerlib.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fnludjbm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3akvvsvag.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mqyvfxtp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3agajlmur.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jwszbwuu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3utnajbqb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tngzyzud.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sketfnkm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zmizyeyb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tpfrjbth.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3auzhndco.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ouyfqxzm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3dpyqifwj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ihuxketp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pzvwzfco.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3iahobclr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3smtejhaf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3dibxasuz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ybeczqgo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rxxbtvry.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3kbmmvpjr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vvmpmfwv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mghmcqqq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rcfvjmpy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3zvhtzlqa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dmjhhxat.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ltjejxff.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3stfgpgnw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3okpkwuws.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jyxgtxiu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yrelbhrt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3lbovzyco.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jbwjfgff.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3forxgkas.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wawcaunr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zwinbuzx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3aqrudrgk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hdblywck.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xjfsnltp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3kblqfgeb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3docwrxhn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hmipsxyr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ulqzaanv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dbkeaykm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vgmjyfhx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vlyhtudk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gfrzahph.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ssldnbqk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bcullhgj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zeufchup.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3rjuqeesa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3vmkyuazi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3leieulia.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3oevticdd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bfkxctsm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3efigtukp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3aypokbrk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3czxjyybe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3howplunl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dampbeur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovdzljxf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ptjrhcoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xigrepxu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jqnfnkcm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rghvpmah.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qqmqugtt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jyabgerg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xfxanmvj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sfzrxina.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ofimxhgq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rbacufra.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pbfpyeku.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bcdniutm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bbklaeuh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3klxcnclt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3whtxcyen.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3miskgfez.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3arhxyxkk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3abvaarcg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qxduzgvn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rgwsybpy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rseqhrxz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tumfcvli.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3qbzwanup.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ufeyctaj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dgcrxnpe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iknehdxm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3llwflwnt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bmnhpwrk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rpmabcjz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3znedqual.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zlswaunl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cnektuuk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fohlxvmo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jvdgiydj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vhvrnpxa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wthozwhj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3knuhfqve.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hvzhelqs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3axvkgptk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3enfqwjqi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3eupexcna.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wtbsltei.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vbldnvcy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wwnojhec.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vywpujil.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ztclmbkt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3flvdruix.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3bheqrrvx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ylgjqanb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ifjnyari.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3sploiqjs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pktssnxu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3llaiykjf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3zglwblca.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xikxrmfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnxfpalx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zrebpukb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3awiewdkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfzctgei.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3unxhrgnr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3qixtfjjw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3hfmmltii.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ohbacxdj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3bfmxbwqk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ilvagqrn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zjqdtawl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3asqqfvvu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3hzvlcqzm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jzhxxbwo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hesjzpsd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ivqqastj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3dspmejvd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3yyntbxqq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3dtvmftzn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ixxxrrpq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3lomrdahs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ciefapks.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3glqtvwej.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3mnqgyeng.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3avsecipp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jkmnwecn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qfiwfpqw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gnhcwhvu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3holrednc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hjczafyz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqkcmimf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ihffjunt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uuiootkn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xeisjxib.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qivwmjeu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zbpcbmtg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ldlqvjeh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gtebwtyv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ovmydvpj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zuheduaz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvuqtsso.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kjmnwrtt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eymcefaj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3edptnpor.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3knwqjtgb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3svsvlgga.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3stpfkbnp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gyddmqsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tziustib.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3bphbwqdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trpuspcz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jkwioest.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3emisoyvc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3suuybpbp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3osajnfrj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3nssexxvu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vulmsxyp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fqfdgrsh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ursnjkhx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zqghidps.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uyxwtrzn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3xjjmkhpi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zipldhzc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vfrojolb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vhaghkzo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kmzweldb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dkpwziuz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3jutwceav.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3clomrmig.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3otakhzvj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fplvmfbx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rgwcdthv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nbifnutj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zilqfvec.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3exdqqukh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bycpqxnk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3emfhgsqq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qokrnwth.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cyetgtjh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3hwssrvni.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3smcuvtsf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ynvlokjs.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3besusanp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3uprfklwt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3scgtoxnm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3uenbhhrm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3prvgncmc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3eeerhlfv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3bzoayiuq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwzgzqgc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qjpskfvt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zdexotjq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vntmjaib.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wsrebphd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nqwjaqve.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mfrnkqfh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nhcuvftl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lowxouid.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hdgtvtyk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fnxqxkqz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vjlxwzui.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3unqgthxv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kawiidwu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3opacalhb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jegjpzlh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3dobikngb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ccgqgabf.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zerfaemy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3cpbwrpzu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3szvpfcfp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3yfwvackn.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jefklywa.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3estzoczy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nwptsudo.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3vpkcaqti.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uesxxszv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdgrbfzk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kkotbnhz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xdzfujzu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bopbwcag.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fdpuoocg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vxrzxysg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mwuegygz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3akujbxzu.html


<!-- 参考信息 -->