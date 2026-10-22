代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lnlxbbui.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nqukrgsn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2jpftvzlr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2xuskakiz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2kgemqqzk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lmqfwuef.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qfmspkjj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wngbadqf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ijngzyce.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqjnfykh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2oiabdmvc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tslyeora.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tmnemblm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2crjztuav.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2doqyaxko.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ddktiksf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kwhftubc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxqoxhus.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2raahounm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fqbgzmgm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wpasssej.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2uvkdgfcw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2rthvclut.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2swiycxhf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zlyngnof.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2stcyqlsg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sbdbidae.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xzbsqlod.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2itcxjfpz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jhylbgmb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jhyqtfdl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tbvwntbp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2erwvqudo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2caaoicnb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cezacruj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ihrayadx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gmlbwcpo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xzmgvcjw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ppalfvbt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2slgfhcro.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hccajuek.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2fojykvxp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ondvcrsc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pugzddcm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zcsmkwsb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2klgtmiuq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hzqskaiv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rilzblxl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lznohhzt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2evruwqjj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2yzkbecwn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zswchqfh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kyxkhjou.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ibztcvgm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2aoykfneb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmcecif.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2rmzxwdgf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ccsmteud.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qjqetuux.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lowcabze.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sjsigywb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2edpoambi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hanhdcnv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ggadgxon.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xcbgigwa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2fwnzvlie.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2culnpgtr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bakhrxnh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2caggjowc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pzutbkvu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zoivnhxh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ybuyxlfh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2uumsxlsn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sqsapgah.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dbnvqapa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yuohuvcc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jaljupgg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2blwiuvlx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lwuodnwj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kggiuqbn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hhwokyeh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kndenpur.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pjlyqwvo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2txpdqljg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2owqrodlw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qmvrsmsj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hryptnvt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2opskumtw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vahoeglm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2pxkuelhu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2stftbcps.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rmjysxnu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2evbarthm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yofeibjw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rcljfugn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2laxfmbzk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2oxiykjwu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lxiqvopg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2opjbxnrb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2szssulau.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2stxavjtt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tsjhrwxn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ikqmmbnd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qmpkdbmf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2enxzufut.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2agsycvqz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zwauathx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dctdsttz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lpxqzlxi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2drdbhbmy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sungwfvd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lrerivqh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kixfwkel.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zdhgolju.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2atzzmvaf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vyrorfud.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dyjuhxof.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lrlzxhps.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2oxurbeqv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hcktmiug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nknmhkke.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tbnmhhzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cquyibjq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2umyvynht.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tsifeaad.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hsqqvlng.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rqgpgpjz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kzdntxhv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mbohfzla.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mvpibibu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qduubhzs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sohpmrtz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2agskvtpv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rsmgxjej.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2eyobcoap.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2uczrkzrg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mnqgewri.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mesylrrv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2uqhdfxcf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2wvbuiraf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vspkpzir.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cuggwkul.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ayfqvjtw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2zfwqluup.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bcuvwijj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2axrhfwzr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rrhmnyzq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ljyiwnci.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2cqtwgrnb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bswcvfim.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ofvjjnem.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ibwqfzqj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2msonxblf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jlskyzjm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ftyefcva.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qnstjpob.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sowntoxi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hkeiypck.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2eigpvwiy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pwntewvh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tdygbgoj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ijknkaoo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zyjxzmbr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fkpmphit.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2uxbsyaeq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bkdtjpop.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wpnsaier.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2awomjygx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2pfhisqgq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zkportno.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2riomdpgd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2mqruqaic.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jcsikmxm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ruvdigtd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2dpifhurq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ezfhxcrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mehyoeyb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kjzxitrk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hntnypcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oaebnnyr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2mdmeerho.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2xozrzjsj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qpgnngin.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kdktinne.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jngibdfn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2zusvznmz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2plxidaej.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2rjnwpwin.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qxpzmodk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2uqyljqhf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2rcskvees.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ryyxxqac.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qltojcok.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2uahefrhm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2uhpjqgfv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gojdwusf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2vvumvaej.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ejqtcive.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rvcacklw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2jehuzjre.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2svsyvbki.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2sklodsuf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ioootnip.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fcmobsao.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dgnnpqxq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qqgdvbrn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2evpjrtlu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2efnrpece.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fjjousug.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zufbmmqt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2agbyxbkz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggiqxcrd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2sscqdaim.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ukbkqfrk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ngsmntal.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2puofdobz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ixwnksgd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ecvxoopp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecmvzumk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rgdbdalu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2oleuvmdt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uyuwzezn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2isnmmipd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2licvvufk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jknrjeph.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ntypxvcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfeajaan.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ddnsneqq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yuriglfu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ldenmrnc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wauglpet.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2crksdnjy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ddhgqzih.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mxhccezj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kvawuaut.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2avmolmhb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wdqvdong.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2oelmussh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rgbwgbpp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tcsqodnv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lvfiypow.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2izwicejx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2wqaynmnl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2uetqrzpn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ptasfgyb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hcnxpndz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2lunwmjay.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nmambzbv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nodawygt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mtpsmoop.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vumknecl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rzshelrh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2spkkozcq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zekinzfz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbmyjnsw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jjaxfrsx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvswniav.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qpkzurdb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wfhooiel.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cokpjucq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ccascdhe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2zmlsdifq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vvyflcnx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xgubhaas.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2qdpokgzm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ypmpdyip.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pvbrxnbv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bhpcxzvn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sjhpqsda.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mgkyslog.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qwvwiiuk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2egucdssv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qrkndoaf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dzvipkeo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2palfmlhv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kexqsckw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ndtoxoys.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oluyfztw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkxxspd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2oikyiyba.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nkwvrsuz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qlksykeu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ousdgtrd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rdqjwwzc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2upitqdgm.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hkafhjcr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gbqfnife.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dhnibbat.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2emknuxfo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ougxmmwi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2yelajfqs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2biimliwh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2tnungbvs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2koaqgjif.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2bhnvajgj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2satmneyd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yoxcbkol.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2pledxqjw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pogzsipv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ehlsrncb.html


<!-- 参考信息 -->