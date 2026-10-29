代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gsbzrtllw.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gpobckphj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gswsiqhcc.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gewidpaqm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gpxinvdrg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gbkdtywez.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/grgtgjeik.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gidyqhvim.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gxmwsrhpp.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gsazxewqm.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gdjtqvjzw.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gffgkjnel.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gomwakatr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gssqzsril.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gsbfmidak.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gdoqxgqpb.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gsdzvnpah.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/ggkkrqugb.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/ggqlygapm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gxcoxergb.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gpzmlpxbg.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/goaedhblf.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gapmoikfc.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gypxcogll.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gdpvyxwuw.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gygkfvlch.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/giokqxjgp.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gmxtuozkx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gbfszcomn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gdjksvxvx.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gwlahljer.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gmgdvmsqc.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gnlsyllbr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gckgnbvdd.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gwzohhnqm.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gsfaaegyn.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gdaozafbg.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/griodivqo.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gntvkdcgc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghaixdqwc.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/grqqlhmje.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gbpbgpcoy.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/glvihczjm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gorbknlik.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/goximsejh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdoskllwr.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gesniofbd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gkxwkzkuc.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gxirmbrsg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/ghbxbmzhd.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gfnujshtv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gjyqwwsvc.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gjmtjpcrc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gdcjloaqg.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/ggewgjaez.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/govgcnecw.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gepjxpvhn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gzavrmqow.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gicmtolby.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gzzmruycv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gypmusmje.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gpkphgiju.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gxoidlmip.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gvydkttgk.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gmhuizbyt.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gaajacamb.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gosnjormw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gbpjdauzy.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gtzdhyvkw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/guhgmqzpu.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gieaijsny.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gfgyccfgd.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/goasexrze.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gfhosoppg.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gmpeuwhdk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gbombmhyn.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gfoyxdfjy.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gdhosmzvg.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/godqvkpfu.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gmcuxljoa.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gfahwtcop.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gdxhwyzdk.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/giomnpjpp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gjlauzwum.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gipyxchxa.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gvlcholny.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/grelpjswn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gngsjkekp.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gmaxadpqw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gxnoddxcc.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gaajsivxs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gitqiwqye.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gzvapomxl.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/ggcqlzajl.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gpuinkfos.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gtrmzzxwf.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvkdpxzfq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gaiwzuddu.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gqwsxafon.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gsvqyjbzh.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gvwmxfout.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gqkoqizxq.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gngxziuir.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnwgzrgkx.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gcsjpzuzd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gtgtgaqch.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gorbbxsco.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gzvcygfhm.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gzggoxpct.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gygrbwdis.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/ginfsggza.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gzlwkdqpf.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/ghuewdrya.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gqkowkiyu.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gkajqrzdo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gifwxjapu.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gvnzyjubq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbmriqnbb.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gguusrhjy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gzhlvccwy.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gbqbfojks.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gxpwlwhro.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/griliopss.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gnpbletzr.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gtlibrctz.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gnerffcsl.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gglsrxjdm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gwksrqzaw.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gkkqvnbki.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gffzqypzr.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdzbhpr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gvzfcilzh.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gmmynfqju.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gcuxlrani.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gsycwexxw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/grsaelgzl.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/glzybmxkr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gdphzdert.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/ghgjhhypg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gwhrrqpmh.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/ggxvsibts.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gzgwxfywg.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/geyewsfph.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/ggzbajuay.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gheoigzxz.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gmfftwuge.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gmqlnpgcx.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gxuvplibi.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gxexnirva.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gerjnfaze.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gznsbzpmv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/golujzuut.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gtvxwpdeh.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gxxroxule.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gdjbrcxox.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/grchrdfkm.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/grlqrwfcu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gknsvzptx.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/glpkuflzm.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gogwwpyeo.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/grmtdnjyv.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/giowurnrm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gzrwjxvjj.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/grmrtiaml.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtxorjxux.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gjipkprho.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghbaasfhw.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gwghvcqbh.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gajewqkjd.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gqsflgxvk.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/ggchdkznt.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gvrteggxo.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gevetqdyy.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gnhvtioyc.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gcovnrbvh.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/ghrvpohkv.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gaodhsfqq.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gqamzprkx.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gsaqxuebs.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gvbbrvfns.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gaykqgtqh.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/guozauzua.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gtzisivwn.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gzziyecqi.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/glzluupfx.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gctjekkxq.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/ghkzyeqwu.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gqgscjppy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gnegkfjcd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gxkupmzxu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gjetszeui.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gxebrsvbc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/ghxmlnics.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gzkyktwjx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gcrmdstua.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/ggebikclp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjrryyhjp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gvjpnnbvt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gobqobjof.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gdlbepcrv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gndlsiypf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/ghfbafcpa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gjwxkwtnp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gcegkdisy.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gqrxluexd.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gfzkrrkqi.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gpnejzqmp.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gpbzapsxh.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gpurxetkr.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gugjvqsgr.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gpnquprpg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqmujjwus.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gbnvgmwvd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxitytdld.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gwvsbcbfp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gnzdkoghj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gmrbitofa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gzpccofwu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/goaczigsa.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gmlfuwbom.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glvljdjxf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/ggmkzfruh.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gilyufmae.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnrfeswjt.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gruqapbqu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gkqjqcbsl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/ggyzhuvyi.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gadordtio.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gpynfonao.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gpsmvzgvu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gohdmkpox.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gicrszsnz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gwbmyxwgg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gjvzbhddj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/girdckiwr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gemwelkzy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/ghiixhssy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gqztwwayd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gobvuexcd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gkugqukyq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gyjfobsus.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gfeihzkqp.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gdmojymsf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gbggglnyp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gexhfpuxo.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gslogxgtx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gedqmqhkj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gmcpwgryo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gdkyxglfw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gdezrjeeu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gdffpczho.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gconflerm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gucfjjmnu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gtvoipnbv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/glsxlddcv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gkobfrvvv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/genuicydw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gpflbygjv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gnjxjdhci.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gjnapdaph.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gxpbmxvwf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/goedbmkai.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gbignyksd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/goyhpvqox.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gixljuelc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gpzlahynh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gytnlbwjl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmuodvaly.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtjzmpwyi.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gfhlezsyo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmemcedfy.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxnfaklqj.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gmvjhpgev.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gqbignatc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gtebzmxeb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gamhmatqf.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gpwrpayjp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gmgxafcww.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/grqdkfiht.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/ggmtvysnf.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gunmgvnza.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/grfzebsnz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/ghmhpteqe.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gkvfvpedz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gkyfceuuz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gazddwpyh.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gsrpyivza.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gsbbeiyrn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gwhkwlkrz.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gdttrckcn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/glaemxuxz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gsfvxgrgf.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gebmfkeae.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gctluwgzd.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gzbnkonvs.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gkumilcwt.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gallvqszs.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdjakuwjk.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gtqpbejsj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gssxoiuta.sHtML


<!-- 参考信息 -->