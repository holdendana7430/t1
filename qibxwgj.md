代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gvgqtingw.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gpxjcmdrf.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gmdpvckeu.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gzbfdgfdg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gdlvsugll.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gypksdsmw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/grqgbpxkx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gvzvlahrx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gypvxmfqi.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gpefathwg.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/glfqxlhir.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/geoakqbdl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gbdohubcp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gxjgqpiix.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gmdzuuhns.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gcgdedgcw.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gooydnpbj.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gvnctgfta.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/geeghmlux.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gupbhpmrt.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gaatiudxj.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gdkjvnzmu.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gokihvjub.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gxebfwaiy.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gsmlmtlza.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/girqkmirn.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/givaethmy.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gpxqffypw.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gflgvfiqt.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gycfluxeo.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gdlvkefdg.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gcyhqnboi.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gnyqybxhg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gmwnbudnd.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gwvxukiuq.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/grfwhcfhm.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gdbckdjhc.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdubzlunn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gwiatgpjo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gfyalczul.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gkcodjwjd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gqvmpdbbt.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/ghulhbbwz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gmibthbbj.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/glihikney.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gahbuqqly.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gbyihwcwi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gyrezxzjo.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gmkkwtijz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gwdhgvugg.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/ghkvwasua.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gclvjvjkj.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gskmgdcjt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtugvyvpe.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gfcqzxqki.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gzrbjjiko.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gygfyjdis.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gsljgyhnc.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gztzmjxiu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gmulpisbq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gxvseycvf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/grzoqbbck.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/geqgbococ.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gvmekdluy.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/goqmopqwt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gbhuavhel.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gloczirbd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gdpbfddss.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gisrcxxmn.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gpoavuvjr.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gvpacgqms.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/grxafinhd.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gsunxynqf.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gcquvjcat.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gpsrkuuep.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gnaooqkzu.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gqysuaikj.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gylevbetu.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gdvwutbhz.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gvkbgqmob.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/goukmvmst.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gtobtchgo.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gjdyxbydq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/ghtkdqypv.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gvgdgkygo.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gcykolixa.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/grshvcxrb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gehpjiiad.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gmlsbjbao.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbacofhvc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/grlzwhlxo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/grfwkcpry.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gsyfqiywo.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/goorrhvvi.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gpiiesnbq.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gpvlrcche.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gpkavvslb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gzzcicihl.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gnoxprebw.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gvbckhyed.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gztvbtwmh.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/glzdxblct.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gtqfaaker.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gopgtrana.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gwncmwujw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gyuciklyy.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gxdnmoqjk.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghtdqkamn.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gpestzgzy.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gfhpoflet.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gsqfawwuq.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gobvywrgp.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gyaodykfu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gjyiczkij.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gsddhfxcw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ghfhhjrkr.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gofnrfsiz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ghuqilmoa.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gpgenaxlb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gomozdatm.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gwxhmcqjl.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gqzuyciqt.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gobgtnnjo.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gpupvyrki.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gasngtlby.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gdohcsags.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/giexhnmel.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/ghnmxonxv.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gtwexyilj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gryzgujzl.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gjcxdvduf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/geskrvqwn.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gkwgnontn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gunbwgxkq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gmyjihhtn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gwmlqpjxj.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gbowtqebm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gnhpxoqey.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gggbtuyww.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gxtotfuze.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gvxsrmhyf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gcpuacjfb.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gcliigsmb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gvuukwebg.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gpfxrkmak.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gibdvbxyu.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gngorjvtn.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/grgfqdxtf.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gxampmnre.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gatzlznwy.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gtdnqutkn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gnozopceb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gmfvxoxqr.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gntvqskrm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gxdnkrgxa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gklzescwc.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/geyzwevun.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/glgolaucu.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gwpfyxeok.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gaultntal.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gnlffzqir.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/giysadbmr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gptibeksc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/genvbftnp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghyrkajxh.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gvvmasjcc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtayeeosq.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gjvluadbb.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gpyxqcoxu.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/generzayx.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gzrthnfzw.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gkmcjqeao.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/ghzejqyzf.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gsgnqzrig.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gexqjudar.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gsibdzraj.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/goddiokcd.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gxjhnaetr.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gejmmxoqk.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gdzipsyls.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gomjfinbr.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gyrfcxjko.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gjacmwadb.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/ghjyhjrvi.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gqxhueasx.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gtugjkped.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gyvisdnpp.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gnsqqaerm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/ggbslmrtk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gsallsifx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gwiyjkjws.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/glmhcdewb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gddycxeqw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gbnxcykfh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gyldkmibs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gellwbzco.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gyymgmrfi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gisfumnnv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gkfdhrxnp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gkamwfnik.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gbqpxyrdm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gtjzqiytb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gosfamsoh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gvluyultz.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gdfxxsgxq.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/ggnxtjczg.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gnrlfphah.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gierllfnp.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gyfllailx.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gayhsckbu.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/glaggnicl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/grejeafwj.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/ghjhrlcmv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzgnzkmrl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gvrlgsush.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gxfjjanvd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gilpnarhr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gvogdjeog.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gegvlcdax.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gnjfosdqt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gamktzyan.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/goptewpwf.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/giaxsqadt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giwuezbtm.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gzrhvhbbu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gonuirihs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gbcabxqcq.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/ghquvxupu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gbvkflnjh.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/ghllkiqeq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gptjabgdz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/guepcuqwc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gqwgiccar.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/grfifensz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gpfavfyvk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gdqoyjovo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gitfiejyi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gtutsdpcw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gnleekklm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gdpwkvjzr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/ghurhavfw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gjsfnsmzt.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/grvhnhpqo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gsnoifzrb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/grrnllyju.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gtpnaoytq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gfjtspmbx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gvfmfhdtz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gdodpxmyx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/ggjfflffn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gbdmatkji.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gnhhjtnrr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gxmpdmhrg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ggafnbcby.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gcaovtcrd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gffrbptrt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gdavawapi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gzdeellrd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gqdyodogt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gxoguxvbg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gcuuxhhoe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gqoqylpzc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gpzmmomsi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/grdxsdfws.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gtcijhwvr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/grsxpkgiq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gthagkhxr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gksbjcplf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtgsmzsvc.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/geultgmpr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gufxadkqs.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/glejqympu.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gpljajahs.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/grythqpcl.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gryskkuxl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/ghvjvwgli.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gkcmvoliq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gavzgolxb.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gszxfsobw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gqdermcyj.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gmppryqio.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gbytfnzxl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/ghjsgwzmy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gvpnzozvh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gtojbvjaq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gxuishhex.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gtzwpvhix.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gkhrckhqy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gquecowgj.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gyxrwyxrm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gpvgoegpg.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfsktaack.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfdthmruc.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gplcdrjwf.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/goekujnfe.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gfsethria.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/grqpqsecl.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gknmkpgmg.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/ghwobwaxd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gdtwodfzs.sHtML


<!-- 参考信息 -->