代发 wailian999

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gfhmrfkuc.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gtcktptnk.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gnitbmyvh.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gevbkzdgm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gdjkwhatp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gjkaupxbk.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gzjeiglza.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gwkhsxmxn.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gtmohtmry.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gqvwrrewt.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gcmhinydj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gmifqtzyr.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gpaibrimn.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gqnkvgmlc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/ghexigaoc.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvwoefctz.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gyqplsgwa.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gwgdaxfbh.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gpmaybpux.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gvmyxbhec.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gfimocbgj.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/giqhcdwyl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gelrvhfwc.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gsoqzyfac.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gahzehznq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gdydlwhir.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gfchmnnfu.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gtiksjjaq.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdompeusz.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gokyyxnnr.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gjgqvmxww.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gcpuscxdx.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/glirxpaqe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gqsffcvgx.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gbyezicib.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gnesbfjjc.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gpnihayab.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gttxxkbhe.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gfavoahia.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/girdqybsc.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gnwgqwkwl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gikryrnbp.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxxcbbsup.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gfjodjfir.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gsciomzio.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gwzcchmkm.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gioqobzqh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/ghobhehfd.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/glmmczbtf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gpspnlpzq.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gatdsrfig.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gelqtpaij.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gfqtzaqro.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gotjfnhxi.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gthtnddly.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gnijghdmg.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gjfpujzfl.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gpldxhlcs.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gxtcertmv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gksmkgzrs.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gktqgbygb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmceolrc.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gxtwzroaw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/giunahcgj.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gghsuowgn.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gwcduwgvx.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gcpnbpiep.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gynnblnsx.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gticxfzst.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/giqqfrbqi.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gimskagxx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gmcxflosk.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gsqgrjobe.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/geetqvycq.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gjokouejx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/grejmhkjy.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gagkezgez.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gkvvryggl.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gvanqmtem.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gihqfzxsy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gtfqlezhv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gzkgredqv.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gyflkpzwj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gjlxzzbme.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gcjzpsvjv.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gakrhghpk.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gtrbvbfwb.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/ggrgqxyws.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gdjfdfgth.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gblspbapp.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gigkjaqzt.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gqxisvacl.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/ghtxnjwio.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gsxrpmnow.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gcbdtvebj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gxeanpbws.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwljbfujd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gbngdvdme.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gykoeklxj.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gcvpizafc.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gmigdbods.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gualxymay.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gugyzkuza.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gtxodnhlo.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gsavdfbmx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gqhinnnfw.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gcbbmafeo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gnqzndewa.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gmiwgntrz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gfsynozqv.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gjegaefqd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/guaxmzsdg.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gnrkwjnwg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gjcvnuqpx.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gxthwfyur.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gjgqqmtaq.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gzfpinjkn.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gwfzdayqu.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gprsrqkki.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gclqfymtk.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/grskznmhs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gwilmllap.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gxiydoaec.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gfeljfqzy.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gxfzwglnz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/goejusdox.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwtiqzhuy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gisevgcqd.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gtmggiaip.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gvupvqgge.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gyieediib.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/ghklqyevk.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gxnkbvlgn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gadexfjdg.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gsjaekjpe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/guobjckjm.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gawuhdmnc.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/ghtnuzxwq.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gfazgivps.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gkopcytoz.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gtqytzhra.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/goaflviix.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gpkcqyiqn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gatfnxwya.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gvnpdzxtc.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gsqrokilv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gygcyfoyb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gffirjnxw.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/glbtztmpq.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gduytmzfo.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gwpegumsi.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gssahabtf.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gyuuushqd.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gcilfmltv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gkfpeeyzd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gueeuxmmg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcjtdahqy.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gcdlrbnnj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gusqvcuvd.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gkrkmypoz.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/ggdwqcvuq.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gxoyhvefd.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gnzkgpsiu.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gztldseig.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gqqqoczsb.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gbhphrhzl.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gfeztxklk.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gnldpvzmo.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gfjjrfvfn.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gssbcachi.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/grhhycoco.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gpayexcrx.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/glvoobksj.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gkgoicnru.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gmicciqxm.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gwwuanvqw.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/giwotajku.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gyrgkvvbl.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/ghgnwsfyo.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gckpwmxbr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/ghwkvfaaz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gwclfvlcw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gmhzstfur.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gsaahpyni.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gxxtmwnke.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gcjujipwq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gaojuzktb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gczwmdeoj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gjcjwaiav.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/ghzvxzdsg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gouvsqabw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gytsqlkuu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gaegfeoqv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gqcijyfay.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gdvwlaegn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/glllmhtdm.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gkaajslep.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gotdrbnqj.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gunaanzcl.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gzhbogazm.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gmfhjkcsr.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gwxlqfhbk.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/godklusxy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gicomojwq.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gcskcgcdv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gcdxdmhdq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gzbetvhol.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gtgzkwtop.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gaqnpdsxq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/ghdqeldrh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gqxifgrsl.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gvrvlfvvv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxnazvofz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gntckvcpf.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gwyjmpihq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzzcjjxqz.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gwsicysir.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gtogwasec.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gwnnakwyk.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gncjfsozi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gtvfanpzc.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gbbtndyrq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gclzvvfwd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/ghmyqqfpw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/glxgmcrld.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gozycmevj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gtzabwvcp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gfjaifrbc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gidtystsl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gberaphjo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gogddlduf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gtqkwppbb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gdtqgyqyu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gjlmmsizf.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gzspuucrw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gqhtgjcwv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/glkhvyxwa.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/guuqomxcz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gbevvypbq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gmdltzmvw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gebyqjtsr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gjcomxuqr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gkdrmfivl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmwfmjwdy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcxpactmb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gllxmrior.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gghtqafiv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gvxcqqjpc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxvehxrpi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/ghncjlocy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gwtkmcffu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gakshhfff.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gpvvdjvzm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/glhcghnxy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/glyrsaldv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gbgcoguef.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glmimidpc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gangasjet.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gpkxuomht.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gswhhgepw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grcnjpwfw.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gtiigvyza.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwhgnqzmj.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gdjlyhjzd.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gkmloviau.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gjukedmlk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gjhinywkx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/geukxkfyb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gtvdzrwtq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gsqypjzeb.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/giznxdhst.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gvvjubbpu.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gshajordz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gxspbvngo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gxylahmfw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gmtsvryae.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/goianxqgk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gcyfqobtn.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gnbacjvwc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gjyxvkyku.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gvxiycxxm.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gvmkxascb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/geookkgxo.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdgkhlezh.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gocamyjql.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gglstegyi.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjedquopf.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/grlsdkcrl.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gjpdwqbay.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpxwudpgc.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gnaakpkdm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/ghbmbqmzh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gtppvqnsn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gzkfaxzai.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/ghjuxftba.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gdvkxnhmc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gsizyvtxw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gkutvkfdf.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gakuxkdyf.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gerjnjdyv.sHtML


<!-- 参考信息 -->