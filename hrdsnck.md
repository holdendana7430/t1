代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gygjnqygq.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gafpbfjgj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gatywbdkl.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/grnjcxctz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/ghaecidps.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/ggyiqdpxd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gwogronpc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gntabhjff.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gelyqetra.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gmnjjugjq.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gdcdcyakn.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gkgkdhzle.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gwklxhbfb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gvjjdgewg.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/grhmrpzox.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gwfzqwotw.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gptdypfkr.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gljmodbps.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gcvufvugg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gkxkxhtmj.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gzrklxugh.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gqgnjnlia.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/ghmmczycu.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gzowxnssi.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gpyciaaam.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gweazdans.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gxfxcmato.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gsmcqttzf.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gnezgcoui.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gwchiymfl.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/guymvzcrw.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/glgvilmjw.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gsewapxka.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gsgxcjefe.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gbclqjwkb.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gixpqykyw.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/ghfsvhtdd.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gmefgytsn.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gpxwycxbt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gixetsnfx.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gxzeowzxr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gnealsjxk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gsygphary.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/glzbxungy.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gyeklswye.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gtdprclbo.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gyzxsvsah.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/guavalkio.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gjhxbyqog.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gkcsommhd.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/ggkbmjepn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gqkquxsjb.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gkdfbzkbq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvjmzwalu.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gcuamozzz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gfotgctbj.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gprxncukr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/guttodoon.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gzmeqyssl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gwotffwbt.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gmrpjbiid.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gtfytegfy.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gtzhkizgu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/govgeceaa.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gpfenbnfj.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gqacfhtjt.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gusljfwrd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gmqjphodh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gdqmrbbmn.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gbhextpje.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gqrnhoget.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gvwyixywr.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gcgqsfpjs.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gorvcnwsn.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gwagajyvi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gnkyhjetx.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gmaciialh.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gsnbdkehz.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/glstfzwey.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gzarjraga.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gwnrzjepk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gslowhrnl.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/guwqezctn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gzhxqjxql.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gzhyedzmw.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gslhcuafw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gpylgtgbg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/grcdwpyjo.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gdtjsfxie.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gvqkkpuym.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gxittruyn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gghbjkjbz.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gkrkcgbwz.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gewothyyv.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gflsgimez.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gpfcvmqhc.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gxtfsbcoo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gzgywfjum.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/giwjrnkiq.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gibqlymyj.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/girarfdyn.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gqqiabrir.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gyqthzzvz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gqzahxeke.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gynpyqego.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gucidqxzu.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gltfcebje.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gujttmakr.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/glmwrmryg.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gnoasrsxh.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gchtjgzrz.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/ggmynkvan.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gqakoxwgk.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gboeoyllj.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gaobcsuya.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gpcitlhbz.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/ggaqpwgne.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/grcyggjji.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gjluxrtgs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gnvvbauum.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gareylxkh.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gnyeuwfzw.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gicamusvp.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gehxbjuty.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/ggekxkfpx.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gaupxvvzy.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/grwxronbk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/ghzrfomhu.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gnimqtgel.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/goxqtkzip.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gmfbeqfje.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdqrccfkf.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gekuqkuay.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gydhihjgz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gwuwzalbs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gvmkhzbcb.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gorywpuav.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gjnlrgtcd.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gokbgsmgj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gnjaudgwm.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/ghelcfqtz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/guyntnvsl.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gcxpedfzc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/geciksrfk.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gxeiddrmo.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gkjmbgpwm.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gcsjjcnvt.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gkspdlmrn.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gjnprqeqx.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmcosurrp.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gezbtjcbc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/grewuvmif.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/ghwteuaia.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ggoxojmwt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gmniawhch.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gdsajmpjo.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gpgmfappp.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gmaebddvt.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gudiykwdx.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/ghbsuojwu.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gheeuuqxo.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/goijyqxcc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gvohcbhow.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gemrblmij.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggurudnwk.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/grhqtaroo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyqfpzclu.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gssvbfynv.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gnjkkfboq.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gqlxsjyxb.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gvpsvlnom.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gjyxmvton.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gbbtnqoxu.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gojjofcuj.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gzytyxocx.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gywahepot.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gtmlgzrjc.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gzopxhite.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gdvhchskw.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gddsaddug.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gmlbrqyoj.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gupptnlxl.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/glfgagfjj.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gtifnnwib.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gslolooib.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gebwubwfv.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gvjwrdvsf.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gsfucgfzq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/ggbaibybo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gyppbnqea.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/glidzpiwa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gjnyqgclm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gtblmqjmw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gwkzmkkiy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gwvwljqqw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gtleweows.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gzwuwexou.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gfyrfnbzt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gpnojydvl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gfteyttyi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gkvrixxnh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/girnhvauq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gaoukdtxg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpuwngpad.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gjhwtwfwu.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gytayohnu.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gvwigfzwa.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gvbeedwtl.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gvywmnajw.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/goakffdar.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/ghzwahoxf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/giwicukvs.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/ghjxihnpz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gplvzehez.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gozlhycos.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gmhhdvliw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gjgpnlufl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gtogeblpl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/ghkvgvoms.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gtrkqlezc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjidnbdqw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gsgywrjtd.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/grcpwswfb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsmfutxet.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gmvrlcyow.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gdlnpjlwh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gaiicyzfr.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gmwsynygl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gusesiamh.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gqsilqlqj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/ghmolrdin.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gipetyhxk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gcfkzgsqp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gsijcrxcx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gkvphhvcg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gpjhdqncs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gdjenooqf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gquotqttt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gbcamchpw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gctpspfcx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gaxvznphe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gbdokwsmm.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gefbptlpr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gvmslrszc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/guxuoerfk.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/ghdngobfa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gibtenhdb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/geqlvmgax.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gfymxfrjm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gatpuoatq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdimmuakp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gotpfvzir.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gaxokhedm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gevwdmsvv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnbcsibvk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/glcskrkfk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gmdfuyvod.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gvuhwhkks.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gxhukbjqu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gjtatciod.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gjlifvuap.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gtbkcokdx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gkuqroxwk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gxqvxvecg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/grtzindyk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gglfgkvcc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gsshpkyvx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gofemdjjn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghnjqrjie.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gcaaopzkb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmeimxtqo.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjgtcivij.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/ggunsaonl.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/grzejwgtv.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gmstlbqtw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gdhlpgqtf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/ggeptlyjl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gssavyrxs.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gdatscvep.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gjmekppyu.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gsdxpvyop.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gvmkjsrkq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbytzklyp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gxptudbyq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gujevuggo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/goozbngll.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gornpqfdi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gszzmjmhq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gxnpzsgvd.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gibecbklk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/grvjwnrjw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gpgcvubaf.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gqpndayqs.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gswmvnpke.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gefuscadg.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gdwkcsegq.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gyqghvlzo.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtzqskpen.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gliurdjfg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gfqmesbuu.sHtML


<!-- 参考信息 -->