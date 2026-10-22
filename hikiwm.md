代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2irztefsu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hxgefvdq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rfjymwmb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2nbggfazf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ebrztomo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dbutxsvh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2eytsgmdg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2awgqyciz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ryaejqit.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fplltxat.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ytwgmcsq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nnxqhnup.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vdixkpvy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yxubakdf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2afqvtxkd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2kzqkybsp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vrotfmsi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2irdfhgom.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2luoigywo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2grbycbqm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2oyfsfocn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2mqroifsj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2djbuhzxa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ipdrsxnq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gwgulypn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2tqsmirip.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bmqxpqot.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2oijltxtu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vlolyifk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2iqhyygcq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vzlpoqrg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2csuwzzdw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2yqgrrlbn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2uhqpzilp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2gsmgqhrc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nqoostzx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xhjvitmr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wqcxjiqo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2teoweuvv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ndcaddul.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2bbulxrun.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hffdbhzy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2btrmyjus.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xcynobya.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kddcgwwv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2tnrfakga.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ttcpxpzy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzjnpab.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2fnwiwwgu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kwkfayay.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2oonhpxda.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uilcnmmb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xcxorwqu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2prmxndsd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2rqxeoalt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lgkwlowu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2imkzhjkz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ftlkohwi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qrnrcbsd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lqxkxgme.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ukepanso.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jurnfgms.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2uqeioxlh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ohnkogfw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ofbprxga.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2buffeduv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qhplmgnp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kyvhfesr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2oyhfqfiu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2slswvmei.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jwdyuwci.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2zfryfopn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2epjlvhnx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2sqxvaqui.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2fjgrodpb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2mxsgsxsu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2tyqwtbyy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcekneo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vkubnidv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yuooagev.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rtuyikki.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2utmsbnaz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bevgfuji.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fsnkgenl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gmecqtey.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxcztgd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ixdrbxcy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wuahnhzp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2qmcmgfnk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nvensslc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2dlmygrwy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cpgmstha.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2clotevaq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2doelfmhw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qidumtvy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2udakpoox.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2edwcszol.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2apjxsegp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qfikazly.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2odsnhczv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cromusfy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zolygndy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nulrhdbx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nonfphfh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aemrjbnk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2aszbixbb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2kvpcyatz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ztalzqxo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2jggatuso.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ulqxamlk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2fipcadoa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ykbdidcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahqkfqav.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dwwphdad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tigfhatl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fhjrjbfc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kodfwzpm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2esfmgipd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kuagwkik.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sqzagzpy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nzqnqadn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bcexswyk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fmdnkplm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2utjamxog.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kajjgxdf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2johoovcn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xamppuxj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2rntdixjf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gtjpnlqj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2qpgjfaxw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ejphdash.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wznozyny.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2urflrfoe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pczggcyj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2yuiuhlaf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ctljkfxs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uqpobehb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qmmgroyp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kgdvocys.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bqrzvckm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2dsjosrjg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zqyapyju.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mvmampuf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sfagofss.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qmqbwxrz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xqncjogb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jeakcdqo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tmbdqpir.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qaxrxrpt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2owrsvtmx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2slbwozrm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eyqblqiw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mzpyfudy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2bomgnuet.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ylfafqyq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2dbctywzb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wefbkrfe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hjdlpggo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rjhsdqro.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lmvludsb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2osxdioup.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gzewlnij.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2hyjohwiw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2cwkugzis.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2oalhjkwf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2cstnyxhk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cdsyyuce.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jrnfcppe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxtouxrz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rpcadjom.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jerlqzvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzqgzddq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2isaouyzz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dbnapacx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nnuyxhtv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2acsuscpy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2icxjsnfg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2zphlxpkm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ltrmrldx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2scigstjf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2tajpscxz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2suanhche.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wbjoticg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2inbbvtei.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2gdmvxcpy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tlsgxjhf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2fcilsdyw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2letqxkld.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2zbesgrfz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vsfutave.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2tqkwimzz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rytglkth.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rcjsxgdq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2jiblpnoc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2atcphyoa.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ckbpuihy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2evtoaymc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dnnvjuej.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jazjpwns.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2miqwmvzl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rfdjyhvd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qdvjumph.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lovpjkzb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wzgkjhyg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nppfhisc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lpdgfmyz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tqkkfbje.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eozcfplf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fqkxdwsx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hbnhzidz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tvgrmgnu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oqwnxmil.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kzgwdwgo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hylzqfhs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2psinlloe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gnjtyefp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yycsxiwp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2lazbrwpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgryyrnu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hpqnzhar.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jvweimnk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2yftahtls.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hqxvuapf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2mevahcci.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rcfvznte.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ibfgawkt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ucrffioy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2juvfsxpo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ihpnehqp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mojawvnc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nxjvhsci.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iecaehny.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gwmfxbws.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lbuzkbvh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2dbzkchdu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2tbfohsrv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qebumhjz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ymlfenng.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qgzizijz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pkgotkhn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tnpuxvpo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ueagrawc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eblccooc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2irkssmvy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2guzcarkv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qntxdegw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2kgdciwym.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ithrfjzv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpuksboi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wkqkejxx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cgtiddcv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2hlwygleh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2apsbvnsk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jvedschp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tvvvrhug.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2zvhwadiq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxalitit.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zvbceobg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2thlbclsh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nikoalqd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zcecdzem.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hlrkggsb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vuwgcvla.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vlnfuies.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hhbtvwjf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2iysetgbt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dmtrwqln.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qeblvqrl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sxwezvcc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zuiriure.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2akybwhhq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2lijevbju.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ktytgspv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ifwulosf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2wesiseay.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lzudhyja.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ujdwslbd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2egmppvsd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2lwjjoksk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lcipkqcz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2npgrmmtd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kxrqiasj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vtpznxra.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lqzsrpeh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhiaahnz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xrhjcjhm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wgdwcimx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ucmhnmoj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzexjxw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ymsrjbqr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cgwoeuah.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lrwrynjk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2icmntrat.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jyqvcggm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2etejzugw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jnfjybvx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ehtxettj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2szbwkmoj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2mosaszbh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2whhasryi.html


<!-- 参考信息 -->