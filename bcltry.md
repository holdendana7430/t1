代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3peyypkbx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fpacygbw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3aooiupkb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3elnssugu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3mbllffey.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3njklzhbu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mhktzunc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yabcznwr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3asdpunca.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cmmfrdio.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xhlteqpz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tkotlobw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3mlsdqzoc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fypurbqi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3meizasbz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ouavnmvv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ebhlnaqh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3fkfbsjpf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3bkgbuuhc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3gmgjotdr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oggadltt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kycbsrvb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zatsqlwy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ntabzclj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3xjguddxz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zfzveoqt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gcfveiic.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ftohjycx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wfuitqwx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3pyjnegct.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3aewjregb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fwxgbhsy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pkirtbhh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cxvkwpqw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pkcmtozw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ptoocrhs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dlcxkutt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uvvwmita.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rwjpamqx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3saxmnswf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3uwjldsyu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3aocmwowh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3kheqlyei.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xuvddyug.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rfpayhkl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zpyzjazz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3oqvlklza.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wglckscp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wpaiiywq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dobzjpig.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pwoicazg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wvrbhrhz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uqmhqqna.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xqovsdwj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3uhqxrdhv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nwfcktlq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gbqjzowy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3aymbzlrp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mnijltuz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zhttodoq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3bvcxgwfk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ggvjgtmo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbqgbmbf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pfxjrfoz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3cvuvcqpi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3upfirbft.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cckgrivz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zpryzhez.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3knbwmxuu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ficjiqxe.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3kkdqqgkb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ltwbjkyc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3bbrmqsrb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3amuywcue.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ipudjtld.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3aephuqfa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gerafdyt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3svtddbzg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dxidfoog.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3brhxoxpc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qabvmknd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mydofkuo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3bphmtysa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nhydicir.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ofpowkmp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tauqegvq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3krngzleh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nrysdysj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mggqozaq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zuxdgyhb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nbfqwoqe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dcvsbnmh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cudnalgg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dajhlsvt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wjtomzvh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cyxiyfzq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hvrelcme.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zhezbjip.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gymfmkpw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bpbcdaro.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ijrvprsj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zfwcnejm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nfgqteqe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lfzemous.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yhresnqr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hevomhfo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3urroovtw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzepoqcv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xqtlqyom.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fgdsathj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ejaadxsb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vusszwxk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3cetzvggc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3izlwxasb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hnsvnccs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jtqkqaek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvciioqe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3fxioiuqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjtvmhwt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wefqdfje.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jjfgvhgb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3oyhfghsc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3htuxblvf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tuyszqaw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3keeeyhwl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cssxurwq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ulgvlopf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ldlugvse.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3xnvxoage.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hfhqkeaj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lonbwsod.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3pzyjygon.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zpznojcv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3iapgmvqo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3urzdhlci.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gictsiea.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3igoillqs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qovzjxhs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ylvrydox.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3cfkzlzqp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3sfpmxzov.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uzbgvwkn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xzpbgxyv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ddadlakz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zjmwbidm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jgjobdhq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rrshafpk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3emifqrsg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lyhbdmqa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mucecvxj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lrcmaavz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hjfxagdj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yrpatwiz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3iasnwvws.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3odakfapx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hsxuaxac.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3znupxtuo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ypscnedc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nurzpfrv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wgobcefy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lzvdztle.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qgcftpal.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3lkqhrlmn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iuqihejw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3askdrcit.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nsyqgsvk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qjlfudbx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3uprbreoh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zvbdqagb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3frhggflr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3azlopeoy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3hgusgwrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmqeyhlp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3obtqzicf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ygchafnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpsuqkcw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ayhtndlc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3boxridod.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3nmhenmzu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3iwmgczzd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wniqmcit.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bxahprpd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3wzsqrbor.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dnldebzc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vdqmepvx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3tkedysue.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3unmkxxpz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3btqzzoam.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rjzjggur.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3raanosjd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3dbtsolmp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3zifqzlug.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3viusidqk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3cpbgqgxa.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3rrhrakgr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3btgejndu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dsxxfndu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3pdfheuem.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3knfxfbxd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yqyyngnz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tlumvkxd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrytvtjr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pvfqwdew.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xomdemcg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rugyhqfb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlhjsbma.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kfrwewkr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pdflmzcz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwehnkff.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3okktxvfp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dslrcczy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zqsgipjc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3frjcblit.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cozqzbsn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axsbqkcr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3frrxigpk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dhsntelc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3hgdkbjfq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wgvqvejc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yspbwgtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytyejurq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rcsnvlua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmbxkbao.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3miuludxt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ffruftmo.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3vqltqmky.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pgdbkfqb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3vbgbglxl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3petuqxrs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3alvxmokw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tgxxftpz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xobqggjn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3sybcsrcg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3eegaeshv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3krjfkcbt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wihkryxy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3cluackxv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3drjlmfio.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qxgttreo.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3psnyztyl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fbjzzmnx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3obrbjzad.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3nrmqreuf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kcuxbjhd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kvothwmx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3abytfwjc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ogizlbhh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qsqkfnai.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ogodrnms.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gtjjiugu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yctqqqrf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dmnewyyr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vupxlxcx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3khmqygwq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wvhmukyc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qmufdoee.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fyzoaoxi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3wftssfks.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3elutjbbs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3oxpbnaxg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nbetnayu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yqbcpxwf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ythzbkua.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3egyreuxm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hfdpbaba.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tqrafuml.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwydmhfb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3abunwlfq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dudlmkmc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ectxtqwk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ghpgovvp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bhklpuqw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3utfrvzvc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lbxciwcg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3uedpnbzq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hizmvrlo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bknvgyvb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ebwnggqf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3fxqnssmk.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fvftpbtl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3suzbvvaa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lcjqjitu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qrmnurnq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3txyiksna.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3aeibfiva.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3tyrrcpfd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kerzczac.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxcedgo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkdaltx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pezybkdi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3alrryzyu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ivkwpzle.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gncwatwv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3oruohpdw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xtqyilyp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ifdondcz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwqqiymr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3epvvmzmn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3scrcbjbk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxkgibnh.html


<!-- 参考信息 -->