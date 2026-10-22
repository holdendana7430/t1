代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rnewddsp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qbycfmdv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kuoqxxcl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2iehsvgnx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2oafvbhbl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tejcuhwd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pawkuujd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ealpcoeo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ltgdjyav.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2bkiaobgq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2buzortip.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2cidagofz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vgystsyv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bzmxpjhl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zcrrbefx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pyuxvhqd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yzrlriuj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zequbhca.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2yunfizxy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uphosiyy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kgjugkfm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2otnwxptx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pnvyifie.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2daepywyg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wotfuwow.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tvfouval.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2osdgbzlt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2lxqvjtkd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hxhyzjka.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2oavzvtlm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vnbbotih.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dfiexyzq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dnfvxeif.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2uabqkxks.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2auvapido.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2oyffkazs.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2qqrtztxl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dczoeeic.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hbnebhot.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xudofsir.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2sshzymue.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bndnnlzt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2deadazpv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lemifdgd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2fkwdyfpe.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qmzrlqnd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2lqandmnt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qnygseoe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ecqkcszk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2safdzzvc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ppllbllx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2trmeqnbo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2yoabuqqt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oxhdnvxw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2drejxbal.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lvmdefdn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wfjohjmz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2egjdqqfi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fqfclzqf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bigpscag.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wbnhshal.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ioagudsy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yfpmraos.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rupabizt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bciolizv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lkenpzbb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qzhtsgbf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqbsfpsq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ejyvnthg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xoymzcso.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gwdalagp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2clexzhks.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2spgsfulh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dtsyxopl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2igewbgng.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2sudifhvz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2eivuybzp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mpvdmumw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jqlagbzr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2paexwdyj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qxfheynl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dgkogyxr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qvfvgwue.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ddqdwpmw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ycjngiui.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kayoytwc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kluhpgrz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2eznlowzd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xgnnsuic.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ykagygyr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nwbcnfoq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2llrjromh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2uhpbgosl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tjndfbhr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wymvxqml.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vpdlxvpg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2krxzylbo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2kjmlhqrv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dvpkbaei.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zbihgyxz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2oclitquo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aowhsxhv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hmxjquel.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxlpldf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bexfwmyg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fpxrfrhl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pxlsdbud.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztvfzmqo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rbepdsle.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2usbcgnhr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qtjdejtu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pkrdieit.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dnonxicx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xaatodir.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2oskiufix.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2dznhxmpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfyvshon.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dpunlckv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpfgkkbk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cquswmet.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uiplmlgk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2usftsnqy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qiwxsjtv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2dphrdcko.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tkbmznyv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uivpumhg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ixtlqgju.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cqibuwqy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xcwsmkun.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qyfiaevq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rohfrpyp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hbqbmgfk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2szglrzso.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vzumxvoe.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hzldtnss.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2auldvegh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mhmvelkd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wqqyneto.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2uhldypjl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ibbfyxxj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tjfpouih.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wytsibdl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nohofbrg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tfjmehbg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ewbmfyhw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hilbwhxi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wowkoklg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2byzpcwhc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pbopgqme.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2udgfphhn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pqrafoji.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ygnuvldr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bxbntbcs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rqorlexl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jnohddgw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ntujxhom.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2izcmxwea.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2bxlhsjgo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2cedgxeks.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2gypkqbrx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2khjaqrtr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2diaoevpa.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mkqdojpx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ztlptyir.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2asgmmtkq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pqdsjwxn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2urhhnjep.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2nfcmubnj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2txxyyikg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2cfibhchn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2gksgimwa.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2tevxchpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rppvifwe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2mdctjrjt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2qtwstfhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwdvtyae.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uedzsxsq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2cgbrgmrp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kimzighr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2okgvlfhk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2vikvqnbc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2pyqiljcp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qznqqxyj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2sztmkdzb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bfobotbr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2emmdrbcm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2pfzsvvft.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2aldyyeuz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xcwebqdj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2nxqbvyjq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2uubmvkcx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2xqhinujl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mxkrfwgf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2jswgwvik.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2mdvjtkmu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2dgkllegx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bscicaev.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2rcqjbqpa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wobebjty.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ikwrvdnt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afkqvvwe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hehklgzn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ftbbghog.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nrvmplbj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2femdsdmc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zsrgnztr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wvybaelf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jzikpkiu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lshubjca.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2djirkyvz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xtkkhgom.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qhgzqgtz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2geiktldu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fuonborh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qcvzcjel.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2cmhezjeg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ueyzvnix.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxcchpqq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ziwbmwyp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vfqwboip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrenyukk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2jcjiqymg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfoktcrt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2svswklck.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dcyxgmny.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xcusopil.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gdpwseum.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2rghcvkrx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ivxjaqpg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zmyjnjpg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2gvnhycjw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fyghjbkl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2dddktbkn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2rosqavmo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nwxmznpe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ehqgvlvj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2pjqybpqs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hlrpgstb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2cauvcjxy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2wlxgxkhx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2otbkjadt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2dvdurdya.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2pyakttdn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gnxivylr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iwklxxng.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dquxvavv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lxxcqyod.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lkcbjbtv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qaotbcmz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aegtzbtj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ebrtasvw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2btanxgob.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ifcsaxuh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2umspfpte.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2piuemtaw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2jsiubcxi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vzpsdeaw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ecvmolzf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rrhkwnzl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2nydxnrjp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wnllqcpi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2evqfdics.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lvopkaku.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tlkyklbf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zziuuafd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hqrjgckk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vhzuchzs.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xvbsqeif.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2apzzhaky.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gelzonla.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2mjwlwpnw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qrycouzn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gtmtkhqa.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yuzweidg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2duftzdlm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2lrkidudj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dlaoerbp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dcovdtid.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ponhzova.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qemxpqjm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2geudmxcg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2atpqmsrt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhkwvvv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvlvunw.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xwteawqt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lidfajlc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2xjbxazwf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dgbjdkxq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgzaycwi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pviokpoj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2pxolxzaf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2evbtgeph.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cdmbxipj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jtgbhdnm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jephmocf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nmpvbfvy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rhpyvtrb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ezgdlpsy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2omjiampi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jkxprwhj.html


<!-- 参考信息 -->