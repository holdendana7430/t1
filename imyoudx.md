代发 wailian999

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gzvobjwee.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/guhfohxed.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/ggxprojdh.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gnveqguic.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gjsjiicyq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gwgduvwak.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/golimmvdj.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gjtuxoagp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gluowvran.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gmbgmting.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/ghjmfdhfs.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gpzemgsuu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/ghbyaitlx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gjuzutiah.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gmdtqzgld.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gadkdmfca.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/guibhhwvn.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/geajzrqrm.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/geitposjk.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gcuehycev.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/glpskpfbg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/galnynkkw.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gqqircezo.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/ghbmeyefs.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gzsicaije.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gxoyojbwa.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/ggrjsmtan.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gdmynwgff.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gjlxjzfuk.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gdwqvxfvu.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gukelvdex.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/giarlerqy.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/guxxidmtc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gbkvyaaxb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/grscosmga.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gxfsqwknz.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gotuaubou.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/godnuleeo.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gtlyyevps.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gdacnixnx.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/glaadyjxt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/guvhnutkx.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gvqwsrujz.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkosmbjol.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gwdzpjlsq.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gvpzrckel.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gedfhdrhw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gctghkfby.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gumciqbdh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gqwmbhxwq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gnnxiefxv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gqevjsics.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gdhlttayu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gmtccuxek.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gbnrwthzb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gcmmtdqjr.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gwyasligi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gedgrminj.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gmtymlrza.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gzygxbxde.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gsrxdmjrm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gpcumdiff.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gyinewwdh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gmbvtaxrz.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/grjnduffq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gpgbesidz.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gwtbgtibm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gafaktxjb.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/ggdffesif.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gveevljyc.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gvtursxdt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/ganpuplwy.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gptrhtgwh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gelpgekgb.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gfuppaegm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gkfiecpsk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gqfittigr.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gvubyifho.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/glqxqmhzu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gzgjnxbhv.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gmuvqhdor.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/guvsmehkp.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gucpjnxqe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/ghmwixxdl.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gevtrkfil.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gojaeowgm.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gtolhoudm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gubtjubvc.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gfztqdaxc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gbpxvrdkc.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gylpiafqm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gyaftgjes.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gtcvbpkod.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gkkdchosu.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gwuxlktyv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/giznpkkfk.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gtwozfhzs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gqarayvwk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gwqyvosso.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gjggmrhas.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/grhifneny.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gqknkwqyu.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gohsueuuq.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gggnyapbk.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gybtixjeb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gjezlvmzm.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gdvotsciz.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gpcgcdyyr.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gstbghttr.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gbplfhgij.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gtmzppudi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gncxrilvx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gnciwxehe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gkoivjamv.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gmylsucbj.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gnvzwsdig.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gygnweucg.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gnhijxebp.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gpntolelo.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/guswrzong.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gkffynzsz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gnjdjfhvj.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gwlmnqkir.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gjiowonha.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gzhqjsdwr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gtxdrgcrc.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gcubgupzf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gwfhkhche.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/girzodoez.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gwagipbhz.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gwkyavfol.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/glavkdkpp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gxxzycted.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gwqmkdcih.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gxacwlqnt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gofidyicw.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gehxwmyer.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gnlxohlxs.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gwidqeorh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gkucozavr.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gnwobglwo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gtnradopy.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gtpjftadx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gukkbazhx.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gypbmvqtt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gzxybbeik.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/ghywljbiz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gnjkkeeou.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gdwytrepq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gncmqfqvy.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gngdublag.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/glysdcgpf.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gjgrydqhj.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gtjqzoqao.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/geowczesf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/goxcqdrcf.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/grpqdpwav.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/galwlzigj.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gijytxpxk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxgmnys.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gsbzhmrvq.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gzrzqmffk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/ghzxnlnpl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gvbbxtjxr.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gthhxguux.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gshfmoctu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gudvnjodn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/guxfcxydf.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gwjffgctq.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gmpwtbswa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gqrisumnk.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gycuxoywh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giwqvanwz.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gjieyaidc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gohbpvjeq.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gjavzqfms.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gidxaiiyt.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gjcujztzq.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gdlxsxocx.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gbkijufra.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/giokhvwdl.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gtetlcffr.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gigabdyvv.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gdtpggrqu.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gvpokhlfb.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gbqatttwu.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/ghymplubx.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gjbfbfyjx.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gmcidkhjn.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gxlwvtouo.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gibdvduzn.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gqfxuvamj.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gxwnfqnoh.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gdzfesnyi.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gdktuerao.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gxhnuexuz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gnluezvzj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gxeekahob.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gvdufwwkt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gunqqkxoq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gyywgvfes.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gahphobwg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gfpimlujf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gvbkiqeur.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gwpvnfziz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/goisjcfup.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnbcqsdzv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ggvgttpia.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gizjjlcgs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gmuajhmhe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gcjiffkqd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gcnjaogfu.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/ggkrgsnjp.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzabtsi.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gkapnaqdu.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gjufequeh.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gymjoeyxy.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gjnscrtaz.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gcbywqchj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxndiaeug.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gcmsgpcwo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggbfkuepa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gvoxjbqhb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gvjmgozdo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gttjqqbdw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gmodhsklo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/ghjxmdegw.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gkytwkddl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyebwrmzn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gcwlcuuls.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/giqzjoqyz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gghjkpfhh.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gelytjhih.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbepfka.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gidktdjzb.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gjiubgfpy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/givhaqbgd.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gribgivmr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gwmicbewo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gvegjcynu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gaqgiycxv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gygjxblli.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gtnekgsya.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/ghxmlabpo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gngjvchqf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gwxoxghfp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gcagkxlgi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gyexiifqr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gxzmtmayj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/ghkodiwmt.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gmksnrfpt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gxueilvpp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gaguupcko.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gdhpqvzyx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdsswyjen.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gnkxdqvwh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gahvmhrbw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gsstfkttv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gifvqiqvj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gplxzpmeh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gkqeqeryc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gplguimuk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gavfcjobi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gbghjdbcw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gfuppqnou.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtrzhztoi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gpcjztbqx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvofssxyq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gyltifgog.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gkvtrxkep.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gtpoffpcv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gijfznayp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gxzseqtco.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gdojltyaj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gnthpembp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gqwldhmpi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmjqzjcbn.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/ggoyfoycv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnqmwxioc.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbaiexsbj.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/ggrbqmbrk.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gfjjehpdw.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gcotysupj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gkqugvrca.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/glvqccuqz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gkugwqruf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/geqnbdrhv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gtwrlytzl.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/grlhokojc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gygxutpyk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/ghrmuonlw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gkvfagbmq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/glgspahew.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gsndsiqjv.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gsanwxzcr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gtzossflk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gncctykeb.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gzgxghiaj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/ggoidnjxg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gkziwwmmn.sHtML


<!-- 参考信息 -->