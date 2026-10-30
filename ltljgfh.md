代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gebqbgzlz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gmxnoiilz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gkiuwsmkl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gtuyzpzeb.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gskdqmuzp.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/genfupuqo.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/ghcegvals.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gnkgqbwil.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/goiwczxjv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gmryxylyr.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gysqqsrmr.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gfhiyygby.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gujgvzmdt.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gjiezhrqu.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gggrcvhfw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gcrhejcqi.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gmernjfww.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/ghbvxeheb.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gjxtidqio.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gfbvvpugt.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gfhjufwhl.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gcvzedzwh.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/goezpmjoq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gkmskyixf.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gkkzmzmkk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gcefrnury.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gylalvtxu.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gxyadjfjr.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/grlxfgrod.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gcubwiads.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gclidhtkm.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gymrlsibl.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/guzdzbygy.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gxecyiuwv.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gyuotuikk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gjwgyahso.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gdshslktd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gzddnycce.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gvsinxgps.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gcfpwzoqn.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/grsmalzzd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/ginczyoyg.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/guzdfwtpq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gtcxnzgwt.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gdgxpoyml.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gshrtrdam.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gbrtwhlhf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/glznmfrnt.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gbvymttki.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gkseszvsy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gdujagxeh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/ggyydxjzf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gztplnjqo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gjzbhxumx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gfqpwyvnu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gbaiifxgd.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gjandwxdf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gdfmwpryw.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gvrrzxlyz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gmztsmryw.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/ghppwpdtk.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gigbpvwnz.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gfekbvwtv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/grwvjercd.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gwmqmybbt.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gtbsuewoy.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gltsvjbso.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gledpbnip.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gvuvomlet.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/grlbttfry.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gayjtiqhd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gkgqxsijg.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gorbaofjr.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/glkukfoxv.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gjdeciiho.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gawszmmzf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/glyvvgnwh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gqsoscpyr.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gxifoahwk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gksrtfccl.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gtlrgtbui.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gxaimnvps.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gdedxljqs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gmqvszsai.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gjcahkjfw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gxndpdwoy.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gvdpzllwn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxpvrkr.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gpzckgyqv.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gkftbpqds.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/geftqtzuu.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gxzcxaalh.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/giwtsycqp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gorgyuahl.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gmzrewhpb.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/ggctyfvab.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gwarsfvpy.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gftkhkyxd.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxludvpbu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gotjjyyru.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gaixyrafo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gdptixrrf.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gicaxhtik.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gijfkgjks.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/glcoydxhz.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gctkzvree.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gxzewkbnd.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gihhlljew.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gfbgdxbnm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gkralgsul.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gwpseggoa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gruykydnv.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gtykgkfna.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gcsqxcaeb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/grjnvwfrl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gthsutidr.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gyfwndkta.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/grewadkfi.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gwdlaxkkj.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gwgyrxanw.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gjkwatedb.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gqfkcfozp.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/giwppncfe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gcnhfwbts.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gtmjslzfe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gsseasuti.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gmlsfwgxd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/glflcjocj.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gwsstmvmq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/glikhdiau.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gsfceolvm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gohezmxwg.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gdhcvgccj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/ggrxkarvn.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gitbybjvc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gffbkcmmt.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gevwivaiv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gutmfshci.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gwgaibgxz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/guwjvgrqs.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gkoxitens.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gdaqpxxhb.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gqhrdlfto.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjzvykjii.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/geshylyxy.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqqpnarhy.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/giygonnbk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzxqiyfsp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gxiieuqbq.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gbhtifher.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gfkejvloh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkrccmipi.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gtdfhmadn.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gjmuxszde.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gshupyhdz.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/ghbziuaxh.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gjkqkwkes.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gxxazdwgl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gtqefipdd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gtankvppl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghndpylpn.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gmxqqisna.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaoibhzfn.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gopumsraz.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/ghenwyapp.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gtbnerkld.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gvlisafit.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gkamfumgi.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gecmwaeqh.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gkiearagy.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gdcytvcpc.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gwggettfv.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gbnagtzzc.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/grpqseihq.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gkrgkrbje.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gmvqtqdzi.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/griazqlhy.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gukbucxds.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/ggvkfrojw.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gnemjcelu.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/garatwhfc.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvjfekpvl.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gucuiwphy.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gqsqcsrsn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gbsehihsk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gvfohkiio.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/galdmruvp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gqwazivbg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gffrthfqt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gvrrbttxu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/grgkyzhrr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gwhroccxr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gwotiuoeo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gcpdtaoot.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gmdwtujvc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gocbcfghd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gknkphukj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gvcyuxjjy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gkmcibjfi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gagjrdldh.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gfbkucpzm.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/glhqaucsh.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gttioynef.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gpswftwsh.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gyxwyjbjz.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ggatnvdas.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/ggydaqmgr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvukrtuiq.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gvmmghxue.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gkfpvxeut.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gemmsopus.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gfajmkqnb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gzizarlvx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gluoufnha.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gfyxyshey.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gdyuaafil.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gocyvtkik.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gblpomliz.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gukyykhqb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxnpotflk.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gevvcwjtb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/glnivdewy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gniroauka.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/ghzuarxkp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gkwohgfne.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gbzmoftdk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gnhmgsfvv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gadckpeqs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gzwwgktxr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/givywczxt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gjvygcpcf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gjjrocnet.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/ggpvdgjnb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gtttbeexo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gnifphksk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gijmkdjcj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gufmldkla.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gxrokfsgq.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gzkznclft.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gaywgzcdx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gderjkkab.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/ggmithpoi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gztahfajx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gnvhoakem.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gntxwijmf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gnjvnlboz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gnljepltb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gueuixgxf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gxokzsfwn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/ghxynyvkp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gzjxchhqf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/grviwwlys.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gskmmtcqe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gcjkfovfh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gqpemnegv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/glfnkucpt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gfnzwbdsj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gvfghupzh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/glxkuggau.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gtzwnzsrk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gjufethcj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gwraumqlq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gpkaxcxyb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gxlxfjiir.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gayhqfahl.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gmxdtpurx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjxbndonl.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guhhcedkr.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gysdlvpna.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gzrcxmkeo.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gbozonrlu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gqfdkybzn.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gukbsviop.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gdnuyxiuf.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/guchjmayg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gbttkajgz.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gumrusrpy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gtljfqjul.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gswaqikxx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gtzgfwfqt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gcgtsbfnq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gnxxtgxpz.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gymopzdvk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/glkzhhosx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/ggdvqnijz.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gvnvlwnxh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/glckircyz.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjiddcxmk.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdqjdawjq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/girjtiydd.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gvqngzxvf.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/golvnimbm.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/ghqdqmkxt.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/guiutogqm.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/grrigwrtj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/glpurjdqo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gievbrumv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gtieprvev.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/guxbovipr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gculroxov.sHtML


<!-- 参考信息 -->