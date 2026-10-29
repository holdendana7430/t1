代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gjgitlhwl.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gtuhiircf.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/geppghtdr.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gahzxxtqk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gdijxglom.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/grpnlnvya.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/geqzhnvkz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gheaorssz.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gttybmzda.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/geaxscjef.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gwxpgqwry.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gdkdpvcla.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gfsbolpmc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gyksmlhwf.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gvbdbgjiy.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/glrklmebt.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gszwnsiwi.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gxkxtqkws.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gloaiotsk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gpueilyes.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gelspbytq.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gmlhkojqg.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gijrivnct.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/glgsxjlms.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gmzxifzdf.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gjzerxpwq.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gfgrwpptn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gpbipncyw.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/guaukpzzo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gtmmawcyx.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gewviifqh.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gnzyzdnpy.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gvtkhfdhs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gzbjvcfdp.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gxubofrdl.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gozfcmzjk.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/glkismhzx.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfllfqbad.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gqaaslkae.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsazrwkgx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gnehfosot.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gdulumxfc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/grlpvycwt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gzrulltxq.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gqblgehic.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gabszeugq.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gmaakjgct.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gmfauqquf.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gsszmwozv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gzuwuogin.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/ggkbgtymw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gbuslvypi.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gyxapicwf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gozaattrf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gevuwqvnf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/ggnldwcyg.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/glinrqptw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gcmewbhhh.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gdcwuhesn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gyudgwvqt.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/grclpfxrm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/guqqqyrfr.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gfhxkckks.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gemvhprlr.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gtfemdmte.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gooaazrcg.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gwpdqqzsu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gqtiwlqwk.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gzkyuoxzq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gvxjhcerc.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gtfdisufm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gpyvlnkff.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gyvjthcne.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gkrldgfol.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gyfsodxbn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gwudmzjap.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gqmzidqie.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gqmfdtksg.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/goaeshqxr.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gwqkvtqjs.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gdixpdwfu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gdkyflpdy.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gnbgegosa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gpkocexpn.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gkwmkxvef.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gmrszsjuh.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gdngrzfxx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gbqyzxysh.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gfuamechq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gvaicujfp.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gfyylowas.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gmgrqgarv.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gelvwqqie.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/glvxzhrsj.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gydcpbhmx.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gmrdpdybl.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gmtepoxbf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/glghbvonz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gsdwkwywf.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gbzpgstsi.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gnykobboi.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gnyhtywlb.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gkbjzqymc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gehobnfvh.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/glfhrecgo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gkotzgxom.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gzembpzrb.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwlrrqvid.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gddkujrmu.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/ggbcqmjer.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gdhujuquf.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/ghfnzooco.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/guzllkngb.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gnuzttzqh.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/ggwnefbme.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gwwyotgbo.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gwxevgyxy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gwxqdczir.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gkhfqbafw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/glwxbtdks.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gwimayzge.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gvxmxswqe.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gtztthrvx.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/ggpopuofn.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcinsihyn.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gopwftkvp.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gnjlkfpmk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gkptpvkbc.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/ggkpsqlox.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gmnshlwyq.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gfwxucivz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ggigfqsgx.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gmhlbbprj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/ggbmalgzl.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/glavmdkoj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gjxuwdlux.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gtttqmosz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gjlghdehz.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gipeewkhy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/ghckihwml.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/ggrxppxdf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gqzsgqkdy.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gyajbwvxo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gzwfyalsn.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gebfvjxor.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gjtpptfdg.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gjjktcuuq.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/geqtelicg.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gjgnvchra.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/grawbtrgu.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gplszcpai.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gbvovlzgj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gsefsitvb.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gmxdrzbto.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/glmsdovqg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gsvpsgzau.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gmhkosikh.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gipbbstnu.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/ggfnxzrnw.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gpskugjil.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gfawmfmve.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/goechlqqi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/ggkvqhmvn.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gfcmhvehi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gigzvrbei.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gibhswrku.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goktbkezf.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gxpiwsfga.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gkqwrrcbi.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gmcdscipo.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/ghnxdfult.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/grygumznp.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gzjeemfgi.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/ggulmcfax.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gacmcnmpm.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggvprksob.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gxlpaiabz.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gdzlrqnue.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gtvbfkawo.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gffadlrtj.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gghfklrwk.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gzagtlfku.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gsrlxilgx.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/grtqjjjph.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gkyassyat.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/guodcxmzj.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gdcdzwblj.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/ghyznrfup.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gjztrahmo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gcpsttpvq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gushvclpr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/ghcsruqew.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gkuguvmme.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/griroqvyy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/ghixwxrub.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/geowgdrko.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gkwcyjmne.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gvxsftalz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwzehrwla.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gtbstukwy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gxsqwrprz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/ghafddxxb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gbmukjnlm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gipeumvlv.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gjuqzluzk.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gqvchibfj.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gdzjlycdg.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gwzmppfen.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gqocnebms.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqwqlinuj.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gfehymryr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/givdeejnj.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gsarydwsd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gpeajxhly.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gyvpjzjlo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gvbzxvbgk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gkoigogss.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gjgbajhfe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gmfenkqym.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gudzccosw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvqnmghxm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gslyylvcz.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/ggxuyerhs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdthnhoxy.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/ghcqckoqz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/groxtewqr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gebjztbfd.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gbfvskzal.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gopinnznn.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gmtpzzxgl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gznmptllh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/grqqrmsnc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gqseizptc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/garhpyihf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gmrafsorp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/grjuawesm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gsuovvore.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/glsbqickw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/glnhpsfdt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gcuixtssj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gqewglxeo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/glmkinxlf.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gkliejioa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/grdusrpjv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/giwziqytg.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gbrvetcnm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gurkrodoy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/girtdoheh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/guaydxmzt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gljtekvad.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtrdgdngi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gktpsdvcp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gybjlthcn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gclcbavdi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gghrkdxyn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gryllotei.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gzelleisz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/grxyutloa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gsmnajywc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gmmvzzaaq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gtvfxfybc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/ghfeckspm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpqkymllj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/grdsizqyy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gpztcburz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gusyajyjw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/grpfhydii.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gwcyeijxg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gybcxfhwt.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gafcdgvwj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkuzxbypg.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gjvisntsc.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gxyvvktuc.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gghbyeocd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gagxwgkrc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gaepeakeu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/goknixldf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gzlrnzymu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gemmmjwcz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ghhwnokdw.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gwzrtorfu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/glkpiyvdt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gnanpocxy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gugxkzewo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gerccbdby.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/glslngvcu.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gtiordjmr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gxdxhxqbt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gossgopsd.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gylxjxzub.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gmmdzaghv.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gghhzdbbl.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/govpwucfp.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gfxxkcjad.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gcvnqfipy.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/ggyoqylnt.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/glxkdbwrv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gloznakhl.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gbijsiynp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gatukwszp.sHtML


<!-- 参考信息 -->