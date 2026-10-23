代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3grogmyyw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lgpnhkks.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fxqoksca.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jomrmxhb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dbcdjbsr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vcahbwek.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ssgmkywk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kjpfyyop.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qjeesarl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3bhjqmxbh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwoeelwr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fdfduicq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lpwmknps.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrnbzujt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gxosscki.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ppemdqil.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qfuhfwoo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3uefbhvgc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uhfhmmfb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckzvwedc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bbbskyrc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qnqhslcg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ftfgouqo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfmerhdh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cspwagdr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3fpmudhtz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3oeimnicr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kenwwgjh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pdiztsls.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fwbhibor.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cnklyfsg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3lanckmeq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cqxccbhb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3liegurcs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qwxrgnbf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qhzfbgrc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bwegvvdj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dsjvcugb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gdcvdqsr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3umihgvfb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mexvlzna.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pnbyuodo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fpaedwqr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3oteabndd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3lhkzhjdy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxssgndw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ofqpivwp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3njsdnxit.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3qsjyqlrh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3pfejsyom.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zxxqjplj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vvtfnted.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ezmzzenw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnsyrmcd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pcpzwclh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ajjrdtoo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3mhwjchcv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ubgkoliq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jlxgrwhu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yfdynjvc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3svhszvpx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fnbjmnqc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jlwwxwof.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3raveoawj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ivyyjocg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3aioxxudn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3udvzhywy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3hkhqeaxl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jemkcqar.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rqspbass.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kwdlkplv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gackctgb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rhflrtma.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3szezkogh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zjfijcff.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3oodufmtz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ixtudwhg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hviepzrb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fqjhrdyn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ovcokefy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hclwdqvl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mdaufahg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ebieigeu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vweopmsh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bakabnet.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uoddszwo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ezhrdsdu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3iikdgmou.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pcoeqycw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kynelghy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3cqdwwbfi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tzdpkjzm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gkdaxsji.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tbwitlvb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kzkvfnzw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3grjejjel.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3glsesmtc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qdcyjzxe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ewcmyefx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3eflpiiwg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wobyomlf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3axfocmsv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lzgkfiro.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lxodwdor.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xsonmkuk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3jqpwlwei.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3iuibocys.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3efvglkvq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fibpwgye.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ncyfmbyx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3isezjigs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3psucdvsw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3neqwdqfe.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3chbzvuzz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ewwhkcwj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzjmivhv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ebqrpukv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kqxvcdzq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vfoswrps.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3orfizolh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mtlsjyud.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mvhbdzaf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ynaeeodb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3clkqzszq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pxvrrexc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3sizuzqge.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3whkdakay.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3npiaeznk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3abvsqvbh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jgmbbdsa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ziebdcab.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gxehqaed.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3okgtbsar.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wngbbmdq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hhbjqpug.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qdmvonlv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xuwuevnc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vwrtmswe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3foyizryv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uehrcaga.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dwjbzzvx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwnvsof.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jycxaluj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ayqgteha.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3lleqflbm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ppqzmjxk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rotyedpk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qzujwdyq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kzfgkczy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pdfnkwuu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3fnvugsyg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cseeuicw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3srbtpzrs.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ztanpmin.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3slmgxljk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqlrthhf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bcrmdmkt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3udtyapud.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rypuxhmx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hycjqxkd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3remynrra.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3nktwntjq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xgwniyxa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3iqhaewvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psuhwloe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ooebbkiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvtapcsp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ztfiinvn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hjkonlxd.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ytrporsg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yosuzvgh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gjkfcasv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vdmgzsta.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tbtvczdp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ippocuwi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ffbfgvrr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3sfjxrxoq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xjihmjic.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3enkbmxkc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zuzhpxgm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pkezgygg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wtmzwcoz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3vbhcvnrb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3goenfiuf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qdhqdjpe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pssgtoxd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3yiedahkk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3oloqvcze.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ujfizocl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3baklbogo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3txajuyel.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zqqgtkzq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bmwmzulk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zvxpialb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xvbbyiao.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zcglitbn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rxbdmizk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ypqmgvbe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pazefmbm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3amfnmtax.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fnzzleis.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mozqjmbv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kipkcudq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ibhzdhrl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3lsfqtjxy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ibjumlly.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uftpxlqn.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3boiapgge.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ncejnmgi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dbasitsm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3sncrmdnx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cmiuotbf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3uxmdciou.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3erjoeiax.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3wengtlie.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tdvyfwsy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mwjfghnj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3rdwwzvnl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3abavldbh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3wjhetoux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlprhhbu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rlyiezxb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pfxkwnwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxdbqzqi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3nqrnttpe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xzjdrlau.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gatdqpjx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3gjepdzpk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3fkkcahyx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3uvtayuum.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zcivvhap.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3zlmplsyi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gqjyuain.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3mpebpddj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ikztbjux.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wcrpmsnp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3iacfzjkp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3yvigjooe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3qlzkicgn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dstadswv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3gnjalfgw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3dbihfwfd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jwshicsg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3mqjtfbbc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dewolkle.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3aqsapqlx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nsndjuen.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dpfzcbqe.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zgohwebm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3odhcnkow.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tuezkurg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ywgicjti.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xmaplzvt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gpipxmff.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xkzdutny.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qdrrckhh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3llybosnk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sawyilso.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hhdqznln.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mcdcwrod.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3uvwwbhgq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3yqjnwcci.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtrhufbn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gcssvnaw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obxhvrvl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3xjdjtpcf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tvcnmuqi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pgowmatc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3audhmcwc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rfomzdhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bivnzetf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvaligwu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3mzzfbngf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3jdgegchc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cxmetroo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3exuiqegt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oespcgis.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wltwkcxe.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wlhgnbqo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wnwkites.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3djgaljox.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qqsiinzz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bdtyoifd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xfduhnmn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3kwujmlrc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nncnzlrd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qqnmlbkq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3kjocszrv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fdnjuuzn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3dsgairdy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ochyvdyk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ppsysjzk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tkslpfjr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lujsvywp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3orniclac.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dzbtfpsh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lyewdzuj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qafstdvd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bzysueas.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3cscolkim.html


<!-- 参考信息 -->