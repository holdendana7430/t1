代发 wailian999

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wmipubnb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3piudfusx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ixxulqhf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ajxvtkbr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pbqjplyt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3amstyaee.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nubfsxam.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zngyfxqr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xxrgmpnh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3kdtlshqk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ciycjmyh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dfbgspju.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dahdbvra.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3udojpgzr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3oqalgyyd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hsdwxebm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3izfqiblq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gdhjdirs.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uelpkndt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xmpkgvvk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gqmzsuqh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ioxainzi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tnjtmgcg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3obdonpmk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3oyoketor.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vehzfjpr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tqxhtqwm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbcbzrje.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vhaqpfkh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ukmeyasy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibqfiiou.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gnejdflw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3cnziflcb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3milxsajz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3lhwzaams.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ibqwbeqp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pvocdrnh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bgfkakmg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fivmhijo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vbfizgxf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pmoytzvv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fdrsmkvi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3reumleqf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3tglancvk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3krlwymrv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3oayoswhy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yivvsfnx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mlgpjnne.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3biawnnue.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mosnxbgp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3fuecdrci.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3axgpbqtc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wfknjtlt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3orfodaww.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mwvzqnta.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ukhxqieh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3muelrxca.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tsqptouu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3svxajmng.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cmegdnjh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xzkwyjbf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lxqshtfq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xnouvrtb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qbxjbqnf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fwkfuzkn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ysggllub.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3moxoxgst.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ajpzeckt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sjmoywub.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3itiylepa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3nlxowadc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rurkbjtq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zxitwkqs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ffzoyske.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kiwritvn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xcbsyjuv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qvjucpzb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fdapvbpv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3otpwrduq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3svebuwdc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3aqaokegs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ighcxdfa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zmarjkiz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3hpyrxvga.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3uyysgvkv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qrsogdmj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3myzttsjw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jhhjrxoc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xalyrubo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ilutwmxm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3fwehaxoc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jtluchkw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dvqlbkls.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uldeaczw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tkvwxrdq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ftnxaegz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jcevyzlx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3kbbevzih.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zlenvhyw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jpahlkno.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ecpifwob.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3pjoagcup.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mcrimqcz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3yhiumpsq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gxkfrijm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dpzhuftr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ellhjcws.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqjmhgcc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3powvyqsg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fswgmdlq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ovxnberp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xngqoeow.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ljckkueg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3xqwcijbl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3opnntwvk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wthyvxhi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3hzsivcek.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zipbwrjv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dwujcutu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3niusvjyv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3arwqswmj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ksopuovq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3acxxtvyk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3kmrhkayn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3bmjlnmzl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pkmfsxic.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jrrmfnwz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3feblzcda.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3asssncjx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ndiwtnvk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3uetrdwdj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lzgxdyaw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jwkxbobw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xzkwypfb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3epyxddad.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lesmqwnu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hhhejqnl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kctmoxkr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nimlftzk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3djovtfwy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eabepama.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xsrgeofx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3joxvmtso.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3fmgstxck.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zplbscaj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vqsfvuxu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3znjiwsij.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3hmnrhgqi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3viyoplgg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jdvfxupx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rcerislw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uxzptaqc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3cagsboer.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hsaelkge.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hcsjooim.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqkzfjxk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fzngtcvl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bgexzpze.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nyoibcyh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztoctyqb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wmeqzcav.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3aopzialv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yblcnbvh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bvtdbjyd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3aolrukcn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qzbdbocz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rcvwehyl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qnxqsmbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elziniiv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3owfqivfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijerkyyd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3imdzwdjk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hsutlwhy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3orfbrbki.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3uspqhapp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fsyzreyd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wzhyqbmp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gavemzww.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3opjcqalj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kgwutnnn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3chjgrvap.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3vajkapui.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lgaoakmm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3sqdlfpvs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3opcbwamk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3oqdtyetx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3fztqullc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3bwkhinmx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3eipumqjv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nypcrpoz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rvmldplm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3svjpbsla.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zpioixuw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3woyrltuv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3orvksbio.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hvshdtcn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fldgvish.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zahngqbt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xuvgeylm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uhxmgjlw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yepvskoh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vahdxksj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qazuqahr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lzphmtzu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3urzhjzbi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vqeytltt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3lsemyeeq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3meejgkyi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gxvrgvrh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3jitrcotm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3urmazjms.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vpboiisr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qjshbpbx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3knbslktl.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3myhzauou.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yhxnciph.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3xcmatiyw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lfbtvrkh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qzvnxitk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3puvfbpmu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3xbdpygry.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3uvnykdhv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3eycmuajt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3lwcelnjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbzkqehu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3kcsbuxfu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ceefbiuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfybeppd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3blfzmxsi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3sbxsduxm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lkkyyaae.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3amigeesp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3wojvumhz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tsevjbcv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3svfwrgfd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3qomoynkt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3avcpzrrs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3uolmpvyl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qboruzca.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3dumsthjf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3bewhtcpr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3wnzxjuss.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vkjbtcze.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3hddqtwjj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rffhlbrn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3zzwckmiq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3upojugls.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3jyezorev.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mvramjxh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3stvgrpvo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nqsymqlf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wllrqwbn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zcadajjv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sykttccx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xgjpvgvs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtkvxnpd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vrkktezx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ldnhhkkm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtfccebf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3znnpwqmj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhrtccam.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ipkslyur.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ggooufjp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yrhmuoth.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3edjwkjxo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3oenpukbv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esdqikgf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rlryzndx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bjzbgqnr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oxhznttb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dhtgpwfn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ntczeghc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uujekyir.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3btgwbkjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpixoapd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uprvtumc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uerlbuuw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3emkmgqwl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3frenahnn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3zhenxlit.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ygqdpyae.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mbyyzhqn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tafxpfnh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qdgctgri.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3efjauagb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3pqjofzwz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ovkgozxu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hkrlrwht.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hwmfhfui.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gvixwgtf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3avziarvk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3tqcqlcxt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qgufksbk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3rpsffjww.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3stijaimt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mrmqejle.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3notdxfjl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dpbosjfc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dqvlmdfy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zsmawgja.html


<!-- 参考信息 -->