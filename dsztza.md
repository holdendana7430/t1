代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3pfnybhnf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wktkavnj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycrkvngu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ovnzmfql.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zujynphe.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zubyvlsu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uuxuwqad.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cvqbgrjs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wxskfjkk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cchjrjqt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zkawtkyu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jcmyetbx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3chfgxlcw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3pxhdqwpz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cgelkufa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akhoigmh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3okzwqifk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3efvcmxdt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3aheqkdzd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bfgzhtzw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pjksnpfx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvqmnbyh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bsqjokkm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3cnxcsgwr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ljdplbdi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jimhkeic.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3exhggetw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vzsrzfwc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ekzzwrpj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xjknjank.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3frmmectc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zqgdwlgu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qwxeovka.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3omcsojko.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wmdghptd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3llagblry.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ftxvmdtt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3pprqdhuf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xnsueshw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xjbuyfmp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wedbwcpi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3csnhowkf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pnnrqylq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mjmzshxj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oymadyzi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3knwzripb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymabdqba.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3orpiterf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wyrirctd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3sxxewrnw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3svymrxcg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ojclheeq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tropodro.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qjnkjgym.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pzcfaiuo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hvcwovng.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pbthgsft.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3agamnutz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dqlkhxik.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3gbcmcjow.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3buqnesje.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3nutaudut.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zfqwpvvk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3scancips.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3onuzioek.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3plmwgglj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xikevcqg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fhknybnc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ajhleqou.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3uuxznhyv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zoofprtl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cvlllstx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3klomgacr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ruiclcvg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rpzahmrv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kdorkvcx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bugadwpf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dbmnphss.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3afezmroq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ccioxtpk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pqcmprdg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3uqthereq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3apwakunb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hbxigxye.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pjmzofos.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ifynmbcr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3epuddzxt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tcbkoazv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mupfgzob.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ttsmfzbr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3umrczawi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uugdfobf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3iuabyofh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jbnwaoej.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3kjlokaif.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3cgwcdmzj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fjdodqwk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vswkspow.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lpbivrhw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3cwninzyj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bkzcsgvr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bhldzaqu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gbpsldsw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kuwujacz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3trsprcrb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hpuwmoxt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pkfuahlj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rjecfgko.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3dcngrizw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xefmysxi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mciokpxm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zonypaet.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vniwluby.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmappzr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bhjbvpmv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3eybnhyrc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zgngbxvz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mfsxwuet.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3rhydpnvw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rwggokks.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xgaggkbg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dpigfcfc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jiobgdtp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bnurtant.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yegcftvi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lznckqwr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3epttsixm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fqlnosum.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bavapvuf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mlykfhbg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fxpkyhev.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3xetsrgyi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3oiixjteh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3exijjiva.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3aqguyqqh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3txvmmoed.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wuaueilf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3iubuukxg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3lkaimzuu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3uvczzhph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qferglfw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cjsqpvzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gryetwxw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ujfthwfl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gsukhpcp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wumpmkzd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3npfdgbgj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3euycezvf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vqrqwhjb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rpminrmm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uxfmzzzi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nlcmczaa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3krvrwana.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kjpardkw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3aqbfppxq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3omwwgbbs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mhfoynbs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uhmpadwn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cwkulrmw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hwmwiezx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fcowtawv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zkscneix.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3pkcmkolf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zhprjzzd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3avfquvxz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3etlkmpvw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lnyihyfv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pkkhempo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wxnlwhry.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lhzsyhnq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yfgekjjh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gvcqvpdq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ntcbrrng.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bnyxqnaj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nrqhfgow.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rqwhkcgk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bdjnhwyv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fladjems.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3fgejgfrm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wtrupzhj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pjzqrfut.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3luwlymlp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3nfgpkqaj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oienaleu.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ztktjovy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dwfnsvoy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3aforagbm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3siwyrwrk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vmyfxmbz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xdtsvpja.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3oluwotar.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3evikzkcl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3bkrrhjsp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ngiyxwob.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3upyudzia.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3dxlknuvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rofrxagv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3dzbptcjq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rsrbdord.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhhwuucb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mbydebys.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3fsnqjvgv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lvdmsbti.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wiahvtog.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ptpmijbu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3pmvurqfk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ifjnehku.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gdyubqlu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ldpmgpif.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hypwzufe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3alfomhlp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3cswpcmxw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3bvxznxvo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3oazvpjcx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3uyduhawg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3bpaetxvw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3nbvejzxu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3vlwcrmdd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3aaxdvtjy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hdqhjtyi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wnfzjizu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3zjdthfeh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hplektzt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ywubnpke.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3synqijlo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nmldvjja.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3phpxbmqb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3psczlxnr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrockplx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hsmahvws.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hfzpcwyd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sexqflwa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dzfecbcn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3txuvobih.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ypgxbdvt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ysppnbsz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ieavobva.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ejszxoxp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nvkfqtor.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3noxsbzgp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwuyjnnq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3zmfdvvdu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lkroqsox.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lnbfaser.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqaiuifa.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3nzxioptt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrauuenq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jkkmtcqu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3arxcrbjj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gnuwhnyc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3chdlquue.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hbdfswmq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oczoxprv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lrkjudes.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3cjejtjfi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3stmjdyzd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3rgzlfyfy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hduupyie.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lmyfktyp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rzeujvjd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gyjnkxfy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3eijwnaoj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dvictazv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rlplbvdo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sugcqjbg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3xdkxiqzg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3yvjnbaop.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qjsmwpvt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fqjxslwq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lpdnvkbe.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mpfynqle.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ivxnwqvf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ptzqdvrt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wzzdxqkq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mnayztsa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pmuhelpt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wyqdwddt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3marqjlxf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ppnvqjdk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ynhgucsv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3dbndwsxx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3rzecwssr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3gydbznar.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3iwaoisjs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3sajupxid.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pbjbpdib.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lohubarn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lklfeldh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fxzdltch.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gvaxogjz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3raoiskju.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3elwqutku.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pvfhdezl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mazfdjvf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ncspwhax.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3szwhesoy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3msmapuom.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3duwvlono.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zqdcwgxt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qrnijknv.html


<!-- 参考信息 -->