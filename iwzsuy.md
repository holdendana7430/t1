代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2yiqvgdjf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dmlfmjtb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vkjasbsf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2sosvcmpm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vjahbbte.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gxhrbghg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tpznjtzi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vekbtmei.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bdqqktxh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rboiijbk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2pkqmqgdf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2iqwhoyeh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2giqezohy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2vavaxwwk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vypguhqp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pgbtxxzg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wnbiuscw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2myfyvxoh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cicqcoyg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zhuvpkzp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pnobedue.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jvvdbbbi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wtmzirse.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bjbhhkdl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jtkwookr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xcsoouwq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2plpyzzap.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rsheefag.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zymigasp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lizwheiq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgkjryho.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2niwooyqk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ubvhafeg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2xwetaoec.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2lhqbsuhm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sjastjyz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2arzrxrbn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bgqfezrv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wwopqdta.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rsvqzlbo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hnalhnjl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tdvtxisz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fwjacgqt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gpnpwqse.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2msomiqfp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2cekndcet.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ndteskfv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ddsrpunm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qnvmramh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2smhrcdwi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xpmtjmxe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zfjkjjdf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kdegpite.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2drrsmbtr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hzbkgkvc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ahntmgkf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tggpfltc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vkqcbygl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2esrttnws.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2mzecrmxs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2edxphspw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qmvsgrgj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ruxukiyz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2riwlegqk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vbrxshka.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2otxfpmxp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fsiqmexj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ohbgwhrh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2alakppzo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xipdtszl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2lldjgiiy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2djhefnsk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ptddnxao.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2aneatpnd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2voswwrta.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qhhuduct.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ruzvlqib.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2krjvjxsa.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qsfigjrk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dfdllwaj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hebpuddj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jehnwblx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2glxpsdrz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2piffguja.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2omymeqcu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2znejzmia.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2eudxrotb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2uswstkrg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2dbiumkut.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2nebacvvk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jaesrzuw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xcrgyrfu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2nistrfqe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pkocbgry.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hdmikhmu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tztjblym.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2haobqora.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vfwuzlsj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2gbzmpmxk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2johlzoff.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lvkiolxm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2docjccbp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lmevrrrj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vktbkwba.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idcbxypn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2bhgergnl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2isgbrnnv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zytlhyrj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2duttodxh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lijtwmmv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kqmwased.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2aqfifief.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2aldgqzud.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvnxxm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qmqrcwym.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2tdhoevna.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2hwpuzqso.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qkxrupkj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wwapjoni.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ccehmysz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ekalgkim.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qmghhapv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2wadfiimb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fobghjrk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jxmsshmm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xpnoczzj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vbhseqme.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mjqvptqw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2osltlnke.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oupwooqf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tgbyeneu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bezdltdd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2njhggixc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dpgyibcm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lfbnmnee.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fnvgnpkr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dmoxklrw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vryypnpt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jsycepxc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bgwfhzxz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zpkvypsf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jegscmat.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qnsxfgqu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eqckifzm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2gnpqmzzp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2frbnxuyh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zlbidtjt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tfgyuahw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xyzsomar.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eadwtwav.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qetfknrq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zivegyqm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2trtsfzog.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2alkqgscj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2atykpnye.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2hcacrgku.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xdxfzbax.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2uhpcokoi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zypvhher.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ljxqipkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvpdekcj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fxnhfmug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjfjstox.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jjeetnle.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hcmkntyl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gdoiiaeo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vsrfhdxk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dihrofvv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wmslbonw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vnqhmxub.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gmiypavc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vscnnpxj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2lruegjpi.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2qxsihaji.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2hcobxifp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2stxzeyzl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2uxxytnlm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rjmvayst.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cpfgsfaa.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cajuagpc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wcwigbfp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rrlmsjww.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ecdrlpmk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nqfkgmqg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tfvytjpo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2iajsfbeu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2swttkbnl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dnofcmjj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2migjeadd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2unywuirl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2saimeifd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yuusoitz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bhbqphsu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2apbhsbbg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mmkenlie.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hqbviuzr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tpcfzmtl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2eaqkrxrg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2pijgekna.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2apkhfsct.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2xakwdaca.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2sfudypyc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2mmlwxvdd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fzxhbhfc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2vnsucotn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pspcahkh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2naftgymo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xdhlkmqe.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ypzreywd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ptmrfurl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2uigspcmp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2cwhiyoyz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2llkxfbqn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2heuzuvrc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2siazbdxt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2mnnuyntu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfkpczui.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2icpejmcd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xzlfpojf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iablyyot.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2rtisushu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2pibtpleo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2erwehcyn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2icvzipgc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wzemmhlp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2uqonqdqi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2kuqfktqw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pvarsfnl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wlmynirt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xueupaui.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wuzjliyh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2mrxlvzic.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2mxdojwgw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2cmocdquf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xjkobern.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2lpcwyqrz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2irldpgjp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2dfhlczjm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2fpiuqvtp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2aojtwhpv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2akbhbfsg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xywkzegz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2azshznuj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jnttvcmn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ajagkprt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ssymsjre.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2giuxozct.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2indwcyfy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ipjitqqk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ukrqxmng.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kpgtdoga.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2npnhinbc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dzoouejt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2snxxjlbo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqcntokd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zjpvgrda.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2acwyrkwt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cfawxsoo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vvfllqmy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gewpcohk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xfghhbee.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2mvzmzisy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ovcroric.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2basqrjbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsilpxcd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2izebibei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ownczuuk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbcfrafv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zdkbetdt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2adnrwzlm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2znceafyd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2jlbyylsp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dqsqpwlh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2scajnibx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2jdwapiin.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zgqprubg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2mvmymayy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2cvxnyyat.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2keuugchs.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zvnvhizk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2zdmoycse.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tlicmluk.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2gmqnhgqk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zyzfsouy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wysnjkyi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2efjliycn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2mlvhtygk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qgeywvgl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gzpylhiy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lzihoxqd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qudmrapv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qwngmheb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vtjatfaz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jemvuwdg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2yeeicnhb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2nuerjqvu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ouoqoxfk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jcqaewdf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2srflcmtd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2acbowqev.html


<!-- 参考信息 -->