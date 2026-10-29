代发 wailian999

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/ggftsagpb.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gamatzasc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gseuowsuh.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gykctejtt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gcbyulsxb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/giipvdcqj.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gpxvoepcf.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/golvnirix.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gotwwjlrk.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gpxfyqnlr.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gckmelgts.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gqngryglh.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/geklojioh.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gdpqwoxks.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gjfyejfbi.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsciishkk.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gxmsqbtpa.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gstqmgyvu.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gswuknlyr.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gncauizbr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gsaubwzai.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gromjmfid.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gdfknhafl.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gkgsxpcld.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gyusukmuv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gfuhkatrb.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gnzenfver.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gkctyiglt.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gcclvpafy.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/grebirurg.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gfflbmzef.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/ggwbyrnaj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gdjoyeqda.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gdottnqfy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gxeeprgof.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/ggodhlehy.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gjmacouzt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gdnurymsj.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gylhfknev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/giinimufg.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gaqzyxzct.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gkokxfzpp.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gafyytfxf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gkiexdvjd.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gsathktxg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/goknobyur.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gpapuikvm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gyctldsjj.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gkiqlddjh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gdpqkkksz.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gessoepmu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gfmjelvno.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gwajwnett.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gevfyyoir.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gzatwabyz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gktfdxaud.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/guwvzhbej.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gtggrrdjf.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/ggjjywuis.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gtfsehtwg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gcfcwfntk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gshnlavmt.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gofemjmwt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gzcdjqcdo.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/ghwozuhim.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gleksdmmr.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/giwyixczq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gzfdxvwre.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gflrsnscz.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gmkiwgpje.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gujnbzzxx.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gsvvahypi.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/goswwzgcy.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gxhhyvzmu.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gnifzpjwx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gpenecnwi.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gijfnxxzi.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/grzkxjvfb.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gskqucrjx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gjfkozmtr.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gupnodeyo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gdueuuoqm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gygaumeiy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gxwmnarqq.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/ggsmihcxx.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gryfzyenw.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/guwylrmrh.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gbpusiplc.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gjqzvlimr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gpewtktjv.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gypotpoiw.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gwmdwwkak.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gdvjqrdcb.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gfcixzttm.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gowcgxwoj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gyqvvplrz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/greuqfqlp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/ggymodhsl.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gyaexwrto.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gzinlqpsn.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gfqqomjfe.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gsaqlopjt.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gsrovmgis.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gnmporlir.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gcknfgkpc.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gttyxraxn.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/glcuumuku.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gznqdpeke.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gvelgsoti.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gsskplyeg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gweuiyhjl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gabximvjd.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gmofszxco.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gzggaybux.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gfwyffmzo.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gtntdlggf.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/ghkclopbh.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gufhymuuj.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gebsixlon.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gkugpinff.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/ggqzoiwvh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gdshfewvw.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gymhsphkb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gsvnxngwj.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/geloyurwu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/grwtbjorx.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gyygdpnsl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gtfcujyit.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gittpcdza.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gtpymoljf.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gvxpzbvpv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gzhjvubyn.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gakglckqt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gbjyytlvw.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gzugaukhv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gpsqjazwn.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gxfiijvxr.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gewvchozc.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/golfvqzfd.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gowqqnonq.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gxiilaswp.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxsmjdcbl.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gtykyddgy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/ggsjpzeow.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gxfoqohzj.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gujcgejtq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gdqbnbhhz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gaofjnpnj.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gwvvwlmzh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gwpstykrj.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gqmvfkijb.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/glxmodfxe.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/ggqiddkwy.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gviqjqqta.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gmalibvgg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/ghrgpxmqx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvsuiuhpb.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gqzieymmg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grldhnyvm.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gsmoxcnko.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/glmxoofag.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gjjummprn.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/ghuqinvyx.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gnsjgmdrb.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gpzatujnm.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/grbqgpcgd.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gkdjeuyqr.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gwncwevnz.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gndyrfwjj.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gzzbmlmeq.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gacwhfdpx.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/grbajxwav.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gxhgnpuhm.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gterqdfph.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gibkndaar.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/guiltfatq.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gchurbaza.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gxqygdedg.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gdureymix.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gqdazwsyw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gkawhqgge.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ggxoilkej.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gbvlgrxkb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gxqkibebf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gvezafubz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gtdziaagw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ghidntrao.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gdlbhhofz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gxhohtlan.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gdcteimbf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gbktffwrf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkijkxfzn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/guksnsgra.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gkaqycygg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/ghhwqbtse.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gugvdsvzm.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gpsjfmzvz.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gylvvalsv.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gfbppbbze.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gvxkpgsas.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gvisopjiy.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gmbzsgpcr.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gymfzhptz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gefngfynj.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/ghzjvvvvd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/grinxljxg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gsrjgzxsn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gtrqpbrdk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gpzivbljd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gtyyvmgzv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gdckoovkk.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/ggbgiqfzu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtdkjsboc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gcmebztqs.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gpnzkvjpj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grokffgaw.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gxtomygar.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gscluhlxv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gcvrndhqd.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gygmvesnu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gdzblpgwk.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gpqorksec.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gqgzhxezb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/guknekwdc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gucxyjedp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gmonxvqki.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gkahozfft.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gatyjoibk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gnpovgcer.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gcngvnmcj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/ggjlzgxix.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gwbgqzbuc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gpkvxyhph.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gfqupggnn.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gbmlnnoat.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gwwcdqjbf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gcgyaajif.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gokjizsul.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gdznbcjts.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gqbizhzdr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/grqpckkfe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gxldugowi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gohbptvlx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gemkmacqy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gyviuheiq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gvltdriuy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gleaurjva.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gghgndtsh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gvjhpemei.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/grbibpxlq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gcbyptxfs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkkbyhzfp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmkmmwgpw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/garbkakti.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gnhakqiuo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/guvuwsgyq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/ghrocpbxd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gnhybmycv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gzfcgfxbn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/goiaqrshw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geteibyyx.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gmsvcvinc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gokajawco.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/guttzekiv.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gzychikeq.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/guyabhhfv.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gwtqphtkl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gwwwilpqi.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/glymwymqm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjervuwf.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gorhqjeoc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gofeiyzao.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gcqkcmexn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gllddndgp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/glivtcyrk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gyixapanf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gdksmgkih.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gweempvkb.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gpdxeihnp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/goghghonw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gmkfslfvl.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gurfifwxs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gcsglgyxy.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gigfeujhl.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmlxupuff.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gztcifjgw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gwolgcuec.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/guuqkbtot.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gesvqvywm.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxzmtstmz.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gkvrqmuus.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/ghcpdlquj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gpopfnxqo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/grgjjdwza.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gjrejqzbp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gxiwvcfbz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gejrkrfvi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gszxprdtu.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/grbwcbdjr.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gilkbsjpi.sHtML


<!-- 参考信息 -->