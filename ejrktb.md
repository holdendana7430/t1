代发 wailian999

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2antmkbza.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ottpfuyt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vvoirrro.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2udsdhqrz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pymwwdtk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wvhlwigd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gpdeckqh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2iepnqxzw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2yddrwxhu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kxaovxhi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pewadylr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ikaqhpjl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gtwjemwi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lfzqmpqa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jaopoqlo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rkquzurf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xcjmxfnv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mkybjswb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uzwufhnh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qrftbndm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jgampwie.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xsyfzudm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jfugqxbi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2hlelyqel.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nnkkntmy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2osxyftwa.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fstswmnf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ajdpnfxo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2abwwnvrq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2depspixc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ezrqmfbr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2iuhrfkjc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2upenqikf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rvcrmqni.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ntgtkzfx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mcotriow.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mdkkylhx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cemndhrz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wolpwrfl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kldzgnll.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jmfnphqx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2shzrwjev.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2drcmjmgw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2chyuipil.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kaxewtrc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xruzjkmh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2slgnxzcd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pthxllag.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2tcmcrhty.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2igbtwdst.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2sujgoafh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2luciuahj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2njxlxtmn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rwaeznfr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qabtiore.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fuuetzkw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xhdswvdj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mhgtsbvw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cvuvhbrj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xvferijt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rfvplgtx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ivanrxtf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2myjrrsxy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2tzivayuv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ihawdqms.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2grhjlpar.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jgmmgytz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lmkdcslx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2inxwfktf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jkvwrlpe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zhlzzmrp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqfzcbi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2btfazwso.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ydrqojuu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lydnrroz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kjvnkadj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nnpogzby.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jwtygpnh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dmtjuqny.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2itwbvgzo.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cwajndqv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zcgttlxl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jbwivyme.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gffrbpfp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2eflumvjn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dphmukaq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qluwwzcu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2iluigoqj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qjwhigle.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ummwpvtb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zotlvnra.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jhngcqqu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dxzhvbdi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dlumfnwd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bypnqvoz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bjbfpoab.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2hopfrfyi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jmbwanet.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fkpylffc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xeovmoet.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ckugybql.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fctpxvgx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jxrdqpep.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2yqjawfyh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2arjnfars.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zpmqxjgk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2millbkrr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wuxjkimu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2acxvhwql.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2kxzkecmy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ytvwzjjc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2clcsqvdd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2akpjlqcm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kqvmxvgo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2enzkucif.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vpsaptgu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ljlkmsad.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gdtrjpjw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ddcbftpt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2emedxmpd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2unsgfdvy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vobrnpuw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2pfyqkdhg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rpiueeys.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2aavmdvip.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lelzovwm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tbakuhjp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zhhziqcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqexlspv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bxclisko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufyudfjt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jidmktju.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nqduxhwk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2agipausg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2nnomtytq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pthbhdzn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dtsquxfb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mvxamxhk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nvliumwo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iwobawye.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vhdpjcki.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2uiilxxcp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2wfnfscny.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bebxxixv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2crzbgtuv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ryzovgxy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2touepfpz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2imvksmgm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2pjzdxurr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ynddrcbx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2yjxkpdsv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kzkycvlv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2onewjsbu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bxcnnyzw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mnzecqqn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lgqymxej.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mvapqrjp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xguzwcxs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ebddvjnp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2slqdceba.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iwujoqxp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wvazgzwu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vyuvnqsy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qguogaev.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aqgmawta.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zfezhnnp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2nsvbzxqn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vcsurtzp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2unlhmbvt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2odtfoyyc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2lviuptws.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xjakzlsz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2nqswheta.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tjqvdjvl.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ijzqrrgt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2omnogivc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2bytpchas.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sphmbhbf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2wcsnfbnf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2otesadzl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xrenxuni.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2gpqbimaz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2trtjjczd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ifqhpvwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2woixpylj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2aswnfnyg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2bmaqsuvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdciortb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2eigkhuus.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vitubewv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ouoredtd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2rlgsgsgb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jyambpgg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bwpbtvws.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2csfkhspc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2mkkvexsb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gfnfyodz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ohqjpsrt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qhoguxaj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2crbxknuw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2tiarztxf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2zgrkspjm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2knjipezj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2opscflrr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2psoibeql.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2prsbyome.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2spmsjswf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2cymwjttb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qpstgacu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2brumpatu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2flexjdpe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2iwqorvfs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2slrycccv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2figqysdy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mxwzhhsx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bnbfkbxn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mwbpfuth.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlvllhup.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fveaieko.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2haoerdcw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nhqfnofu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rpeseqpt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yuiegqnx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xivahxmy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wvvqdwyk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2urtkfisu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xefbnxln.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2bznjshib.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2siqcnoyb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kwjweobe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2epvhbiwc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgogfuhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aawhkcgw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kzhyahjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khndlodq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2obwgaufd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vbgktqfr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2lmcmuzzc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jkchxwwn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2vgfuwrcx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gnzjccfz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fkzlplzj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2tmkvnefg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lzmujrtn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ulmsukqr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vavqewua.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sgdtxtly.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ylmmljnp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gibbgjld.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pqjftwow.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ynolsrop.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2gxrtmgtd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rsuwhdsv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2cnjgymly.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ilejwupv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bazrqahj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dtwfbntt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sjvygxnp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hfvezrwd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2atburdnz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wpxfmeyq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rvltkhct.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2hpvqfwml.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2tewotkop.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwexiabi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uinixopz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2lphmjscr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ckvfiapv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jexjtrfc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2aonrqycs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2slzpsaqw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2reiwqzbe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2thpmarbt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nzslihxp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mewfzcdv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wcjbozbs.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uhwxxksm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qdffunkv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2irfkarxs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2agjeandt.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tuzoaivs.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ubsrqqla.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2mlkxwnom.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pxerjtqk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iuwmqraw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qhgiuyxi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cosfstdc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ldvwtbsv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nxestjur.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dhshzxcw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mogihygq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzcqphm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xjggmrei.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2fkoajwxt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wjhddidg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2pzlrzaur.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2iixbebvn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ermentdf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2maqlbdfc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2okdcerwr.html


<!-- 参考信息 -->