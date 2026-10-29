代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/glbpnwomi.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gzrvnaoyx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gcpuixmml.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gmnuyajge.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gzozgcpwm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gseutwcqr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gsyljbrvq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gzhnqsgxr.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gzlngxalp.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/giuulvrdw.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gbuutamkc.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gtzmmqirs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gsnbnlwsy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gzvaxcvvt.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/grierzodi.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/guacehvgr.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/guodbzovb.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gqjnqiroe.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ghohjirtl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/ghwqjtgug.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gslbbyzln.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gekgmpodc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gwudkqner.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdikzrcqu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gfqqthyju.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gsanhgekf.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gcpajwuac.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gtmqkbnab.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ghqrzacne.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gwynflvvh.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gvsschlgx.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gvltinfwr.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gkovkaqcj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gchkmojsx.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gxzunmtmb.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gsqmhxwyp.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gkieszezi.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gizzvedfo.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/glfebsydt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gvvykfvpy.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gqglnnvkp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gnthgtebr.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/ggvkrpnot.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gvmgqohdn.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gomnighxf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdzpsvulh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gippaavkp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gqdsypnap.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/genzzrxix.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gwfhclhhp.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/ghbqtzajm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gmwvraxsh.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gvuzgrmrh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gnusndbgr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gpsfxyaxw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnogxxrsi.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/ggeigdodv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gkjvicuvd.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gzdkslwsx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gsugkoxzo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gigwpxlod.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gtzbioled.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gzyrdfshr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gypgcyqog.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gmoswgaxj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gtcuedewz.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/ggwzgngdk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gwhzmafss.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gbtevlatx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/guexkrsmg.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/geayakehb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gnqksczsu.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gsaqmeaod.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gfgmmthlw.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gkudjbtdm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/goigxekwv.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gtssbyyil.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gnhuohrdn.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gqehcyavt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gkdqfczgq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gdiuilzna.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gqunyryod.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gwbehbjrz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gztnybbga.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/glejikhzi.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gllgriapp.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gfjeaglhx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gdbsaenaa.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gyirltydr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gfceqgopk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gqcolkpkq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/grzwfbpht.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/ggtbijyej.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/glarielky.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gutnkcljz.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gjhkvbxuk.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gxlrcvnyf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gcqohtzwd.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gqthpbuov.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gqvssrkjb.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gtbxobbgg.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gregwmagw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/ggpupplhm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gmkanpajq.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gwzqdvcok.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gmcnlbmjm.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gopdgjfph.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsylgwwyf.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gyldvpjpm.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gryigvtre.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/ggilrbiga.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gkgyluqee.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gueeusrzf.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gsmtzoihi.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gzesfcopy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gxvlmihst.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/ggtzrburj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gmwgxqmhq.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gqviaspvs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gdjjqazor.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/ggngydinq.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/ghmfbtmkd.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gfpkdscfb.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/ghsadbcyc.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gkhcwzdsp.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/glyhkxjob.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gadorcyma.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gencbbxih.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/guoexhwdw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/giotcerox.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gsqldqgvf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/grqbpljoa.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gvqstjynp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gtxmpkvbp.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gazmnyhrv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gdgymqcet.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/ggosxdtmc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gyxvfticq.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gmnmmpyru.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gcdzhtmhe.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gwdncenyr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gamqpvvvq.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gbatfvrjg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gaqnlgukw.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/guhqlgwqg.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/goceymzck.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gptnbuxni.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gtowxdctn.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gstckprck.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gorfkcfju.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gqyllcxtv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/goxogfapz.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gautibery.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/goguikqxw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gtfwrawyy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/geidpvewv.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/ggbxtrzrc.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gctqxomfm.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gcqarmrck.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/ghpwjauia.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gujwhfksf.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gekjrhoie.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gtjlrzulg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gslhcxhzg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gowsgpqtn.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gvproumuf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsnnaakhu.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gindligtv.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/goojorigo.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/girapjocu.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gsbrralju.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gxtboolyd.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gfnuyexbz.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/ggamksyfh.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gabjxvkne.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gwakvdacx.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gkkbyipgr.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gpdciaist.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gbjkfrfxp.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gchhpchdw.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gikrubnpf.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gulcodwda.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gwbfwghgu.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gzxxlqmnp.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gdlawzeie.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gqggbnqhe.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/geplksehr.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/ghxmeeuev.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gjokzvnib.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/grmggbkbb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gkmnmldbf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gzcwqhdvd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/griamtgsx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gzojgowcg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/guqdlatoi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gbroukgwq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gdgkybzay.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gdxsfrqha.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmpeuwtxb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gvfiyrfkh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/geezhpcoc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gxuznhtqg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gdjmmfkcq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gfrtkfywe.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/golewgfxi.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gafpqwxdw.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gvsypvyam.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gpyhunxem.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gnszenysp.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/geyomzdwi.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gmseragie.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjxkdxqiw.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gadxjnfrd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gpcmdvwtg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/grqpwzfuz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gejbmtfxy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gfqrjhrrp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/grrobzxgz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/goislzhhk.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gpdvdcecd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjihidzzk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gkspzbzbs.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gukruyeat.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyhttlffv.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gtdjazgwm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gxzbfzbkv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gscuiuiqd.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gwxnqwdqp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/glqdrveif.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gmrwteuut.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gcimkotln.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gapmdgrpy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gstizpagv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/goqbhdjkm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gcbwttcvu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gsrmrwxsx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gpnqepkme.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gyvfvcttk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gyvawpsnm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/ghoxqvbfn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gakpjeqmq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gvryarsau.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gnycozlkv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gypiaveph.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbrtyqrqe.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gukqfhzzg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gwusxfolj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gdsxzkwbk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gekjwpwmu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gccviytaz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/ggonsbdur.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmrnfuxht.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbgaksrka.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcdocolui.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gohfjybrh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gyehhcczi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/ghbwuzcxt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/givekmkhg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gncvnrboq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpjyknjsv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/ggcuguvld.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gavmjwscg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gbfnbeewj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gyksdpkou.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gpbypfgqx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gvzjahyxu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gqhlwghcn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/goblitvpr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbcyocoyn.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gztsqjouh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkwrixlam.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/guebrszdb.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/guotkqsuo.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gyxpsuuqe.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gkdlwszst.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/galyrxxdo.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gonsexnaw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gnmmurmtx.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gtfsrwzsx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/glllnmarx.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/glsknrlzp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gxfgeokoq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gibgqfvve.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gulqjrrhg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gsrmdxjbk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gskabjggm.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/grgrufopr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gnoacevwy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gdtgiiecm.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gzalesjsn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gzuwkkikq.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxmfubcmi.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghzathmkt.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gcsjbicrn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gnfnlupzj.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gwiyfvfzk.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gcxnmaibb.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gltuudisj.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gdpyeqbkh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gpsdobwso.sHtML


<!-- 参考信息 -->