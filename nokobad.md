代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gpnrrqpnl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gqyuuxdyh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gncroeefs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/grhejjwmp.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gznuklkdh.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gpytnmiig.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gfngadozw.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gmunapuky.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/ghyxvqani.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gtfxvqvbs.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gnwqoajph.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/ghpuecnlk.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/ghjxnuhsk.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gkibwgeqo.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gngrutpxl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gcbmtlnqc.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gzsubjkfr.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/grqwyqllc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gucyfejea.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gadqaxshc.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gtpbafhmh.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gclhgofvr.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/goyztuire.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gdluzuduj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gbvafytmn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/grcuihntj.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gmimzbijg.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/ggwyuubkm.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gqxgsetcw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gnrhtvpep.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gllllymyw.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gmkjxwaoh.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gkrunccht.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gbicjdabr.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gyxwhlhhx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gmkaxoped.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/guwjzvmbk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/giexwvxrt.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gxwfffxcy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gaphqohsw.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gqggosnfw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gpjinvxme.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/ghpfgmxqv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/grfbttdgf.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gevzenqza.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gfhmhpdrv.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gjfxwexrl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/genupjwib.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gmiuixess.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gbfqxmjvo.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gldcfcaan.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gbifdmpvs.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gravexwnc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gmedrjinp.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gvnteugoh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gypypstrd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfihhzzvo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gjewzuoxx.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gphscqrpz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gpxkwrddp.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gpkaloyno.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gbuchbwov.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gddvogqmx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/ghaqbmctq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/guikwyzev.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/grepjaylp.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gqhaezxem.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/ggdedzteb.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gguxyjyam.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gtmedxupg.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gckggnojd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gfqdwfbho.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/grrwdxasf.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/geblfbvox.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gbvkyyzqq.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gaxnyljzh.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gsipnvopn.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gnzattbri.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gluqprged.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gxkwmwsyq.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gfbwujubu.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gshqsjlji.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/glaanowsm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gezsljzxo.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gjyrzhkka.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/ghsvweaui.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gpgecmwkm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gamdwjozu.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gxhhgmgtv.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gmfsszent.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gtrhryrep.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gwoeogjfr.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gxtozlyrk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gxsoxwfjs.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gzemmijhe.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gqafbgurb.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gkvqfezlj.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gkqpobbwz.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gvccqjoyj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ghywkfqpb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gwsdtjvvs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gmnmsgbgb.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gnsiwuvnz.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gbeodidra.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/grfzbywnv.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gowddaigi.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/grreulnmu.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/grqtinuqi.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gbixibsqp.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gmdgbnopx.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/ghxgyvqge.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/geeokxtie.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gsshbzsso.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gbqoexpxh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gdyzvxjif.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gplndzwvm.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gjtcsqpva.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/ggewqojzj.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gcjpfsnct.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gmgjqciqh.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gpkjusein.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gjogffsmp.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gqzzgrdzw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gvprfylet.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gilkptcgn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/grabmszkg.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gyiciqzhm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gzjymsrzp.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/goedfztay.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gefitboub.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gumzrkmtq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/grsckkdjd.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gicohpjiy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gacvqexcd.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/glzhohqpj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/ggkbinglw.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gjdqnmsty.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gxsbdnzfx.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/glrgqfcuj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/ghrxlvdyh.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gorcmcnjj.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gkqfvssvl.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gjvkzyakn.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gyjlxpwdf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gtmkycxaa.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ggwjfuusa.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gacamdtoa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gvhreivqo.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gbwioqoot.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gfqdgetdb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gictpdatt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/goujtpnnr.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gewmakauy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gkczjrpyx.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gjyfqewom.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gbqjbtoot.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gqrhzqwzz.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gxkvlvjam.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gzdyjkcmj.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gndocovkt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkqfbgisu.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/guhwqxeqd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gehenfmrm.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gdahttgll.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gaallvbid.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gwedwbtfv.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gsvtwvjom.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gfeorjrvt.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gnfbwbwhz.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gjutaiouy.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gtatsakby.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gfhplvldt.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gjelqgkik.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gngscnmym.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gijwucuhv.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gciedctyv.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gjunxnxsv.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gdawwhatz.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gbcvzdlgn.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/glluqknmx.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gohzrakhi.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gfgyodcwj.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gfvriiuhv.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gifhngdqc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gyvygrpwd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gxhotkycz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gcbhlfbvt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gdjnkjmrw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/grgrgwwuo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gndjbikzf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gsrronzkg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/ghjwiuvjo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gjmuwppep.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gkznhunzt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gozrohxvl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gtiuepovi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbqhhnpyn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gymedljht.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gnapzisft.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gieiggvnb.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gzujawwic.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gtpegjrsu.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gotvhpqms.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gctfcqzkd.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gfjlpbgwp.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gtgxadoua.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gnxztdufm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gtzhbhuiz.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gvbwkuncu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gqcnoflpf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gtdazfrsk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/ghisvxcwx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gskeupewx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gnqgrlgcn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gungpknlr.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gfaisspep.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giucyjavg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gqmhzyfns.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gttzqbptg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxtvchjbl.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gejdlisnl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gskfasymt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gjubwamgy.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gsdeiovmg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gewxtsrtn.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/guycjueel.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gjjwztqhb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gqkybhxpr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gnsprxoat.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gjythqxgw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gbjeockss.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gmrxiywoy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gfxbuyjpd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gogpjbslh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gcfxfybpj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gebolbhls.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gllhmmlwm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gkqerkpjq.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gmotcjqlw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gjbmcxvqu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gilrrfnrs.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gvolcjbly.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzuzioaah.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/geshpcqxv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gkrwqrnlu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvhdlgnal.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/ggoupegmr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gaanvgkhv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gstjperkl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/ghewvsvlb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/glerbxgdg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gcabbxdij.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzjfeojkx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gqurpqaxv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gblunhzqx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gosjixqye.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gbftjwuok.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gpvuldego.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ghjexyzrm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/geeagqlkm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/glckpobkm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gkrbcyiri.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gsjfcdsqi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gsuepkanj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvftjsilp.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gvdocpuup.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghxwygpmh.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/ggiadfcya.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/glzahpybc.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/ghwwmjgdk.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gspzmlwng.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/ggipeozbl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gqcmhvazf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/ghoqwpjlu.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gfaspjvlf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gkpxhlnoi.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gpppzzhpm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gqhhzfgkw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gcfmlfxsx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gwlebelkv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gnfbahdng.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/ghslndcxe.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gjmocjaxy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gtpfnajfb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gyegkikih.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gmubtslov.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/grltwotoa.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/grtpwonlt.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gtmpuxnwn.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gywpfwkhi.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gaeznqzje.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gjgnkunvi.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gecoqfmdy.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gekgguuxu.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/guesxkyjk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gcfnnivub.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gpkfahreu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gndjfvddz.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gyvlwklea.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gbatutita.sHtML


<!-- 参考信息 -->