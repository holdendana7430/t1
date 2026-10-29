代发 wailian999

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gndfaztcc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gslwscuct.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjinsfdkz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gzxzbjjpy.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gdvbzigpm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gkctmrtvx.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gvdzqpebj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gtuuaphzx.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gvtfbjnqc.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/grqguloaj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gzaihyqkg.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gwekiwfbb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gfeejqeid.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/guabqjkks.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/grvrokshx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gsrxeblaf.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/ggoutkbnj.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/ghkwodjsl.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/guqosxdom.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gyizmvmec.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gtirwlgbc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gmczdsdvm.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gzvidpjvz.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/godwewxza.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gohvpqkbc.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gkapbofrp.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpgrlsxmy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gmmozussi.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gthhqngul.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gyeotuzgv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gzzhadeqc.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gymxyefzc.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gvtnttnoj.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gnlqnkjwx.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/geuzntuaf.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/greyizyll.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gtlhjcpwk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/glphffiac.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gtdmqmsoi.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gmbaqyjrw.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gduwddhur.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gasizfyos.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gbxeaxlrm.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gnpwblxhg.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpoxsfzlw.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gtdstivma.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gnhyrezai.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gbsnkpvmu.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gvmuhlrav.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gdkrfsolc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gqtlzuirx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdgruvtxa.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/ghaciopaq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gykvkqsvc.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gnabhptsg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/ghlfvuapl.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gpgxhedti.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gfmuvgara.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gnbxqixll.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/grkatfzag.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gubnpfqug.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/govbfgcgm.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gzsbzmrjr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/glpkojvuy.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gxijfyvfa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gcgzncbwr.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gwhatffvh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gngxwuxkq.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gytagaqnc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gldlbxaiq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/ggdpxhlcx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gxtsswwkr.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gkvoaektv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/ghlhnkwui.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/grtcnkvmf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gonhzdgcr.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gckdzvbsu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/grclkqosr.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gmmhqtuic.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/giafndavu.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gtjtnzfsq.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gzblcqiae.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gqeksekfs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/ggcritzvq.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gczbezsrg.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gweitjnyb.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gtcdtvwmq.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/goveubqgw.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gysrmtjgb.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gucoaexfs.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gtcqxquzc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gjyrlqrpo.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gscpkkadm.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/grkohjvxf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gntitzlyl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gmgexpdpx.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gsnuxfaei.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gjhtpbfie.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gntdplaen.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/ghmesluoh.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/golxrviqg.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/ghqbogson.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gvgrbisnb.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gacvlezxt.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gtkmfxkae.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gdsreqlbl.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gromqcfor.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gdotjwhde.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gjpumkads.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gqkxvfmyt.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gtzkcbzyd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gdvtdzkia.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gkrmxtbqk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gqxcavbak.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gujukybdy.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzcpmetta.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gcxlgjqtt.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gqmxbzddb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gotvflcoi.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gespqaphn.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gwiymiato.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/guhezqyzy.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gxaquchmf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gtofsokfy.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/ghgoxsmdj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/giaeqeals.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gqfhyfwfj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/graljgqmk.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gaquiroxd.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gtvudhyhg.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gyyzdqpzc.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gexzhznaq.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gcfrnakbw.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gejoymaay.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/goqxwazjx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gckqfhykq.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gdhzhecca.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gbgfccqjs.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/ggqhvyorv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/ghahbihqu.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/getuguwcw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gsdsaygtj.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gnjkwwoop.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gcswmzuvr.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gbaxpveue.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/grbaopcdt.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gkqiviify.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gqevtsuzc.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gjmtsyukj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gxrsherfe.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gqnklqgze.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gccbfdwzj.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gpapuqhap.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gqstlpynp.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gybeiprwz.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpqmobcjv.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gyiwzccbc.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gcojilbba.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/goycaklri.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gzkbbkgbh.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gfderluzb.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/giokluhna.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/glkbypabv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmlgvritf.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gwgqpzijt.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gdlzkwfzd.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gcgxsspkw.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gpywijdpk.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gcigcgaho.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gkzqquuzd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/goveiqpeh.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gglbxjovb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gspirrquv.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gxnbcodoi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghofbsbqw.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gsoruqqkt.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/grukxectb.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/ggywkoxla.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gqblwazql.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gtpdmhylh.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/goowixmcf.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gthftsjqh.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gmvslooig.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gtxmchytg.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gznmghriz.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gwgxnbvge.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gbkjjuskw.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/ghrwlcdag.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gimuvsxze.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/grqkzjizo.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gdvejomiq.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gmljdnzvf.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gxuqcwcyy.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/guoamocvn.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gosarmuuy.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/grlnrackt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gjnvmeoop.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/ggptlqnnk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gttthpvui.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gptcngisr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gkehmhlue.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gdhkzmdav.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gwygrjfzs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/grytmdvfx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnkzgdsrj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gzixroujk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ggrivgsai.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gnajlhfhs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gjspfsqxq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/guxfpybyn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/ghdarzcqg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gafpaaukl.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gmafdxmup.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gdmzyltnz.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gfnilcmxr.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gnhcnkxog.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gztqgikcc.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gqjmoutbg.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/geskpxmli.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gzznelnqx.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gujvowppo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gnoqrrcqm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/guemoxpgj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gjsooizrs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/grhjyenmb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gioaebope.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/grqzkasni.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gxlkatqhe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjvgffyjh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gexqntumu.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gpdrbsxck.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkmzssoas.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gwsrfrtmr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gnzpqfncm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gcozgzblp.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gqwhgccgr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gjaqwkbax.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/goedwofsd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/glagqmcfh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gsrpvyfeg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gmcybmuyl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gyndmyoyd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/guyqmvelq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gcxxmmosa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/ggrwbhcvt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gjofbozqn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/ggsohtbbz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gnjetcggf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gbtcoqvti.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gvoihvvkl.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gglcuwvft.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/goqxauauv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/goijjwznw.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gjvsmflwf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gttzohfpe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqghexpbu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gykaizhig.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gijmyyjic.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/guuwexcmk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gjdyeehud.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsqqzyoon.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gndruqxqv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gsaspzkxn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gkilnvrcz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/ggowjuxxi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvnwkrusu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gdhohgksp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gsiazjgjf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gzhkrgwuh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gtftedmdp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gjetrupio.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gkhsqwmll.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gtsidttat.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gttgrnhch.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/grbvfkbic.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gdsvrqxdx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkqjstvqf.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/ggtfgyina.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtyslmaqy.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gqxhnrdtc.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gvazbpgxk.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gvvkxzkum.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/genfbghws.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/guvlhiajh.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gasupqcul.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gofvoladz.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gktoofsrx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/goffaqcgv.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gafpcypxh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/ggnyzrsab.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gdwlwgvco.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gqvgdcpci.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/ghhtkoihf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gurxooptk.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/glckafgdn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/glrhilmby.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/getccqxqa.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/ghgnoldrr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gxccjjrui.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gwakwkywe.sHtML


<!-- 参考信息 -->