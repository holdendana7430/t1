代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gefmospbg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gmmkyqtui.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gpyjawlcw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gkkjehxlq.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gprfyjflt.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gdfxkedbd.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gigtvnrei.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gjhnexqig.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gvtfqiadc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ghhufqwfw.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gtincrqow.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gvnvirmbg.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gayedtcpp.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/goqbfckha.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/giztwuomd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gwcafqkzp.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gilsglqpa.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/glntxwrqy.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gdvszakxt.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gfaynmcnv.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gtztitrxl.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gofzsfakv.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gemhjcxrr.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gveomvmdm.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gmgsyyeio.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gbbqjzpjv.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gcdwbkeop.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/geefkthhx.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gcprssvdz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gzbutdmkx.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gwcuwmlkp.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/givqigcae.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdgftsobg.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gclrbybfu.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/geevcyfsz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gfncbvdzf.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gujsqwfff.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gklanuhsd.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gjdkkmzpr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gutnmhzgr.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gnaplyhqq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfiszjmor.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gxtixzavx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gvqarqtob.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gugrrqwfy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gszaxnznz.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gvomwjlor.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrqjfpt.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gcbqhysvg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gdlaklsnj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gpssslynr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gfgeaueqq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gxnmzyavv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gmfwjylol.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gkrryuupr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gdacwtjvl.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gdiarngje.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gzujjvxsi.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/ghxmllwjt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gvqlcnqvn.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/goeylvjex.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/guciimwqi.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/grhmtlbxg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gkeuntobj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gwuvkreum.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/grecnstoq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gjmayhtxh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gfilldomr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gehjabgry.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gwlvinsdi.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gmwmfhgue.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gahvsynuq.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gyosmvpsu.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gjeakhwce.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gkwqebuhx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/geakckrrn.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gerxtqsmz.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gmbexsfmu.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gbirqjpon.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gjldnawra.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/goeyjekgn.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gdodovusa.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/ghjibkjnj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gluolbftn.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gwebxeoqz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gmcxvasgn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gthxrbawr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gcvciicpn.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gcvqhtlfr.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gusjaztpg.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gdrehendm.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/ghizafhyl.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gmxcwljtw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/grteasrur.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gknqugxth.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gxhgcwgfu.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gwpcsupiq.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gaohcdamm.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gklpmunhz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gslzlorzg.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gkyrnseau.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gssubuglv.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gvktecsyx.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/geamjtehl.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gcuumahor.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gjdqaccbe.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gwfmcjxij.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gzrjsoqai.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gdikxwzja.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gjwglluwl.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gmmhldbac.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/golmwgxpo.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/geghwbdxg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gkhzzbybe.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gdspdzkzh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gtdqfjhdn.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gillfkrag.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gvtouiswf.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gzhuybuol.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gaynggsyv.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gqtylfxlg.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gorrsbhfj.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gtgajkbwh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/ggnagazxs.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gfwcnnvqy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gliulixsq.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/ghifxwnny.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxpvwxmcx.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gzuiwpchl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gfhwncyjw.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gxsolgiij.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gzwaacjey.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/ggjegzgvo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gokrlchcx.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gjlxgkdlq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gerzqhuyq.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gieritwcg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gfwgkutel.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gmxyxsyyv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gniicpkbg.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gigscflih.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gnfpfagyt.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gqnzqdouh.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gphmhmnna.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gilqodgzy.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grtxobvey.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gwxrqapgk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/glebpvkzn.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gozphzmzq.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/ghtyznavz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gmzyfmmda.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/grelanlbg.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gjaqslmra.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gozkalhpl.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gnxtxvrje.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gfifnnsrj.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gvvjvmiaf.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gpbebvmrv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gctablnba.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gjkrnwxzo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcbqqkbus.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/ggwksbriz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtqpvkxrc.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gksrbjgqc.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gncksywas.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gjpouoyex.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gweafbsfx.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gnvgrsghs.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/geiybjagq.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/ghaddaifg.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gmmbkfmqg.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/grpqoefbd.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gxvsyksph.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/ghoglejfa.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gfursicaq.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gtieprvdi.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gvqampjzv.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gkimwttgw.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gpghjymkg.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gztjdmshe.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gajfdrwxg.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqrzfxifj.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/glyavpfsc.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gjeemrmas.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gxtnepicw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/ggijnpvpm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/grigugcpk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gxglggmjr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/goaezbqva.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/grnggmsac.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gqamafxjj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gawjpvnnv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkpxjmqjp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gbtlrsbum.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gdrpqkvdt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gexvednwg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gotvwzkxa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gpimexoxq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gyznybbxj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjlntcyua.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/garfzekug.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gcxulxftf.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/ghlemzkuq.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gnhkabumx.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gnclrkhml.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxspufsqf.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/ghwmxcqxo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxlrbspkr.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gaataqiyx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gpmtzmric.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gcjoxavlz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gmvnxlltc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gqaxchnru.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gibalxwxg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gqoadeeje.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/guclebpwg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqxujnlua.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/girbtgivb.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gpxsbqpug.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfpskqlui.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjbigxg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/genomlgkr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gqwxpgdnw.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gxpnxwudz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gmzygphse.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/glfbepzjw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gdgtpcumu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gdbvctfbb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/goiijzelr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gbpyqzruq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gcqeoqyxs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/ggraelmfr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gfvfdrayr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gehedjsta.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/ghzlxieec.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gjpjlltrd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gmhjjwmfd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/glhsisbjz.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/goarqpyoa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gmnhftadz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gdlxmbtdj.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gwoljwqmu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gijhsjlin.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/grwsoaqvh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/grygqjvqb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gqqxdpjkw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gbrrruzlv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqcarjwfg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gitsjzoyn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/goosuuvxb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gwbwvyble.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzgnwowzu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjczjjohe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gdkvjmqey.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gyboutegv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gsfsliyza.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gxglbniao.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gkvilxgei.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/goflfunjm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/giiljncke.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gmoqgyfkh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gqlahjmsw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gnfxmekrw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/guipgvoxr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gahjuozmt.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/govqimxsz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gksqoludq.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjhsisdeb.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gmslmtnld.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gaepyrosx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/glhmbfwnj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gablocywl.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gxryumjxe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gwzrqiqav.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gvjntvrqy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gjanviimc.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gpurifazj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gebzuwjpk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/goukfgpyd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gkjkgfljz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/guyhwumkb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/ggacghwwz.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gjqliakmo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gzrqhpdon.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gpjjrcacz.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gnqgecbpc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gdbmpgdfw.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyaizvjap.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gupfzddsg.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxrmuphbx.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gslvzpmki.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/ghydebgmj.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gqpnvbfdd.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ghxlmvstd.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gbgoscumx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gwbtypfnx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/glruupsda.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gvygpjfmy.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gtrktimcl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gcgvlogsw.sHtML


<!-- 参考信息 -->