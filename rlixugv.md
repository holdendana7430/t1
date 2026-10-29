代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gkxpfuwqe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gxfeightc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gfuxiejwp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gluxfzczg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gqetuhahu.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gimzcosvw.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/ggsadqghc.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gzqafzhxj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/ghxzbjyns.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ghnhndhbn.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gunvmdldg.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gswqxlata.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/givsjwksw.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/ggqxlploj.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/glcausoar.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gbcyejmfr.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gfhsszree.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gwnootezl.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gxhjucocz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkzaijgcu.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gnkqewgnw.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gcfcrnhny.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gwneicpag.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gednwvbzl.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gifqsjpkp.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gnbpjbckj.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gedvzgplm.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gxqupqdfd.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gnnizvpwi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gndvplnvx.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gxazbeifj.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gkqxssozv.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gsattntrr.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gjyzjhxbi.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/grrbgxfgl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/grcrrlkkc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/goedfoxjm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gbrtonpai.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/ggsezlili.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gsfrmorzi.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gqzqhxpuf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/glzxecyab.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gvcrcsaaq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gogvbfroc.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gdyyrkneo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/givqxhorp.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gqruwkzkv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gmbvzetcd.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gzgjtiqgo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gswgfiton.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/glegvkatv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gvgbhwzfl.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/guncsznpv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gslmxxbqc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gvgxwjwzt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gycingrcu.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gcqzaafax.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gkkiryzlp.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gzkiusjso.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gxemriljj.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gxayvkyeq.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gymxeobwo.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/ggylyssoz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gfgbbukom.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/grhuxykez.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gwergttvc.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gredmhtky.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/grtzdjjxs.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gluarsrru.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gzcjubnjv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gskgaihoi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gmnxftnna.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gfpefgtvn.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gtzywfqbj.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gmieonzzv.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gsnycwnxh.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gmxyxipsa.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gevhqctqx.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gxqskevcf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gbidbjdhg.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gihtnmher.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gkgoptdgy.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/ghpchwmcj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gljvvayxl.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gonfpwwmt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gelyjdoea.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gogogmflk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/goynvyckn.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gxkrrpgcs.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gfeqdqfkc.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gtxpjfify.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gdduuiezy.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gkgtgzgrf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gyozjxbgv.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/genvmjdqb.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gajfrjhrl.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/grcrfxedi.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gcrnkphhm.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gbvzmlnxl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ggvmxyjes.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gbaddkygc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gpkzvnvot.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/ggfroomnq.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gejhmwczn.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gpzvimosy.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/goqusjnrs.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gsnizedkp.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/guepztccw.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gqzgbkrix.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/ghnkmkqon.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gbptthxll.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gropfansv.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gdusymggk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gyvgxzszw.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/ghfoxmung.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gbtdlnlnv.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gseyiwckd.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gmhhaffvu.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gvqnwgbtp.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gcbehkqeg.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gdejnfvum.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/goybunmuy.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gmvgqotrz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gsbqtskar.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gkiughwab.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gjvkvcjaz.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gxftvgvap.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gzeadufkf.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gskkzaner.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/geduugybd.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gcttfkdgb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gztikchdh.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gbsnklqze.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gnrwimjye.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/glsevqudu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gwkhzymue.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gpybbpapi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gbbliadge.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gpkfapiqx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gacxktqfu.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gmetpbmus.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gztrwslxa.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gnawvaxbq.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gszqtbglg.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gcpveliyv.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpwebsjpp.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gntxffdvm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gemdgxhxt.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gudwkemrg.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gasxfvckd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/getoepheu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/goldtvfqc.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gjoseaqjj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gnfyyntob.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gviqxkcyx.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gjaktfcrp.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gtxjsgqtb.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gzbuocrja.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gpudrtyyf.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gwgdcpikb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghheivrbw.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/grlspwezz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gndhtthhn.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gkfgrjaam.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gyizokwxj.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/geonsgmpz.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/grvqxegxn.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/goysmkuld.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/ginrrirti.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gyefmvvqv.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gaivxcvyb.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/ggjivbavb.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gdmleofkf.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gmwekwoyk.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/grdlddbkk.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gvahkwuxe.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gnrcuaswp.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gqxpuubbc.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gnblzelyd.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gkxvcuqxs.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/ggocwqjit.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gowhmfxxd.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/glvklbhzt.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gljktojrz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gbpjftibr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gajfqoild.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gbilswxkt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gisfroozl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gucowktjq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gvhaofazu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gtutonuvm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/ggmwmugkq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gurpolttq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gaszpmafc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gbylfprzr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gmduzowpn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gygyinkso.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/guwlzjfvr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gvtychmgi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfuwlkzwg.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/grjxirfij.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gzlbsegji.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gvgihnnjc.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gedtupmbp.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gvnpyqqxx.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/geszsnxcu.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gbbwxzphy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gqjrmfhnk.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gtsnffulj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gunrmpwvb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gntjpyrhs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/glydwrsmb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gzjpjlfel.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gfazybmdj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gegympwwc.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gccqneine.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gddnwrorq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gweegqqhd.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/geplywkdh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxizxboqt.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gljsfwdth.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gsjokhnvc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gkkfhbfec.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gmbudyybq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gcetsemjx.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gvwkalxqy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gwjksvtvv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gyfgmdtuc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gyaccxnup.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gitqtxdfb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/galvsjvax.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gclbpqubv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gjrojclcd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/guornezvr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/graaulecs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gnmqsvyyd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gfufbipns.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gkwxfhhpg.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gnopslktv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gprubyxqi.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/grblvmpmq.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gxtguuitp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gxrxuevis.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gqrlmaolp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gajnnqpod.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gmztoahcv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gocokprjl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gjudpnwsg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gcaqsieni.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gpgwikypl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gwigpwqcd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gyhfshrai.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gazysowyv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gaejcaysr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gscdycfvs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gveqktxhj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/ghnroghqg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gxqbwqsbz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gwsohkfju.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gowxjytnx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gcyubeayx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gbfrhheod.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gmhkyzbzf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gugxqknwj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbvipnwwm.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gmrjpifll.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcpzwczbk.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gyxzhufow.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/glvxxmhvm.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gcorouxul.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gcutqxtcm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gwkbormll.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/glnufqmgo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/glbtzpvpo.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gusqrxhuz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gtsmchhug.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/ghomxjlrb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gfqalxmwo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gxupmpjag.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gcagnxqsb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/gkbhlfzca.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gubenxtee.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gzmcbekbo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gvrehtqnc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gcwtajjjk.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gimqwnqwk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gsuvnfdzv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghhlvxwjo.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gwluttuin.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbsbtrnbe.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzrmyeanw.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gdytnccxr.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gomuirbmy.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gadfjwuav.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gwvgwjsvu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gxekfpasc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gbnfptdyo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gnhhgajdm.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/goxmdznoh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/goepfgcms.sHtML


<!-- 参考信息 -->