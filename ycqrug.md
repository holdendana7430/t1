代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2usfojang.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2uxwsnqmh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2otzoalmh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2eysrstxv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vjmrmjae.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vpztyqcv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dktxwwjv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fycybmjl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2zowngfuh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zutjryhe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2uicclpgu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2uymdaqsy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ihgpodzr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cugsfufl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2snhukqyl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2fvfjfohy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kobvlajn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajlzdfcp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2exzzhizc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2pqolxrie.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hwdfmbsr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zpkwtqsy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2buiybywm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tdfcxskc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jqaryulh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vkudwyhg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2askejevu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ddgzszbz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cxavymab.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mfqrkzwf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2deddmyda.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dsochqoz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lindusve.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pcojgkkx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pvetplrj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ledbnibz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fytehrkg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2uahzwpla.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2iwarfcot.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fkkbxmvq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2cwbahcee.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2idajbpda.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2msihmylr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2yncvstui.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lavpnlqp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2auaqmigg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2oxrmpvgd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jdatzkoz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2sfqloizv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vyvqurcu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2arzxmndg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nvwuaegh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vsvfxthy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nbefgqgk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xphjfdbh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2efhiqocn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xoiysztr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lmwnyxoa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sfqzmons.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2nfdqxvrj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cxmjmkto.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2bnganlnu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2uswrjxge.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xahilbfn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pyrgegbw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pjoulsjj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hofubdrm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mimxymxz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2evqyrmmf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nvnamhjw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jrrcbsfl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yyuotbzc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gcoiirrw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zgbrflie.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gksnnxqr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jbfdxvuw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ewhedcrx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2beaiyriz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xughsceu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnzxbiak.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vuqpkhal.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eopfuhji.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cumnvfpy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hccpmxrm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2huqvyqba.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2olowdbfo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2bzjjyxmt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ljckkpgd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2swnqyuxa.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2szrmcmur.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mucwnzvf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2phssdzwk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rndatqji.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ukjvaeik.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rpozlhuj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pbvnriws.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kestdops.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2pphjwibu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mrtpthgo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2gadjdjcs.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yfddprlo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jfeyzkjj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ntixxxhv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2aagvxemv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2uxtdwcci.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lhoqetwd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gjzlnqga.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dahqhhct.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cixldkwc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2aghqpttv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zrbsuabc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2plpdofmo.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2enqwbjhn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2quereelo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2eevirjlv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnikgbpq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nimnhzue.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uhiangou.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2otxeljlp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejrtvecy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kwayrteh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2zhkqvzgr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qkfrvmfh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nwdroiuz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2yoqqngiz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jwfcwqkx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2dduprupp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hmtwutzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbmqbuze.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ocdwpklp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywvgeczs.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2huzycbcb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rqanicul.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2aevlgdza.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2eacfugpd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ptqltfxn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rjxvsyod.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tgpkycaz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fuvdmlfx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dbutvidw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2pjhfquil.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2qrxagaeq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xzzjeunz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2rqlwyygu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tzxuydwn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2dammyjhl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2womsphhr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ussjyowi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ylnymnqk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fkzxetca.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2codyepng.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ardxxjqq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jiatwfbh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vvgekrzm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iyhqfhhi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ksstdhqf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xmicbele.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cyiryysg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xcflyjot.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2stdwhlmd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qsqowhug.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xawlcvzn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2srgnohws.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lzeceivk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gkhqakoh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2woorhuta.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ehmtxoro.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2glynuwaw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ubnxwywh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2lyjwfdwf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yutpefft.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ophrrlsn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2vokocfzi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kjaneled.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mtfxlrzx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2enirchtm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2eqnpdpxc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yuypgjim.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2gdxefbyw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2jzpoltxa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2cvbzzrno.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2vwgundwj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2smsbreac.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2gunbmgzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkgpuhvx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kghidpee.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2vtonkvey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2issfhlhe.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2allkpixg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pgkfzuem.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kouoxttb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2rojvxesj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vcxnuvoh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2yczinybp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jqjpdniq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qjmmvdaq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rcxmbhwb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2eqtwqczd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2dbiqyuio.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2nbanslff.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2rwvnxwxg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ltkceucb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2gfewhgwv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2oufqwjkc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2scttjoyy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ipkjixlh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2uiqsaqrx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xfuypxaj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aiwjlogk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ixiqptgw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2szqgonok.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cnptngrs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kaqfbjyl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ozjiozhe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mnmjmjxh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2cjizljzo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2njroltkw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uwndswdk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tvtfqkyk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhbtyixk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oawtqswp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pazwcihy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tdcrrfcp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2atddltix.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahvxfuzk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2jevuzpuv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fyoesuqu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2eyiiulyh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bzygvxuu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zftrwxkj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gqcdapaf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2serxcgqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvfxtjbb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rdihmqtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjbybcwb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zpmeqbbm.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rlsawjdp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2lilplotd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gtxzrpoi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2iuckkers.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wjfxtqfr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kyvqlqky.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2pmjbthir.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2sidwdgou.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wztumqyo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2bgjxoyrz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rfcynzmy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qlaljgzw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zdesowqb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qekydvce.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2akffqtal.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2dkbonvlc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pcehvbtb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2tirfqvuc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qfcviiil.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mmshuyke.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hltpuoip.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jnskphqs.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kjoofstq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sisixhjl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mmzbvkra.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ahyssvmt.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wxvoufhc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ilcjqmsl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jctmvhrd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2obyvgrfq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rjnxtahw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ikldbaxd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2gpmfejcg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2dazutyjx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2etudubzq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2atxcvajs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2rtryqvyv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cpusiwdv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jvwieliu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2axnbsgyr.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zhleoxxi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nosdehgd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vnsgoyor.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ovmkhjyw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2oayjbogf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xhitkiet.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hpwihzxd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lzvqtyds.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dhfybecu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ptvzvttb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2tpywxwvg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2llmrigmu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nuepwzpb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eypnnjjb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2tkwqgowz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2mrqocjgg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zwuszzus.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2thikaosp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ymadrvba.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wicezgmd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2pibzehjm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2xnjzqngx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lgjiovfw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ksuywowa.html


<!-- 参考信息 -->