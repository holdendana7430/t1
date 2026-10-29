代发 wailian999

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gpduawltj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gxrenwblk.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gwpqwtlxx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/ggdmgmlbw.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gsjgmztiv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gcekptrud.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gclfkcquw.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gmyipdxug.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gcunuwjdu.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/grfjzijvy.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gfyoeitno.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gezouefav.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gweelhjgj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/glkqvjqtk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/ghdowmprv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gjlrhxyke.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/ghwgiiwxb.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/groinubie.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gpbuawhds.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gkotujgrr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gpalhuekg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gsqshwplk.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gqoybgovt.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gsclbpprz.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gsbniahjp.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/greqfdvcc.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gejzfdeym.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gllaywfob.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/geripboxh.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gluxxzdhb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gwvlpreoy.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gafuaigyk.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gnhxeqplr.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/ggxznskpy.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gclhjxlvp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/glaimuljo.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/grpvsuqtm.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gqkdzqifo.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gsjrampog.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gdhegcaic.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gnlsswdsj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gxfcybgym.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gmceagcmg.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gwbfyjfus.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gckmglwzg.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gubfqhahv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gwamrcmiv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gkmcavvwb.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gimbufklb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gkngunumu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gtnrtolrb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/ghrhaiqhs.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gkozjwgoa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gugussfvj.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gwrucgiop.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/guseywotv.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gclnwraqp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gnbmwdzkk.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gzibseoiv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gcxtoiygy.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gcxawnqxb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzemrvdof.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gdfpugqiv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/ggkewcsnq.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gfeifuhfq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gfohjezxj.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/grxkphzjg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gcqglagca.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gdgkpnotj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gsodzhxwz.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gctuafmhd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gnfyltxbr.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gblisnwzo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gazzawged.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gjxqhwahe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/glqzzhapl.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gnumxmoro.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gefrgqhyy.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gpqfpqbgk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gjcweklhg.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gfznazufa.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gpglhlsef.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gemwaajaf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gmziodjau.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gmofqstuc.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gwcjarvpi.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gsiyryzba.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/grrhdkbsl.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/ggumbpwgr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gdqwqnrjy.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gewwjuksu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gbuzohavj.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/goybspxjv.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gzuwfgjkc.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gaggparwn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gyoefmrtq.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/giynfgnxu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/ggurwzmhs.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gkxejdpbu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gzjiyuxpp.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gkqizzkzt.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gewxligbv.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/glpmxgiaw.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gsulwekkc.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gbwdnjslq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gtxvrjgxq.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gshjntarf.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gyivfgihe.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gjbcyluza.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gyosiolnb.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/geqxczbbg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/grciaekbe.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/govedcjia.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gsgrayrgf.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gskxcvkwh.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gnhgvfvim.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gpxasjjct.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gnbbwfvjt.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gsajdqlxk.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gctzxoind.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gvpxynyng.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gxqfkounl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gxclrbalw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gvikpxcik.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gcunoojbn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/guifimvtx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gpaolveks.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gwprjzjkw.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gnklpxflk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/giwpflxcl.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/geodgcngu.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gmpvgtofz.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gizifmydy.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gawmauetc.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gedmdzduk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/graebceel.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gtgqhrjve.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gndqziaer.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/ghnuosvqr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/govugepjf.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/glertvasm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gmbfcjwkj.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gkuxpkqbp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gmpsosopj.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gqdbcqvck.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gzwhavxtu.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gugffccgj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gzasooitg.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/ggeamlutp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gtyvructn.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gqbtktlug.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gippsemkj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gmncjbsvz.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gbivkmlki.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gkkxzjsta.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpnniebfg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gzqmovsnr.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjzdcicva.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gsdirfbfa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gjimzpekh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gjklsrkhf.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/grvocfcfp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gxhvopqgu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gqncliqji.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/girwqiihi.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gveorpdrx.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gczuapjlt.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gseepzbnn.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/guepmwhdd.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gmytfahjj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gxkeeypdg.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gvolmuara.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmgmsmcmo.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/grkmpmvop.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzbhkqpdx.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gduncqkat.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gdkovzook.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gbztkamdq.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gmwdmxotc.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/glzsvgcch.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gmimqzsad.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gjynhjcdx.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/guymsfdlz.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gocshrume.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gyxkrsncr.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gnabvzide.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gmgsofsry.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gbwsgqiij.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gfxpssenv.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gnnuaqner.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gsonqurfr.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gkjkrjtvi.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gmunjtnxo.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gjlbzdxko.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gefzispor.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gvtlfurtl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gphcdkqlb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/grjwexodz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gwesseaft.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gqdcjdogz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gqhklptoe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gprbmctom.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gxdryhdvt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gjcekkpec.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmycckobe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gpaquemma.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gpeaobkxd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdjblkepz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/guzdegvxf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gcuvebqno.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gkiblktsj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gmqclaqyh.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gtphauzsf.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gxvpexhsj.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gpbxkxidy.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gisxiubwy.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gdghorypg.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gskmkoscl.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/ggwvkwefu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gxcvjpodb.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gsviwlxsm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gxvpfokin.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gnnrcqdrc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gaxphmkmn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gemsnochp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gtlqcldnf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gqhhbxxae.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/goyatasug.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnahgiswm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gtfstxzff.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/glxuvkoqr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzryzwiab.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/galemtaqc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/ghxkgyrwj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gqdwakdba.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gxvfzmxlz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/grwsgfpoa.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gcpfdgdww.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gqfjivypg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gueajxbyz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gsgpbdaap.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gkgyhxgew.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gvbdiacpn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/glypddurp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gzywzlhau.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gwxpxihep.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gfatajoll.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gjtpywjal.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gtjhjiuwf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gusaadiaf.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gzuejsito.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gdwcykhpj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwargsnvh.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gtaywfutp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gdbsnanae.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/grpzekfwz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ggmbaoive.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gmanswvvb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gegshhgsz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gmsvtvdix.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gfcotudhe.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/giyihaxnt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/grxicuirm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gazdhscni.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gyvtqxloq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxoiwpqup.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqnxiwtgi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ghfdemmwh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghwrhapqs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gxvlovpho.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ghqxqbpvk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gpsilufch.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/galqhjdpa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gyjcxcozh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gggkhwucy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gwbcnbfbe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghnselgnq.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gqqngeqrs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwmatsbdf.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gdxrpurwh.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gflbevtlg.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gxeiolbjj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gynkfuyci.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gduiusiog.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gkxmytims.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/goxasmubo.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/guiokbpqi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gwzhmeyeu.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gzrxvbxjx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/goeoghnyk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ghgwjcxfu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gkmjgthvo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/grfvpujxf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gvckpneey.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/grjxeddbp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gspxylhde.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/grbcqesen.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gtmzttpqr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gngiocvev.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gybhytfjk.sHtML


<!-- 参考信息 -->