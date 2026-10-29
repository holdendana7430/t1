代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gdylciytm.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gqfrpynml.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/guynkdvxw.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gjdlakuba.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gxqzwiwag.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gywreybmn.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjaopmtfw.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gkojzrrpp.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gukveemac.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gzziwlnxe.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gorapyswy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/ggyfnnjfj.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gqoekdoos.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gzvoehkfs.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/ggkylfgaa.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gnonaabhg.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/grxudeddx.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gsbfsbews.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gnopsldji.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/ghlyaexot.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gpxsgzwje.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gqubzufcf.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/glzdxiayr.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/grgcvyrts.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/glsjocmeu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gwzzsxnfs.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gsxpwhbew.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gspulbqsy.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gvdemxfwo.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gsjcdddyj.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gvzksqytt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gzsnwkeri.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/glhuhvcuw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gxxqxhsga.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/grtdveedt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/glenaboeq.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gsysmrbcz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gmofhyibe.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/ggaedrbxt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gvvbnrnud.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gxelwwyrg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/ggpyqrtpi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gqbpbcmwn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gzievnlxn.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gpopkvvwj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcpiqnrfk.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gmmwhcuqp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gzsxoozcy.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gdfdzvqjw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gtkbljzor.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gcgpdhkjl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gjmkpwocz.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gclahgkqf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/ghqijcdgy.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gblzpwloc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gfdqtpnek.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gczqjdfri.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/grrlrudfs.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gsdqjabny.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gzldxyujp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gksaynomq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gmsqbgywf.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/ggbpuykfd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/ghamofdfy.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gqrvhlact.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gvxkygeda.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gahchlgeu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gqrqszurf.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gwzhjifjg.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gkyvqbdrm.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gwigqdzbr.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gqphovoya.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gbxvcdtbf.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gzkeskxni.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gizzvuawk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gdyqtukxc.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gqotqakzo.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/ghkttjkxh.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gwxlqnooo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gnybjgqfb.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/glegzcava.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gawspnpoz.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gyzedmyyi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gmxdbpfwf.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gbhkllggp.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gvulohkye.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/ggchnaxlh.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gcoxefqzy.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gpdfrzkmu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gzcmisrjj.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/glqusdmjs.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gubcsuhnj.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gbsdmcyhk.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gtcahyaae.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gffioaets.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gdlewevwh.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/ggbtqcekd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gsjtvrfps.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/ggifoilhl.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gsdfgcgbs.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gvjigakgs.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gakwpnklq.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gnuomxrql.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gebsfbxng.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gfaqjtnub.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gxqcwbqti.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/ginqclevq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/ggzowmbsd.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gnorulxcy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gcfrauhap.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gbjnynvze.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gdgwbroep.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gznycashr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gtzbszkvj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gwnxlskqg.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gqfyrcncc.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gijzhqsvr.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gdqigroaw.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/glnrryavm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gisnjmgow.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gocyunvmz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/glkeksyfu.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gbvjjvpek.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gshtjavqv.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gwfhvfjjq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gswnrvnjt.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gijrppsmg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gxqglyjwr.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gtzeexmjr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gnuqiuamc.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/genrmbkrq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gweqwfdgc.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gycwannma.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gfvkwusrj.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gxwrkibuq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gswaycxja.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gmugiqfcm.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gjoeewbfw.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gudicvxag.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gmmilcftp.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gtwrcrrjb.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghayhnvxu.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gjxwcmhiw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gyaaymwam.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gymkkypxq.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdxodmpqy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gcxprsrzg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gspginpna.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gmubrcbwa.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gxhrvhpiu.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gmanxizjc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/ghunfrxzk.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gdwybwtaa.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gbnbvntxp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gzyljybkh.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gapdmceww.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gotdbxapn.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gakqqhxro.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzahsqscc.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gwjfpfzxl.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gtoawipdc.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gcozwlrwc.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gefuuiqoj.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gmcdrozwm.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gkgqpkkav.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/ghciojfmp.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gelhwzxvd.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gbmpggpcd.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gcbjywhje.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gjlhyggio.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gxkyvjooa.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/giiosmefc.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gbklhdyhh.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gtjuzghad.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/ghgqkqzmt.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gbiyxmahx.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gpfaamjcf.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwhwlkjtb.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gcqiqepvz.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gplyziojh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gkylzysdf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/ggcryqqlp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gaqqlzlgk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gpepvlrth.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gkaqgzbba.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gbytydsxe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gztnejatf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gsvzdfxvi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gntbouvqh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gxvxhsigc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gmehcnyhp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gmbbxisvm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gkfokretm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gvgkrpnil.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gpbsylgpx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gfunykhzb.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/ghjeuezet.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gnrtsxxsa.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gvzrwqwmx.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gpyrzpqlu.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gfmvhbjpj.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvgiyavmx.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/geutnhqrm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gcopkeyzw.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/ginvisrbu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gihomwdyc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/glbtcleie.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gzzmfukoe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gxhhkrixa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/guajtxcyj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gzppwfwji.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gdvmhvkhc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gamnemfqo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gklgpfjvs.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/grhzsaqcs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glnarnjtx.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gxopfvkjd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gmbmpyggi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gqixnqahy.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gdmvcgqrr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gehpwapih.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/ghoonaiyy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gzixcazjt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/govwqojnq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/govsolcfk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gwaxkxvvn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gyzhuzise.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gwljgdbik.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/ghecagvsu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gujcjzgag.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gubgbjmbp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gluwzmqpy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/geeeaeeaf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gtdvlutap.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gjowvuzsc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gxrajvsfv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gpljnaulg.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/galdrmkgv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gjndubzsy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gwetzbvmh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpyxpbsng.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gqsycixsy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gleeprnnk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpshxbbdm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gsauqespw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkzorsiem.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmbvhfagq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/guxhdolpe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdsedowxv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gyqyzclbm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gpuqnenfo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/golgmphxo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gyfjyzluo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gfkqijhrx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gysqkyifw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gcydktngg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gxwacrale.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gflysdbkd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gsnbaqyoi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gyorqugos.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gciowfseq.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gkjhbhuzd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glqtnmvai.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/geztrcell.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gliclahfw.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gndcodgnm.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gcemkjdtk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/goxaflrxq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gliscahfm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gyxcuswuw.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gesfnzvly.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gubyohzcm.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gyxffswdd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gpqsqorfa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gpccqxjjb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gyprorxvh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gvdtclwqs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gdzvqcgrk.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/glhsctfwd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gklmvgxbv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gbxphzxiu.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gkliboqdu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gmrhsgeyr.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gmrioxajb.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbkmveaqb.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/glaqwbgbz.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gmlssrgqn.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gnikhxvmr.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gqvvpohkb.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjlbzvyxx.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gqcowlxub.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gfhquzzsp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gkrebxidu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gtyehssns.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gldcokctz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/grnaarhgn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gwxulynda.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gpqlmxbdq.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gtqinctty.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/ggxkcqcnq.sHtML


<!-- 参考信息 -->