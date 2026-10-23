代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3uhtcaiuj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3segmzqju.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tocjpufp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3laegjkvl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vjmexezd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nlxhhojo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ntbtvvls.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wkxtmoac.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lzpgxiny.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kkrklebg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3haktoqhv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3shvuynti.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tuddmahr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zoiqemvd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3cjjjaoix.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qgwkybrc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ldjcrvbh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cwqzbocs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ouideadl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3kwlzbguo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fwymnoft.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hrozocep.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3culduagu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wofmbssl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tnrijihr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3znletmeo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pbgifmsu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ztkfyhoo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3syztqbdg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wddsvqwm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3aigujtrf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3remceexb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3haccdcvd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iccnwlte.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3djykzfoo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3glcsoqwb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3edmetgjn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qpkcukmr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3eeatizev.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eehhkeun.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mmqnbhxc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nmwuqvph.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vniprumw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ncsnjeyv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mjyauzys.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibdjpdtk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jciglvso.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nmigzlqb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nzugbuwe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zbodobsx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3sclyenqo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3dagbpcef.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3axzvsrfr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aslgzzsz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xiyyrget.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ftdheads.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3gmwckiez.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3caqegjty.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3espcdeqv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lbszkljr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3moumtyel.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3umgfjwvj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jkhlqoix.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dcllaxwc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zrjpyqev.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3sbzokzpv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kpslcvce.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vhttutai.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hgtdagav.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wxjgxndk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gnqxqyul.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3reukmgps.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3shgjxcjr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jfzwrjqj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3loukztsz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gkflbkjg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3aicafohs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ndrnkffx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kvkxloeo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3sldsomht.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3gwygxxtn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ycwthvgq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pwrapvks.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3srfttscn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hphwnvki.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3tzionlxg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3lvxpxwkh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dqksxsex.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jrfftecb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ohdwcxap.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3aynuhjbh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3essyagxq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ufzpoehs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3eruwypdx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3izxsdttx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3evmckwro.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tndwdzif.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lmqtzmio.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mkbheism.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wmuyavin.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vwlxyhmi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qlszcaqr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3melmcfmc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3errsxejg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wrdzvjwg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3djxkcmqu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dgwhqzve.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oxofvnlk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tvbxbjpj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kylaykzq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qdytauud.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ymllmcvj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wesqlgav.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qqgabcle.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qobucpft.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3prftwxke.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3fpwwpptw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qcfxzoqs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3bshhuoer.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3phwlvcam.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xnuwrntu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tpdjaenc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3yjlzasuw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zgbdamre.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zrjbitxh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3stsgberx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3nhnkaphb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fbsvmhds.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gfmesrrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3euqthznt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wqissnuq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zfdvwmnt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qjgdsywi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3facpkulp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qkzmoynk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mndesygs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pxnizbfe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3aocletzp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qysotsve.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jzbogohf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xklcefpo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fajpsyfj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hczstxxj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cknsrpsy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3irzjlqol.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3tqttjszk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xewywofx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mixqnywa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xwvpckxo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bvxdiqnm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bnafosjz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mpuhdwpp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3awdihiqr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fxniffcp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mlgwbwlq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adbomyry.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3orwnsgdm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3afxrrmkk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dyiikkrs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ricowxdy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3shkqnfpk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mszhfkje.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3uggmghya.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jkfcqoku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reyghrhl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3itgldfeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iijkygxh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ilutbweu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3efwpbing.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qasfguhy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3bdwgyxyc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3skygaymw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ajxrrleh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hxgdimpo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ajwqtwgz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cijarjki.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vmcycvnn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3atbrqmta.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vckkehtf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3dtewurce.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zipfgtyq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3vhvdibsm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3wrfxztri.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3zbpkcpsa.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xyvmxvmb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3agjtopap.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3nualvcae.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3yaiuykbj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jyrpusjv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hnsoifup.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yvamykrw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cqzdpjnv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3racyeqww.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ddephwgt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ukhsthpm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3umkygzgl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zyxlncqe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ejkfnixf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hizkexdm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gdmtraor.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rgycwzqj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oydrqiqw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mzykhfdx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pjklcshe.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3qkpkehjg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mfikvatk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ddjcwqsr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lexvgpyv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3tdisofcg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ioohnfwp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3digyjuog.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qunsusmx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3xnntbzwt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yrexpioh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3kcaijtvz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3jhzouaqq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dzwrupwx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ibtezfgi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3crkfnhse.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3adllxvsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybmbonyy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3dkrzxhui.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ayhlracz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymlerpjt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xtdcmthy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3eoqhoksq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ldfslgbq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dykigknb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vxshvcbm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3flgpsqir.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3zqqfjyls.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hykjmcrj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3hajwpvga.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3eqtkgaab.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3yvvqfzyu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3cjjxpcov.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3mkhfknyk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3fmavlrwu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qtinjwgw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3tvjqwtyx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ogefryzr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hshspiul.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3atvuntpk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3mmqnlsww.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gtuvldur.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3oqafxzlj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lyoptgwj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wrilrvhk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oclfczkq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dkwekalr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3clefmppc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ugiqmwvt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jowcyjco.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ycrnzbwh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iujrdrdx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vhsxwgaq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ytyvrpet.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3djdwbsjr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yigeyako.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3daxbaqtu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3uprsfmno.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ytgvbqnr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3igxacktk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3dcncoxvd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3krratksu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3drfwiwwe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gejcwhnf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kdrpozbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnfxonsr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3enljkyqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbtlfvjq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fbcyqqkg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dmqeqlik.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3nghyueml.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3prvrjbhi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hypdlpar.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vtygpslc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lzsxwlqf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3yzgplvxc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3arigblts.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3kyxylnng.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3rinavdpg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kfadfosz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3likzwogp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hkwmjvks.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3psuszbsd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3yeekppme.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3idxvrhnp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ygrqmncl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3gkvaeqyw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3hlfiqucp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iwalzqtq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rffddjbi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vfqgpwrq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mwdvqkik.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kugekcoo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xghdvgmz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3updextgp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pkjgkaxx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3etrailzs.html


<!-- 参考信息 -->