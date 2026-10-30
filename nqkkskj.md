代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gongpvgtc.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gsbkselhm.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gliuwwmcd.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gkvkuiuez.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gpzffkboo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ghkdbhhgq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gtlnpjdfy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gtxtmqvtv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gdtytjecc.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gcnroowql.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gksjrokwp.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/geegwnwak.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/ggiomukeh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gseodvfyy.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gfyssofzu.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gckjfpfnz.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/goosnfjwm.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gkbfrkuxf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gbqubdgeo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gtwkdxdwg.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gylakwmyt.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/ggyswsung.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/ghidvuiod.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gefhthnwz.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gtkaugzfi.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gzqeawubh.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gjxwpvvvd.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gcpdblwjf.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/ggyjifrqh.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gywiuiktu.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gwldwtwon.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gfnauslvh.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gokohbcfa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gvbqtwysx.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gioszqvzh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggajcnbwd.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gikzwdtae.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gmlccspzf.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gpvqswnol.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdwtgrcmk.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gzibihdlb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gcztjocge.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gguxmlpnq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gysrkjbnl.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gbhhbqgww.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gsteaexgy.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gtrbojbvj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gmvmclkrn.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gjnffqdib.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gjweeekmr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gpxfxdbrj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gfebcwaoj.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gstvfjpav.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gvlnjdywo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gcmgxdlii.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gcrwvlglc.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gssimwkgf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gjexrnmoa.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gduheebvu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gbluoixoy.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/giplecowj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/grnbznitc.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gcqiigxsn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/glmihujmu.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gyovflhxa.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjwirxi.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gaggjhbkh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gousucntj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gyjgfzeph.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gwytgezin.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/guswqiaim.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gxeiwftym.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/godzzzfng.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gpmzhjszj.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gphwdwhsx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/glpzwfvmj.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gwuuxvhjh.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gnfkjpmzu.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/grktzwwyn.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/genxuhggx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/ggtprxijw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gaeajbxll.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gzujkahrm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gaqvqnktj.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gvrkpuiew.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gslpgktmj.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gxenjzdvm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gtvztrght.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/ggoubmfbm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gjevbhahd.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gnddgtagf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gmxbksmpa.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gwuqznigk.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gvdcsrsju.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gqxoulctd.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gxpquzgge.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gnamejdzm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gtkuyxeox.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gvtpkzson.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gjftimgcw.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gexfdpkjf.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqbaxufay.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gkwogppib.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gkogahzie.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gedkpiday.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gqdhcelgk.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gvdgtfigg.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gwfwxdqjh.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gotrdlyce.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gyyeffeox.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gisjcdlad.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gnrmwvzcm.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gufptkgrj.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gfgeiuzbm.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/getehsbss.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gckturcmj.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/ggrjyigak.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/geqrllshg.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gzgkjuutb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gvcxjdocu.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gmgqzfaat.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gdygipger.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gokaladvl.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/giwnoyubf.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/giyywpdvn.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gyziejhpg.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gurtefoek.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gjpqujqdx.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gdmgrzknt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gepkolwco.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gdvlxbzgl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gsenudnqu.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gexgivaal.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gcfpqiexq.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gabfvtgob.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gcyyyqfyw.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gcayhpcfm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gbisaylrd.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gubfawfqg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gdfclkrbu.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gawelbjgr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gelhsamwc.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gahjhvusv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gifbshmes.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gptuyskae.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gtjgwfbfk.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gddlhxluu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gppjnhpky.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gfvhdfarl.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gmvpruxlg.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/ggoziptsg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gqlkgwyvi.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gnreryhbe.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gdovzmnsd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gemcgtmsj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gcetramrr.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/guqyqoglu.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gvaifufzu.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gbrldqvbv.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/glcutixic.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gmqrxtfqq.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gqmhmgltg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gfxvxxsuw.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/ggfgvlghd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gahltbove.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gbmzfsjjv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gihloqwds.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gpjzvxcdz.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/grnptlsgj.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gormosgar.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/guobusyds.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gtwqpewhf.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gxejupayf.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gffedaxqf.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gzbaratqo.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gvqehbzep.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gxaiettst.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gcpgvqbjq.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gwzlfoxcr.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/godluuakq.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/guctlbspd.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gkzcjjrrt.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gghdouxli.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gxyrkffvj.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gpcbeaeza.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gvncbrqib.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gzumqyqcq.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gszspvsnw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/goscwawzy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/geolygeva.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gnnietzin.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gfxzawkbd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gvpnlmygm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gixtcvdsh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gwubkauvl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gjtjwzozq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/geklqtfjc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gkcsbrcmx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gidotkoaj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gkynxgqxd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/guieizqvz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gkcuptnxt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gbxgoxrqb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gczfrrfyy.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gtcqnftcg.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gmxzfvgmr.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gyxakhrxp.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/goadpntru.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/ghxnxbnwb.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gwiszunfu.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gtracisly.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gxwdppjlq.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/girgnnkkb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/ghimsnzoq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gruordyte.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gwzmyppic.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gphqsartz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/geidnjhii.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gpvmyvtxi.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gdhrmrssj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyvxbgkct.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gfegqaact.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/ggjnarbir.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjujbbexl.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gcuzybgwk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/giqikibej.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gsvglbwft.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/glztvwkvf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gyystilai.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gyujcowut.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/glllgqssk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/ghagioefv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/ggxefvioh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gzwfjyjrk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gcgmzvytx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gxecbeyma.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gqwfqekrj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gbrhigsgc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/grrsvjrxp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/ghhmczpfx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gseryuoru.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gzudneyqc.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gmogyribk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gxfumsvxm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gszxhlwwt.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gdjlccmlj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gbxtpudum.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gnmshsesz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gukghtszg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gnunbkrta.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gwpjpogyy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gbxdxwmym.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gtmouuujv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/grtqdaobv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/ghfztppjf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/guxxwbcqy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gmjlgcrha.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/goluulyhu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ggzkvidul.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gvjdnkoxs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gexuvudfc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/ghghrenrd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gllpfufmx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/glxeuhdpi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnkorlagl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gayfntbmf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gojtqpzsm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/geqjnuefr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbzoosxzc.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gncimuiza.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdkcaxbgy.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gdznqgrhq.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gdiwoitep.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gwnsikkgn.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gkivuirlv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gptexsajq.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gycghlaqh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gxwdvhkmm.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gjjrbykya.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ghgpjvhpn.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gvqyifapp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gbnsctito.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gfnpbtevd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gvmghdejk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gwxihicne.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/ghetwonei.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/ghrqnswex.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gvulqpxbk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gbvozqhny.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gbzpgzdei.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gjzoaaurf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbxlsbcey.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gurkszoki.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/galmtwfbs.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gmwcyusih.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gyabijozs.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gpldkgwee.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gzwcdjcee.sHtML

[A04] 判断变量类型
来源：http://read.share.fehbvm.com/Article/details/gieiwjitv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gwtqhzhzr.sHtML


<!-- 参考信息 -->