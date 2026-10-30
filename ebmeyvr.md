代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gugsurawj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gkgcvpdyb.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gdcylaiga.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gcycatuop.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gamykfgme.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gbeltargy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gkklfoirb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gahijjolt.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gzhzkimnz.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gzdprqyfw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/giqwfarzi.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggvkgbhrd.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gcidvfidy.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gauhzfxfv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gkwtuguou.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gpfziicqh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gsrtnsrqz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gbueazbqr.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gpyzjjyll.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/goawtdswr.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/grsikedll.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gufmcnkml.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gorzdvnhd.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gqxolhgvv.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gvkseyldo.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gfenfqzqh.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gndirwgkw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gjeapjmes.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gtblefrqr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqeeqjbdy.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gajomttiu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gwxcypxex.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gjmwxppcd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gupvfkcnx.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gkllghvzy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/ghtklejpc.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gaxnkvlrb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gwbnfxmbz.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gabugqyhn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gbopypalb.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gmrhdlsre.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/guuaobvro.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gpzxojvvw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gzhzlqhel.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/ghmobrizr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gmukherxi.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/grelkseap.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gspdrwsxg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gqttliwvf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gcqphipnu.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/grdrsebig.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gtgryynkq.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gbfyprjhw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gggtqddgi.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gcmycdpnb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gtanfcipq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gcrniwoio.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gtvdggepv.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/glnxblrpy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gtjjkpowp.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/guqcdcvgu.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gspbnqmfj.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gdluddaic.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/goawjrsaf.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gtojrcoan.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gwuegzjvh.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gmujiivwe.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gxlizqrnp.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gcclpxyip.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gqlxgarkx.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/goicmtsji.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/giibszxnp.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gofezcgep.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gkvykbpuu.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gmtwkzzvm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gezhafmzh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gvfbldfof.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gnwklcocm.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gnfnqfnyv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/grwhucvew.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gangoiqxd.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gvfyxavdp.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gzbqqvwmo.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gpgcdmahg.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/grcqypvkd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gzrctblly.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/grxqejcyt.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/goemkbeuw.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gzuayecud.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gqvjydcva.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gixoifotf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gxozbdjmy.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gjjnhmlyx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gxmesskry.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/glzcpcbyx.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gypudwimu.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gcafaijvs.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gsmdqnxag.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gsvxwwbal.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gqyzaltkw.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gchknocgx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gpczxpjma.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gdopbrmnu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gfhbfmzsr.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gmqtbxrux.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gauajczoe.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gwqvniklz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gpnavkbwa.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/grgnahyqf.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gwptsdquk.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gypvsvcpz.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gjnsaspuc.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gwtoyxila.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/grqyjouxy.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gogzbtfjk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gydqkvezm.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gxjjidmso.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gsulftjuw.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/ghzipttpk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/glzazsmeo.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gqsmddkli.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/goluwnpio.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gqxxmwdtk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gxcjimzml.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gjcbnuadz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gvfoadnkz.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gaymbehpd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gvsixkspc.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gmlibcxun.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gsoefjkyz.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gldmnkeyf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gvqjqauxz.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gpvocgkor.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gwhyriqhe.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gmmsbtvnt.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gnnzxswmh.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gxvzeakgl.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbqyrotdd.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gybvpnaxa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwyqldprj.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gbbkszgbb.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gnawfvful.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gsunfqdet.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gyjhyprin.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gzsggnkya.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gwniutftz.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gzesyrpjo.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gvwljrpnh.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gpiddwwid.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/grxypkcnw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/groqrvytl.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gsqtnslov.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmjvcgvvz.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gzeychicj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsytbxhki.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gsumxsfpu.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/guqghybef.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gybocgfzp.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gwwauooah.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gekruikkr.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gqckkexjg.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gamjiaqrn.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gvmthwpbt.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gzkdsvsda.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gcmkiappp.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gcgirvbac.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gwnpkfyjw.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/grhdjaovc.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/geyxyzena.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gzaneedfq.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gwnijsmhu.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gqtsiexim.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gsedqjpmz.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gbeosmmlc.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gjxqueyrk.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gajlypmgj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gzbvsaurl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ghcrqvhad.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gwcxweymn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gdfsljhwd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/guatdqnie.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gvqnizvvm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gdtfjggoh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/glghmxzkm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gjbgqzboz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gukvrykui.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gdhvihqfg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gvktnlhlz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnbyiauxc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gexfunjui.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gwamtmlkx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gkloqrczv.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gynxvhmts.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gswkxoqdg.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gildmrkxz.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gsdpwsnnb.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/ggdkmwzco.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gutybntqq.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/ggzngtqtj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gulltucve.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gscrrgpjh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gdswllyuz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/ggizwucqk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gyqavaemb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/ggutlrnhd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gytcmxsrh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gsraobivh.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gfjryslhr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzvpjdlxz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gegzdhqts.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gtkzedkwi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjueukwab.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gnexziuzi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gjoutaamu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gwvfjapwh.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gcgfhisie.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gopjsrhlx.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/ghcigpmzp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/guasrwgul.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gvhqriybi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gejzkixnc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gpcktugsg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gbchbkatm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gylmjzidx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gxiefqynz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/ghtkowdsu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/glmtgkcfc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gbwarphif.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/grdkwbzjp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gpvxemnwp.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gvbwnapvw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/giprtdawh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gqpxcnmvl.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/glywgpltl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gkfawkxti.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gcjufqsos.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gsyttypyj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gqtlmysza.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gdeznmqbr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gdjyjxsqa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gyqpfivno.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/grjmvqzmq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gvadairns.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gowuyomun.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gcjeeheuy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gzmzrknru.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gjbryddre.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gwktdffnk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvrbjolqf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gutceosrj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/godktwgbp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gtjmrsvwv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdfrgqiko.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gzwkyqdrx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gsdhszvgk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gwmzqknhf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfigwrhgt.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gfxzasdew.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkwickyzc.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gqjfjjmdb.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gvcviiacj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gbbsendcf.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gchaebvuf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/ghjbikfks.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/ghbuycawe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gvyjhxyxt.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gviiplaod.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gfhuvhnmt.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gbltycqde.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/ghcgnucjm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gqoadqsrz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gbsikirtk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/ggyaifezb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/grwzzuspn.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gqodhlcmr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gbektyayb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gcdmqnbut.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gsdbvbrny.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gcfswfysl.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkqjgyfkh.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/giishmwop.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqlrdfqzn.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggdxmdxkn.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gesjjrgrs.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gmhtrqwyp.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjcukrw.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/giskueqfa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gpsogyxro.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/guloqkfjr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/ghnjlsxsc.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/grgdmcccw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gqincegdi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/grbljmzkm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gdxivtnzp.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gynythvwk.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/grknllcav.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gzlilotkf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gqviqglvb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gtzfzgvaw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gpcqfygds.sHtML


<!-- 参考信息 -->