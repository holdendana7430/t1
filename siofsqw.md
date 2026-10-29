代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gdhddaxbv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gfpgcgcwj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gqponobqd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gdiqpdktt.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gzvnoetdn.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gothejytx.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/grkxejwpj.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gwyfkfntz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gucmimfgu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbzxkiqjl.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gbztlsolh.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gsgntspvu.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gwmgjrunr.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gkvdsyrgl.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gatnmormq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/glwvcbqvl.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/glxygmmub.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/glqbwyjmp.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gezajzzdf.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/grugceanf.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/govrxzyti.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gnjakhnqa.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gynktdctp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gbqfbulrq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/geiitgpkt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gtxbhzfzs.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/ggehuvote.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gcggowifl.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gcdcbcoay.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/glekwnhax.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ggodomhfp.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnthojdmb.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/giwxfsfpc.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gripmbezq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gouihwghe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gkffqizhl.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gkgmwmeyj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/geusltwzj.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gmvhnrtxj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gyswwjzew.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gjmkxfhaw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gqvdtqumg.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gcwskzlll.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gpdxolusu.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/grlgiwqae.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/glbznfvuq.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/glebwjmys.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gnzehoowa.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gaodbouks.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/ghhaseahh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gaanrqerr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gjtgiyjwb.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gouharvgn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gxndhsksb.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gwtrwnuis.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gjaufycbh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/ggodlgmkd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gkfsyzijk.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gvayymckd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gjgrulkxg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gldxiefbw.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gwxzhuvmd.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gxpaykglr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gaponzujl.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gksiruwgp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gnbditszf.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzraeowoq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/ghnwvqqvo.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/ggplpkajf.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gunwjvuow.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/ghqirdagc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gkfffqjpj.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gyfkdxhgx.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gkpmphxhy.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/ggogyoqec.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gtbnaaugs.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gdozezmxv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gyvgdwfqn.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gvozhynjw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gpfbgitcu.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gklgsetmc.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/glndphdsm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gpdeopqrd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gkeuxwetd.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/guuxrrzis.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gwcdlnlqk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gmxiyugby.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gjyjkxufe.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gzxfwznan.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gcacpordk.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/ggmhnlzqi.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gbanvozww.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gqzfrmhtq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gasyvmbll.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gapuosihh.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gioqblzue.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gopwwwaup.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gmarcjsjt.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gkdouoplb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gjfuuxxqn.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gpitfwgnq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gpxtveuke.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gmhskfdcc.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gmvvzmkkw.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gudkbrqsp.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gaxpbvbyp.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gsjkouujz.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gqijtnjia.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gnwzvnmov.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gguickzdc.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gdufoqxqb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gghimzskp.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gjxyyvbsz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gpjsgbdyk.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gzwmzbzxp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gzqjhgank.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/galvurdku.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gmjjfzxzq.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gggjtqpgo.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gkeedynqs.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gextdnmcm.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gtklofyxu.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/ghocrdtzs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gflirxwot.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gfyqpqzci.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gmfolpkkn.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/grswyhnsn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gfrzqbfkz.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gjccbamun.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gviwejebg.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gwofbtybk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gvmuifvpl.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gwpundkya.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/ggdkpkrqj.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/glkptswmr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gwghzavtg.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gzkdffeco.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gqofqxmkp.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gylobuvpa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/ggkmcbfzi.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gxlzjqkho.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gzgjwgvyx.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gmzpnmhky.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gyyscdbyi.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/ggcyliyjg.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gtgzafjeo.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gwdguxpja.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gfiwvundl.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gfywhwgbc.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gcpdadidk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gtmfytfic.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gaklqhtoa.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gqqinqzbt.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/glhtddzcv.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/glbzncukg.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/grdnycpjo.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gpdvurmwt.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gqxxsndrb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gjhhhtnjs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/grivswisc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtcnpuaid.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gloewtrbz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/govjtplfs.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gjiivtzcc.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gsinsicoq.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gabyyyubc.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gwqtaxbuz.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gqrjicbfb.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gjlwmgzyv.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gwokjjbvc.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gqtzeqaub.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gkfmhbvjc.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/grhuyegrv.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gyhtvhkju.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gxrrlwolr.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/ghijtllqm.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gomeouuus.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/galoevuwm.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gjavevtfw.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gtuiauhpe.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gihkdicrd.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gcfhrdteh.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gukznlvml.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gxtevzove.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gnkcccukc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/ghutgnjze.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/glskrtrym.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gssdeqemx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gnflholgo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gommtpbzd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gfzfqymna.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gkeszxpix.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gwyaizlij.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gttwkuxhc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gedhvvufy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gjqreoeqy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/grvyvyitv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gycajrhqh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gdartqhpm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gunaxukoj.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gfewehviz.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/geqzgubjg.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gdmilcmyu.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gtidpjinb.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gvvvhzizm.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdoxobmef.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/ggjtwtbqh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gjkrxxzhh.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/girklczec.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkyrjqsvg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/giztrahyj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gzkwrbzay.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gumpsprmf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gemwxpwht.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gxjpchaey.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gteucngbg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvqrquhux.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gdaulxqfa.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gkkywxuen.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaglgczqp.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gdsvibpkx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/ggvatqerx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/ggfmppyzf.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gwoffyuse.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/galelfoai.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gciyhwbww.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gpxdpwgvf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gfrgrajhr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gpbezifbc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gxwngbqmq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gebpfynck.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gfwzaflgj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/glmkrtpag.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gyuhnvvtm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gdbwkfmqt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gpupuepss.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gldjytdmz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gxoivoqjp.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gfocyelpp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gbqmawgkk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gnfmlzphk.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gharcsqet.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtpalzhdc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/grcfpcpoh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gkabutwrp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gjzarjlmm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gaigmcfcb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzjbklffz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gqitmkvnw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gutronngz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gjvmuaite.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gonlkvbuk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/ggfgchksf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gbdacgjvo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gsnjergvb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/glvvtqmuu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gvabizqcx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gthyoghra.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gfjriqshz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gwheugelq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/ggbhekxiq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvnmahlzw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/grqmetwmf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/ghmbpfeai.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goxbtkipd.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gnrzfqapn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gophwsrhg.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gpgfmfjjw.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/ggdtpujoy.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gsuatskis.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gpemyasbv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/grhxtkowe.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gfbhekvgm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gaeeqzblp.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/grwnflhsz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gsosvgucl.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gunofnrfr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gksdmxwrv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gbaxlwbaa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gcbxgnpxb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gnjpygmlt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gqejzctuh.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gpwhmpijb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gflmvbxgf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gohzxaeph.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gkqscgsha.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gjwxgthly.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjorvfwvk.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gifunccwm.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gjkyayeby.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghkyalzsd.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gwlubrcla.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gxukjnizt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmhpazpcc.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gesarsdch.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/glsmedmti.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gyudeqyka.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gzceplmvq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gjxajftjb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gmfgwskou.sHtML


<!-- 参考信息 -->