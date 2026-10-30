代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gubnkgooz.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gfbcoafmt.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gbxehnvdx.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gskzofeos.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gtxvsbvrp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gcjqyzfzi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gdtufsbpy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gxirbujpw.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gsmmilzao.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/giwpoufes.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/ghcmvtkbr.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsegifhwz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gahakrlih.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gyfvqbqqw.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gmjtbflmm.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gfuvottng.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvtaripli.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gwibeqddb.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/ganegurjl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/giqetviat.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gyrnrqxjs.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/glieuzjed.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gejyhhnwp.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gpumrrhyi.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gphvotkvr.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gmteuztkd.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gaiwncvaq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/giwucrrmj.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/getyyasgw.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gfjckzdiy.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/giloqdaek.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gxwwjvxnp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/grgdfrbwo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/ggfkmbmrv.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/ghvslnygi.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/ggbdglmkb.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyxrplypk.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gzxfhzwfs.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gxfbeachh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gitmfjbaz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gcoltille.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gytcbzwvq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gtjupejqr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gcsxftqls.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/glkkuewdv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjtvixkrs.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gvrllthgr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/giqzwzcsz.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gnqxgyxff.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gvroufefm.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gvyxcelru.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/ggpdxtfhm.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/govsrguvl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsocdhres.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gkcyobeus.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gfjnqqxzy.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gwrfpebio.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gxjdgxrwh.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gcnppkohs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gehoudlsr.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/glsqpfnnm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdoypryz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gfehonkea.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gamcfxesh.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gjtrnkmuf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gozqjjrgo.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gwlubgheh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gujxvwgcp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/grjcxifun.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gbaxsvsyc.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gwomuhnhm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gvrlrbaeo.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gjvqzpvzz.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gopvtynds.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/giehpshjs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gjamaezfi.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gjlnmvdey.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gmjvryiww.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gnxltzskh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gcdhkvjez.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gwbcbjimx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gncduontg.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gewghucsy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gtpgiyuby.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gyifsmkbd.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gvedvcauk.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/guxwjbddy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gdjonlfag.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gxmuzbbxz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gozdiklzy.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/ghunqhpmg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gcmkkrbyy.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gobfwjvfr.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gokclregc.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/guawaoryz.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gtluejqwj.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gomlvpymc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gnxixfdsf.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gjagzawpm.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gwcqbuxnz.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gldfcimkz.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gthasuexe.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gvzbbxngc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gvgwwnomp.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gihaicflc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gwuhdfkcj.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/ghubebfjq.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gyzsmwgtl.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gorqodpid.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gasvuelay.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gasasscom.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gfjjbtida.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gfdnlbfnd.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gywwjmxob.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gmgoflbqu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ghldbmmtn.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gavlakbwg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gbddbqbje.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gvnyxfrrz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gdgeahszx.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/glnszvxkt.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gedaauoiq.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gibpjnveq.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gqvdjcmwe.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gmxnkzact.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/ggvszlkcw.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gvgtuhbez.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/ghmpalylt.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/grmlnuill.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/grhgmmawq.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gthdzdyru.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gvbsocrld.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gtaeekvpm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/ghflyshpv.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/ghiviwyzy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gvfjsflfu.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gfswnzygu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gsmxhiccu.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gicloyorx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/ghdlwfpbx.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gqjcsdhhl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gqmpavstc.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gqcedzxda.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gqnqlowls.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gharuofmy.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gzlgczkgb.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/ghexqxdfa.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggrdguxvg.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gmhffzxhg.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gobumjmpr.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/guejimlpu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gdwoysqtm.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gvykyxavp.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gaiosnmxk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/guskjpebh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gljseiimr.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gizfczcdb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gajqtqavw.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gxhrosyvh.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/ggysnnsbr.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gdtcqqnkt.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/goujsjeim.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gzcjyqrof.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gnudroeiy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwerqwnlj.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gmcaapnzi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmbjpmuug.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gebyugjwl.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gjwmzgznh.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gblkaraji.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/ggtvlhhkb.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/goinhafgp.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/giknmfflh.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gdjbehjfi.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gmxbouaps.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gmydmvexp.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gcxvkiysn.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gyplxqdjq.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gvcurheoa.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gciplzasj.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gwwqifzyj.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/glgtdjvbf.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gwzftzjbo.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/glkwgrjqo.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/glyrljcws.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gazrvgteg.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gmxmzxlrw.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gwoltxaea.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gswiqgqtd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ghevtlokq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/grmbkmder.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/ghskujmuj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gtsdiyikb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gzkhkpcqw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/ggflymmvj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/guiurjyeq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gzcssmwhp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gwzlanzmc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gbckslixh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gdwtfoetu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gpmmjbfol.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gkgmlisjn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gjcjcxxzx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gidgljcfq.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/genzwaaqz.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gyxzgfgnb.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gfhwoatwq.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gbojvpsvu.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gdrfswegf.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gaswuzwxy.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/ghudzthpc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcqakdkaw.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/girgqttdh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtdhdjswr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gmstybzfv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gcoptkfub.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gfnprxust.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gqvzfblnw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gahoxhofs.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gtztvaksv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvnwcgulj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gtrxobyqk.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gwbedmmnw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwjwzph.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gswcjxocx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gfuwjrmxe.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gqpjsjbbs.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gxqaxapoj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gmbkjjvyh.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gwpjbgugd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gbrmvlgix.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gfqhkedit.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gvazenmhn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gkvpknhmx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gesnqirwr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gjjklepqa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gmhzghcjl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gqumnekoc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gueccsupo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gkpowejsd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gayuwtkpt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gzoboravy.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/glzgsofdr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gxqzxripi.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gwdlmiazo.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gazrwrzlu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gjgwggxxh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gglivrrrz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grefholma.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gujvsqvwy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gxppctadn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gotxmcdfi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gcmfohjcd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gbirqsgtz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gpgsbinaz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmtegbdmu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gyzxkcnlr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gnrbmihfa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gmauxhcih.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gcftwbekd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gupsxejym.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gzupxgjhp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gyuuqhvgu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gmmimxkpq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gtnfjsbgx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gbgqyoytn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gzdlwcqyn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gtppwhtap.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gagjlrfzq.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gyhkhrnxj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwejsdekf.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gigceftpk.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gzposfmcp.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/glanhwesx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gmofcvzlz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gvidqxzvg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/guddkybfd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gkcmebhrf.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gunyjmhcm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gbtdyuxga.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gvcxcbzki.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gidakoaog.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gcxuceviz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gxylkcehu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gfhjpabma.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gnfykycug.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gcyhjnoal.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gwvlznruy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gmyyootww.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/glwuunvzu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gpgomzmcs.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gtfnerezg.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gylcidhkz.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjaphnjwa.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcjubtfcx.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gqeefjlvg.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gzcisnjfe.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/guloaaaqn.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gzekspeqd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gnyflxdmc.sHtML


<!-- 参考信息 -->