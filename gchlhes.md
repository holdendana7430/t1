代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gmoaqnnwk.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gubrzwpuw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gzktzyenb.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/goifttlgt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gbbamchuv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gedtcefsx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gtlspcihl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/guswbezhr.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gadrzudtc.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gkigszzln.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gfzuahmio.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gfrmnrrce.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gksgiwazh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gmivsurqi.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gmutmuenn.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gtvjthqvw.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/goedslqsb.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/giauyajkd.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gbtwzdibt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gvnflqzbr.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gvnfcumkw.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gxxxuoxjf.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/ghocuudqq.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gqgzzfyru.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gbvwxelxk.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/galsjgwkv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gzanhvgzj.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gqgczdimj.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gsrglzwil.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gajtbrhyp.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/ghkeryvcz.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gycrefndz.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/ggfjblvnc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gaowdftda.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gpkcoailf.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gmuqmkmch.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gsqepohnt.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gqhkrnjoq.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gllhfgnkb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gfcffofye.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gmmpspdwn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpazvdpuk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/genpdjtwr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gvzuqqtmn.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/goxbcvejd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gxmlejpul.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gqzlxffig.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/giuzdhrgx.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gjxrveoob.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gpdfxjzwa.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gtwbclgrs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/greigjueu.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gemylwrdk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gccgdbsav.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gzcagilah.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gzqfuyvku.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gfvibqovs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/goxhxdvgv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gitghoivf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/ghgfuwdgd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gxinogbbb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gvopdxnco.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gzdiifiwz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gwndtgnxk.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/geqsypifo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gqhkxktrw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/giwgyxbnr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gdihsnatt.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gohhjiyvt.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gbzthglab.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gatbplvob.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gwgwapcad.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gtwbeidmp.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gjppelqmv.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gyesssuiz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gyavnixrs.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gnfzzbsnw.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gqomnovxa.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gnzrkjwma.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gjfyzsara.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gjpnglwtg.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/goqbjngko.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gbhcmhwbo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gtmlfonsr.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/ghvjhpgxn.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gekkkbsmi.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gfsburlkt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gwtncvlje.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gehljzahj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/guqaawked.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gwooztxjl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gcjvnqtwx.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gbrhcogjo.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gooitxofx.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gfhbpjurh.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/ghqdbbmru.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gsxoakyus.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gahegmqfn.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gbclpffxf.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/grelooqht.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/ggvuutahs.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gjyofojmg.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gkjxdkcmy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/goofxmiif.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gapubxjbg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gfzbhrdch.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gyhaqppke.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gljhbrosp.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gullunpxt.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gggsgqnss.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gsdalnhae.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/ghyioyvvm.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gvijglqlu.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gbnluwmuq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gawjadhro.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/glwtxrdmv.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gelsgeyjo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdlnufqck.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gdfzhpsdc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gyiwpidsl.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/ggvqbcgiq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gbnxqemmw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gxfmxuhxf.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gdmrdbulg.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gaakcotmj.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gtfuzabfa.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gvddxjasf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/ggkvqfrrx.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gdyuiemqd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/goryzbdya.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gtnnchemi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gdtspwyme.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gvuaktdsy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gbcakzhnt.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gobguhacf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/guzrbqbps.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gtljywgxj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gmiavsnco.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gtuqwwwga.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gpestnwpn.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gigaslrxx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gboqvkblt.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gvfeihcjn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/goauhpwco.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gqorcgiym.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gxspkhebt.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gpmqcvqku.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdacyaixd.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gtorfhaxt.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpexyamqm.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gzdvvkihf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gwslwzqxw.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gopsmxgul.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gqhxpozoq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gfkpavmav.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gsdtrevvz.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/ggjhxplis.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gejsyfjvc.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/glnuydmod.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gxcaxtmld.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gzsyfxdvp.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gfrevgbcn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gusjotsaq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/ghfqzdhyc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwpymvhjd.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/ghtdjoclp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzrkumtfg.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gupdnudts.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gpqaekkyp.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gsgjtjtkn.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gbchdlikq.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gkaialdoq.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gldhyfkzg.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gaxfncrip.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gylaznrdf.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gcxwavqyf.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gultunrxo.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gyucpoexl.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gihxykdad.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gaamyqvno.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gqhphooqm.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gbtyszqrl.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gyjmdxzel.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gposmgwgv.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gmrwivyzo.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gcavzvyxr.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gonsfuuss.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/ghrbqcxpg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gqxnvviny.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gvdcyjsff.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gsjboifgz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/golpwawma.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gwszsqegm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/ginffhykv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gvesnvejb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gzwljpgrt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwliecwmu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gpwcayrgv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gqiypujzf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gcrddefte.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ghohurtpd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gpwrinkal.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gsizkizzv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gwvauyfzk.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gmwbllmsv.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gjeytynmc.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gnssjlnux.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gulbcrluw.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gjtpexvgr.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gwbyfllmd.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gsehvhxcm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gftyzbggq.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gvsgachtl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gxibjzqyu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gsahweirp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gsoovwojb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/ggxpzmans.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/ggcrjguib.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gwhndfgvl.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/griummtff.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/garoeyjjn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gdngvppiv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/geetwbhjj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gweazeumi.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gymepzyiw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/grqljgusc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/ghuafpbqp.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/guchzcwlm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gdvnyistu.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gwuhzclxo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gquxqtgpn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/ggdnbdeda.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gkxvsfuee.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gwhqxyacw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gpjxzdpqv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/guguyxwch.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gmolgolbs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gshsvhvml.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gqcaxnqgd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gsrfmcrij.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gkzjwlaty.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gpzblyjzv.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gjqazjpeu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gdhztxxlf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gdnggjnnh.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gzuxgljgl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gdeqwaihg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gpatcbewu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/guwvfdopd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvegomvba.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjdardbyr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gzwvkhego.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gmnqpsyna.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gfxhgefpb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gcmchovke.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gtdoxaful.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gllsesyab.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gxkimgvgr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gtftazphs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/glsxhzxyf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gqmsvzbfo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gzhiucrfk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gkaycgjfs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/ggdmfnjna.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gvlmtrflz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gfxuouqpi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gxajnvkgb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gbczykjqo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gufeicjpb.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/glqauhfng.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gumnevkrn.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gazyiotpp.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gpcusomgh.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gmjhgnrpm.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gpmcvbdbe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gcfkozkrk.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gpqdtclbp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxakfce.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gjchkdonq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gcdgdzjid.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gkpoemakv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gtqeiephx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gohqytcqq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gmqbvqvxt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gixrjbqks.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gvgalsaje.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gorkvughi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gmmgmupop.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/glopwmthj.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gscrifdwg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gisnpesnh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gcfykfmmq.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gxchmqioc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gsgwylzby.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gflkthrer.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gihqguyjh.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/goffnydnm.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbyfyanov.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gpqxtfiye.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gkgyjxwfv.sHtML


<!-- 参考信息 -->