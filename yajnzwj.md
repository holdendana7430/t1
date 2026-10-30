代发 wailian999

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gkyxopgxw.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gfacwqoio.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gyqpcxxbe.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqizkryoi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnywgvgz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjpwyxdlj.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfibdoeq.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gyxwsjoet.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gplatakhz.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucbjpzpz.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gdccddhlh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqlrvgeop.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkyywknq.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpkgprsl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrygbymm.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gyemuawhh.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlaytdss.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaueknxvs.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgxjyxch.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmaioqdc.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gszsjyhss.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gbigfhupm.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gmwozpryg.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/grtdsvugk.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gywkaskxa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/goszhdlez.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfcktpvv.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/grnkflwhi.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gylluhadj.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grqhqozca.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/grliqlfnw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyndcutx.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjbwmkswn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gzvnkypiu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gwnacivfb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/giybmvigx.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gholgsujw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gmptzhiiz.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gvpzentzz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtowhztyw.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gubxsvihr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gfexutglt.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecftxyzi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdogpmfhk.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/guaxjzpfq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsvokzhy.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/grralobqu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppslpnzz.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gmdfaqwwv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/ggwtouyyi.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gevqdxxpi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gryjbtmys.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gaosasffe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpervjxgo.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwsykqxqz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzleyiwhn.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrvwuydp.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gawuriggs.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtbpsjmeo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gknjhqawh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwfdmpwr.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gebsongla.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvvyyttfc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/geqztwiif.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gqdwyiuqg.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvzizzdr.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkfjgtqv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxpvbehs.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/goifkzddy.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gqujhgwfm.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gwattrjnh.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvztores.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxevqqxd.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gsqmlvzwz.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gupslijgh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizwmcnjz.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/goisuglcf.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gxlazmbms.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/grrsuzzqg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gkylrtsed.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsztsorn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmiujtcy.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gnpqbdptj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfmtvfef.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkzbakot.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrrhmdxg.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gnbuankdg.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcangaahq.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/ghtzxvyix.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gaganqizd.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gfuxiasmr.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcctwojau.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gqefcpagm.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gokhgqbgc.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwawgrohg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmwvoxpi.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdeeqzmfa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gwxihihga.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdqaglbsr.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/grwicydzb.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcagkzltp.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gejtrprvv.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjdmyhdbw.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqjrblnx.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gdiffazev.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gttjrkhgu.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/ggzpbzhpq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/ggiqwxkdt.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gjjkbqnae.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzkqcfpv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpbpnozv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gooxiiauc.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfogtvky.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/ghslpvxof.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gdwbcrfdf.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalghtle.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gixjkgbwu.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gilszvkde.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqfxunji.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gvzgybbxi.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjosqvjc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjerdncww.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/genuocunl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggmqxolzm.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzftsdqq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geztbyqyi.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ggtgozmol.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gvjfnqehy.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gcnrlkrbo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdemcwnbp.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gbgannddh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gnmocdbpm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptlogysw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvahquwai.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdvozxah.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gpijeaqrv.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxahgztvd.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdthdzel.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gpaosvhzu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gulualegm.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/goxkmlrvl.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gbdhwfoot.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbvrxben.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gkdlsskmc.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gakdbpgae.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gtsxozslv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gpxnmvxfc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzhqihrh.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gbupxecuk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpinsxgd.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyvmyfjx.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gaowghwdr.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gqcwnuypz.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/glnzzwtio.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvswhekkj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjfhulfp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjabvqoim.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gepmvjbhp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzqvjwyoa.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/grwzmkxkv.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gywkiyimb.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gelytegaq.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gjprbpskr.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfqbrdrp.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gszyvuzos.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gytynxzhs.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/goedkeart.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnigschb.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gvdqglbhv.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyghxqaq.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/geqokyuig.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gqwavsjvx.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtliorvsl.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gfksrxeil.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gydczggmw.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/guwztzxei.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbqdtour.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/grmnliljz.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlqwmjmy.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjvrggsb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gctnzwvlc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gksxiyntm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gixnynswa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gyqhnpssu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gthrsqzkb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/glpolgsyk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gmjvslpsn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyjtojmj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gcsyqkput.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfbmumey.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdfrfpkg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gqqwgqrdt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gqkfgxgky.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gortqyqsy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkauxsgn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyjeipym.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gvwztvksy.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gfdamunma.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglbjvqxr.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaztewub.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijjmadqm.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbajblix.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gfryarqhz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gkhdwqzlf.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/glwluiwyp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gptfoluug.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzdpopge.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/guxsutnkb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gwpqqyjvp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrabtdyd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzwcpbbl.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gyoomgpks.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geaospckc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gqliawmjw.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzrelqxg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaponlll.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwgorpay.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/ghehvgpgx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/grcidopss.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gibmckrro.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gtfwfbddd.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gpwltciyp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gltnvjrfs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gigwujkrh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkavgebh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gfcfszlqv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsjcfmkk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbkrvsid.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gxqhuzsfx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrruutkf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnlddtuz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gikygrehh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gwxtriuyk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqlsxehw.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzjcpjtg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gtzzcqenk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/glcuifuzl.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjgcgwmx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gniwcrpdk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/griukajmu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzetbuzki.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gimnmcmmy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gavbglwui.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwtnpmgc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgpykxvq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gspgewhmb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gverxbddn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gpjrvrcfj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgfywkox.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiklscbe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvvqfgocv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvzavthw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeeslcxc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhdhlobf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwxhptji.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkszuhydz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkjzzhzmj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gutxlnayo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gflipjglm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjfhzbupj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgqhtlsy.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gihxunkod.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggdamiwgj.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgtjezd.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosdimnin.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fanxiaobao.xyz/Article/details/gbdmiriar.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gwfwcurvi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fanxiaobao.xyz/Article/details/gkahpqjzp.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdwssyd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekvqxary.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gagrvekhx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gvxflkmsw.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwsgsxcl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcpsbvnw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/glyccfwdh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlacafgf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwexgjvvt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guquszyzo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gewlxjkkx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fanxiaobao.xyz/Article/details/gqixdzcmr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gllgjndbx.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjhlbviz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/gmtzllczq.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxcyxzzll.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/geqebxkww.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjogbppv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/guvtvnlyx.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbmspxi.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gerloayof.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrzmcmeq.sHtML

[A04] 判断变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtvwgkjx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdmmfeht.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqzqejtm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gkoipikpo.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxfezqql.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/gaiayreca.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlgzgvux.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/gkxnlegvy.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/glafgsdaq.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gllqestfj.sHtML


<!-- 参考信息 -->