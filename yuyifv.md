代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pamkyxqy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gbovzgfp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2tcyavcab.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rxrwmdii.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2eymkganl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ieksohwr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fiyojvmw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lvynlqzu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zleafrrl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mbbjditi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2nzhjtstk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xyyjxxnx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywnprloz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dmtlgsby.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2snalrqyy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2uzkwzkds.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2cdeprqrm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jwxajiod.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xauflmph.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2waynybvw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2eibdzuyv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xawadrez.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cnniyaev.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qcofdqbp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2upkcwklg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2buudxkkh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcenjtcc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wgqqkege.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2uwbbbvxc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wmlrfzpl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mwhrxjyb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kknnzrwh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2yccplyms.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xbasphcm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tspsqhkv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jypacjyh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lowgctoq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vsqiuuao.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ghrixqyc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2szsmkcwm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pidjaliv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktnbvdax.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2drufhwiw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rfdfcfba.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gawlztjh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hdsjvqll.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yakdmwlh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2sicxgmkv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dzzmfjtx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2aidmuqpk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pxiptmxd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wuvuvqxc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xtjjmahs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qsfwfpzv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2agzzwpfn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2jkexlrlq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2uwhgsqwl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zfgfeiwm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2eoxgblja.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qkbkulxc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2uotgmlpv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2lqzfcbug.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fnoxuqoa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xoaspbts.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ejmoyrui.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2epscuxwv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2bsiyodoo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2iuumidxq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vgedepyk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2hsjvncrc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bpkkeolj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ojszglks.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2shocdzqc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2wcgmrktc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2fqjkyxnd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fydowhmo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2eneklcjh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2odfopgok.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pgfivlda.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2bvxeukhr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dmjzdtaj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2otzmtqve.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2iimrxldu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lgtpbaqd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mweqjrbl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rkgzebfq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ukhdbxis.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2yrfeplez.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fhgovfdh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bvwnbdpq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pyvpsezw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dxbazfbj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2klzqoyzt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2aectibyu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2eevwzvnf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2phbpnciw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vxenmsox.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hvgsdkid.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ztetbfbm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rlmikaxi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2izygaxly.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zddafoca.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2sqovzcfb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnghibkl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2jpusfdlc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ypvsvwso.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yagsejnt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vbgyhmad.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2skoxodin.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jodrwvrb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cexoaror.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mzcuplhn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fevmnwrz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hakqyjbp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2eicofbsg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2csjwormo.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2iixubtwt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yfcrwwid.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2uhscskkq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kvkpvpnc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2daoveqxa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dxbpokpz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pgfvuaxg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ftaggnvi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xeodlyrm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fnjoyops.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rncudjcl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2uqickdhm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lcsrdklp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xqujrzrm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2tpeejdec.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2biwpnwol.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gxsztvuh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bbmkgajc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fxqgspjh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2srypykda.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iyifqkjj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oqtsahzb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2psehdhal.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2lezxvkgb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mjfnnkmq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xktcfjhb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lnaukqge.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2mlqmeign.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zwjmzbvr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lyxzcqla.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kobdvdqx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yhjshsxb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cdlxpbcz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lnrlkowi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2iqvwdvwd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hllsaqen.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jxhimfkn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tifwyzut.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2cmvgxzxw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcbmakhh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tpwcchlm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rwkwmyap.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2lfchfelo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jqsuuyls.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vbhsepgz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ioverrxb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2bnthbtvg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wvbgrqmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmmpshqe.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vaxeqgip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exdetihu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2oakglxrg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2zotokvca.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2nnfzfpur.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2sxpwtwko.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tnfjbgrb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ymuatvkx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ollnlotn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uqzqrwiz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2croaiovj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dogpubjp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ayjgxzqw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lgspsakm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gcjkqjsd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vfosbvxx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ojfeaklq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fhtgmlob.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2soztiagx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vrwgztfv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ahviryor.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tejmlxto.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2cbpxmjet.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ejrpisyd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kvwbwugu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ftcnkxwj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gmkcijin.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dwvyzmul.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rjpxqsop.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vcaxujsp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lbwqeasq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2knqettus.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pcdshxlq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rgqsajat.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pplirmwz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uxupnmga.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bkaulzyz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2kivkuidu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rqzdhrba.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2xubiqzps.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2yioqobbw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2sxakmcqh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2faolrscx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hdbdsxjx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mhbxixei.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nacbxjkq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2scqxvfsp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hghgeetx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rmxlkldi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2flgknyoy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2isujmijv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rxapdocb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2wmfoupil.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2tctncayu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2diocoail.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aychvfyx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2guihitef.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2samuplwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eucejifr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kbltadaw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ysohqgqg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2tlwghwmx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kfoqftlq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jvlcaiyn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2eypuimno.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2amsrjzdc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rfvtknqd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ohudxyif.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2npkkkuuh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2pyvuzweo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2llcxjffj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2nuxcjnef.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2whbimvwr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mekdjlks.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wepnxikq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ssgwxkyr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2nwfiqstc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2hvzqmjwf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2gogvbkjo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hdsstufa.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2lxrxoaum.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yemgxgkz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dujkszyb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nqweefep.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pjiyuayq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uagfriqg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dqsnvzvx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2lfkxhmbw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wxuzpyva.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shicqgte.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbkumnor.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjrmtuap.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wcmusvgm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bqprysrv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kevmmlts.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rrzpxomz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2znokowzv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fodgrlxa.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ulobddai.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bktfctsc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eeexhvol.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iqqygcoy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zghffvbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sayrolmc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2chmudndv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egrksbqz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkichhxc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nxvnadmv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2iabuvuci.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2piztourh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ewebrfuz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ubjgdeau.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2berficyf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ulrutamq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2thskabxc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vpmvpgwr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2mmpzdlib.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cndhchkr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ofbhdjlw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hdbleeob.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sgwfldcw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2pxttwqjb.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2emmaytqs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rocxsdts.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jdfembkx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2bcpidpmv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hizniyxf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eraekrdt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pgqhzrqr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uwgypawu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vueybpcb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vbwgbvum.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2czufijxq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2yipqjngh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2jcbcqppp.html


<!-- 参考信息 -->