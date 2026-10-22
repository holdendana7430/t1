代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2djniwnkd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xpkriyip.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2mmgvxtwe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ymqfcmib.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dslyoivo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2qseswcmj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2iaihfgbk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yhwnltol.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jwgpgsdn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2obovaumt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mwfarpcw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mxlglpyt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2burltowl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2utcxmmmv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2icfxriqb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwsgegqp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wjwleeks.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2garotrkw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bbuxxrdi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulleuygf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2oflbfbon.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nuhsmyqm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2knsdbeas.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uynzbwpy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ygdhziaz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mxfjodvj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tdczppmu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yyqqnhpa.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vftyuqej.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xvqdupnr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qeyszysd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wzrcbgmy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zvcgwojn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2edbbnrfg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2elixneuq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ygxodsqe.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2onsshmra.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rpafibub.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2phatxufz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hhcgwnwf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rlwxdqgt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2odqvwllb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2npicttzr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cwqwogbn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2seuzwoiv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2omcowbsm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2otbukzuh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qpbqcdbe.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zziltmmc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pqstmheq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pzexuyjr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nvmraujg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ezczglun.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zwcbafwv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mcrkjskp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tdwjtksh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wukitlxv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2auaazfdl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qzbirerb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rkbjcpdk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gjavqxqq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2gqvaocim.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2buhhugox.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xhjaebkp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kbrrzpjv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rptpsqhe.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2birfxwyo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2gbustacr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hdggkwih.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qemxngqj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2owsnvlzg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nkrlmvcu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2brfbpeuo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kxaztpnj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zbeinxfp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2gxjiyuvn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ceyjljmi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ugrmxmrn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2sicghctz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2bgkmsyrm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2udjtvyuq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uxhzjxnl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2lqetwrvd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qokdolua.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2deivullw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2obobxsol.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xkcltfyq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lodpalhn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2znxefdxx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zpikvjlx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2riqfdvgv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ftpcvohn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wqqjzeto.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2teiqphuk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bhcipvzf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2tmywevqb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cvixnekq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dhsdfioq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ptrpsqpv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lsogyral.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2alouestt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ugdtmjdg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2achrqtro.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wriifzft.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fnyfoxex.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ychmrxtw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vvatwjnq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xmaoqpps.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vxcddrsc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ilkcxyoy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wkkafyus.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tsjhahpo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2erstsnpt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2decktpum.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qhfuwdml.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qsdlvmfo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2yqtdrnen.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cjvvbjzd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dzlidixy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xjfvbtjh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ujrojwio.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ohwzdnny.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jtnvyzwj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2uesfaxif.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kgfdkupc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2fhxafbvp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kchzuhjy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yysfqrbb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cszblvww.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kvmnjgsl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gjthkikh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dqwwcepw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2orydqmiq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdelpgu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ctxqlmiw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2berhgukn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zwybhauc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kbmjvlsk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nytwlxog.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jvzvixgk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ejwwyrbz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ugotejxh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kpovqxeq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yymlbytn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2meyprkdl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hturpsah.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gznrsgkk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxfuysz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vgxljifx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2usfzggcr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lzqpttof.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xngyzlmw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bcdvgfem.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2upukozmz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jkuvqawg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ojdqvmso.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hufqbsyf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2chcqrpwx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2sbxjalfm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2iurdndbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esgylfst.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2urbmdcbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzjjiuoq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2uoliqsoo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nfrnhdva.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2fczykept.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2tmnjndql.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2htziwazj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lpvxjeit.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2summzjei.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lkiuhchw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2phehfdtb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2itzrxsxs.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2stzwetge.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qdbhinhx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2czwujwzu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dyinqwqc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2czclossw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xuslhamz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2aaatisxm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2qtjtnwrd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xjpnpibf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qgqylsqv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vzizwoxa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2flyjcwle.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fctihsxw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mcbkymvb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jzswbjwk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2eieneohh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jnjyrvoh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ctswdppv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tmcuhydu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wgxiivou.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rjbrdgxs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yhabcryd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2agcbbkwe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bkyhqxxr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2enkcqlbi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wyxionsw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kkktznnd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2fofdiatx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2svjerpqn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2psxvdfkh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2mzhslmxp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2leibwfno.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2awjsrgpv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rtvaodcw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dcmifbml.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2otocqoej.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uwgeojjt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vcqfdqlo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2dszrqgpa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kgwtwtly.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2iiczslvw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vczfetva.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2emhpfhgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2runmykyx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2msyuwyuo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2slwaejxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufyyfusb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2joktbxqy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2sywcpjoo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2shsxpbui.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2rnhwemvr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2nwcwowfe.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2iezwyjfh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2liuodkdj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2amzmryzu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2bgkhajhe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2yaixtefw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qeblbxny.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2lqzglkcd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ggqixvwb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vwqhluxt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2whoxuehb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2yjvwhfsf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2hfmmpczb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2wkwaqmaw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2krkkgdlo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2uqvohaan.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2taczeuag.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2duwrifws.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hnrlhzdx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wqiwmbys.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tasrlvci.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vkajjdoq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kyibrbtc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kfxobqod.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xsiufwbg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qwguwuos.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vbtfrmnh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ctxkosgu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xrmuctwv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zdoykcwp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pnuxkqoj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2usbjktvn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2czhxzxbu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xevblrfy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dobgynfs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2necdaokr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lhamwwwr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qmrygmtn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iwlvqipl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fegcnzkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvvlaqxq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ltbguksz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tulwsvmq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tkynrupy.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vnychyhe.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2gerisdjc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2akswlkqo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2szuesisu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ihhlxnps.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2strofudy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2bhfvdaef.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2reixjaiw.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2llhmfzhg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2jnjvebzu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pdrcotzf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fdtnxvmk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jwfzvicw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ggmldofv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2jbdnoeyz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2kqyrhwzy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bamnwwft.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pazomxsf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wdhwunif.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lyajzkjr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oqmhntzu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rrzbziln.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oezthupn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2myhhqobh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zigzxgzt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2snoejwbk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2iylhcsal.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mzxvhhvv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2cdxtlsfs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jvoovmmm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zvuucsbf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2mhgbymka.html


<!-- 参考信息 -->