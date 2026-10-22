代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2bavoodae.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2htvjeyie.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2eviggxun.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2fpdifqqt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pszhzrki.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vggyqscu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wcvsrhaz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2eywaglpz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2likzacex.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adjiqktc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2hpyhalsi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ccbzshmb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bdqhvmyb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bodmunbt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hxkpuzom.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lemtyafp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2mzrytbxq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cbmdrdsp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pqyvqccj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vrvvkqik.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jjdittnd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2umfxnzll.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zkdoffrc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ilqhhzcc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2akrhtmqf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ignrqgqe.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2taduobcu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wmwtgroz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2shwdvkai.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2erbjpmeb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wxedtghs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lrqpguqu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xxstjzkf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2bkqdflnx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2huuxmqiz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hszuebwm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hjhvqqxm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pvuauezg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bnkhbzgx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gelqiavz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2rsmkltvd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mnhyxpoy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ldsleahn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2aoysdaot.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2fppzzauz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2kmnpklkc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wfdqutrg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hdovnnxh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zvqbpisd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2arojywfz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pnmszojl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ziahvsdd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2chdcboky.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ubpcywlg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fkvhhwwr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pgwwprcf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2adofdccz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xdlwfsnn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ijcnctbq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2tegffnbt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ffbkrbxt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xzeozzkg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ofjvdzgb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cymwctif.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ujmorqun.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2klpsskam.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vkbhowud.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vmrtgqrm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ghwyzdwf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cnwqcteq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zosjbrqy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2pettjgmc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sepxerkj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wqindemk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fldaojem.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nwmkikif.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2gincquhl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vncbnecv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hfzstskq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ahdlxsps.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pxwzijfo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qoiawzjd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rvmxtlfp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2grxphngn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cgqvaklt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lwgzjtwh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xxdkaist.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zaosyegt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vgohcbzd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ywedifof.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2oxfglxeu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2pqndwpwm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2punsbift.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mptffxjg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rwhmfqtz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tclalxxa.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xxutrrjo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2seiowduz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2iviyaprs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pftqoljq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vkkmitio.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vvqniywe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uafygqab.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2edlibqym.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ifezospy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ufzofowm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2oasmjebb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kxhfxhid.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jhyzuqky.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hxaxiasz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2huvjevpr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iufervtp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2meilngdb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2njgilsgs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2uepibuqs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2auffcdjj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2sufcinoy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zhlpfjqk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jtamgefj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gmcvphva.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nwqfkbpd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2exjmuese.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ddxahega.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zwoidkcu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2idiodddt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2izbrmlfa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2exwuouyt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2punqfzsh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2csvvivug.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ieijyzdn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cntlnpnf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wejnbliv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wtoimcrf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vtfawdkj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2dguselqn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vowikdga.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cuqtwgyv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dactcdnu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tvdblyvi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2sanihjqw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2oeghbhsm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2eeoxfixg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vxdvqrjf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2otwictnr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hpbgftqf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cyzzhmpw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2nhickrer.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wlilqkyu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eqyvtgrj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xwrwogja.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2tjvqwjaw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uchpzwsa.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mrwqbgzz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gkrlryri.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jrqwgiot.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mofhkqqd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2slnzzafl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bvpbsgdp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2leltfmfw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jwvsfvdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2payvmatl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zcolucxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kggpnwdl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dykeliwl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2eedalolx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mcloardi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vlaffltj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sxsbhuvv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cndlqozd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ypdtghce.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2snhnievj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qkbbcdrj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2lucnotvu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mmvddysw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2iuvpqfqx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xbidotld.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2irlrlwxu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fhjcgekh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2duqjqlpn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tpjloxxz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tlnlvden.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zeyawihc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2abhjkffj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2hfokpljm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dgnukbhl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zmxcrkmd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pnykyksc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hycniydh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zzygbqil.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gzhubbek.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zgglexdq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ffkjblku.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pbnanqqe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fmltfxbp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vzwpkukf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vmtroxkz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ozynuslq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rdqrhbhz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2kdvzccip.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zhupwpsk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nqqkpzjf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2zmwaqlkz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2tgbgsnbd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fegbupga.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mksgekyp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2abzdydyj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2lfoujedk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2opjbprjy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ilrlklou.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wqfilfah.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2uvmcpeme.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2syhivmnh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2vxxulfbb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2mvkzmwip.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2bsxrcyfm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2eidruzei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvkwzrcf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2szftsfyb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nxsugrse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otpfwqap.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vhialujj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2xzhcdtau.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nklzwtgs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2fszyitzl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2rcaedwzy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ysxvycca.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qjbjqpce.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zwbfpovp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2krilmmjl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ikkrmifh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2acnboonr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2rulrpuvu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2pukbryfz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2bbjibfkx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ybaxqylv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2femwovdy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mqicqpfv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2glnmrulx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2swzskbnv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2yekunsni.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2meomikbp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2dkgzaekv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hherlnrp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sisdrudo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2itspppai.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vtlxjxdh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lviabikz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbobrqth.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vnmohdcl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2txolhgcl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kxsqzkkq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jsgmfcyy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yasgcwfv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mevxuuvg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iartpobc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2utkuojab.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kucfoljq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sgpvojqm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ckuwgwqe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2qmgsetxf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afnffncw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vjrnvepy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zrzxffvp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gbhpwvid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjalgsro.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wejmphwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivrbuhnc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ryshjthh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pbeaewol.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2expkewrx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pvezvjpl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2aqaghfsw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kdkkzzmd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kqawtrxs.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2oeollsdd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mseqfrgq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2oeactigc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gdaiomoa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vwrxynqc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oxybfmcm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2lyxjinlp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tnyhoudu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2spfidryl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ldubxeyy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cloguyba.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2aiextrkf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2zlhgivjb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2muknxpke.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wowbjjmy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tgaxjbvf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpnupkl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hxgqybcv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lwjggzfe.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gqzkjoqi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jbfzqntc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2nxiotixj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qgicxhzv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gatknaxw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sdfawznj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ffvclqtf.html


<!-- 参考信息 -->