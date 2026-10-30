代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gfdpyhesu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/goiruguqa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gdffbwewo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gedpleqyi.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gfcsjfxxw.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gumseypca.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/ghbytxftb.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gxpxwtzrq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gwpwymrnt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gzkmqqmhd.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gjurfacml.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gzdhuracf.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gbwgvcjwq.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gjgihxyna.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gpszazvlq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gncopmiph.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gbhwrozds.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/ghpvequor.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gbghxkdwe.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gdvkbnzpx.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/grpkiayhg.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gbhumoeem.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gsjpxvygs.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gfbnsyoyt.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/glhsbchyb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gmedwjdfw.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gzduegbka.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkabvny.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gflbghzwi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gsfestlpr.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gcutvvgte.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gzuomrqjz.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ggztjdbbl.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gmesflpvq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gvmmwhdkm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gajcncxby.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gygeifjej.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gjjonryzn.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gposhlytk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gbcumrdpi.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gqiiyxmmm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gthwotiqm.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gmffdwwld.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/ghzcqozda.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gozcasvqh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gavgkgyyl.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/golgkygze.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gatwoycdq.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gqehjuosv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gyowvcpjb.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/glviscdyc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gzcphvkmu.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gpjeaugtg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gbsqjfnuw.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gntefrqzp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/guhifjyjf.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gwtggdmxx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gbbyjqvit.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gtqnsbhms.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gixfmqogi.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/ggxnxlesf.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gnzxzlqel.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gygsprxdl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gjxsbgzvl.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gncgbteyz.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gzhlrhnfy.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gahacffne.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gxbihawnh.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/ggzmfqwfy.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gguhnkfjx.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gsxtcjhmy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gltvdscbn.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/glsbylxlo.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/glzxkhjgs.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gtazdtibo.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/geyuoofhb.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/glcknvcal.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gdfexgxly.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gnbuzbutq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gicpaxopn.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gsvvutwpj.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gmclvqwhn.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gsyouknre.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gtpidaord.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/givewtntx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gdmokzlja.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/ghfvrfgpm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gqkrtlehf.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gaernfenh.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gvtsxmmgx.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/ghknhakps.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gfaawoyyu.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gjshsqhbi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/ghbpxiiqu.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gqqxdoigu.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/grindoelo.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/glqdkzdpw.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gedhmwubu.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/guyseeqdp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/ghmujpbjf.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/givnnwzqd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gvwhtudku.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/giytqjcio.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gztnpltcc.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gloneinai.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gwxnypupy.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gsqyaodaq.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gsptazaug.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gooxoxyko.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gteblwirp.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gpgaefqih.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzhxncnni.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/guziscpxn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gaujbzviz.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gsndmwuoh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gsfuritac.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gbtbetavv.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gkoxewqlq.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gsvhomlmz.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/guossapbt.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gqlrfpwft.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gjkitdrij.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gtewelmqq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gaahzwoyo.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/grdjodlnb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gpabjjuoc.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gztozpkxs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/goiexmtgr.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gmsghltyr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/goarfqrqz.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gsidteclt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gqgqsumjb.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/geaoocsxz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gwuoykgaf.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gtqbfmiki.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gsnknxggn.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gvvvbnivr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gdupbzquo.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gwlwminxk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gtqvwngtl.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/ghkljfjyu.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gdxseyifh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gmrakzsog.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/glldplwfg.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gefablmlo.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gumhqbxtw.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/grwkzlprd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/ggztopucw.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gltrrvuzs.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gtbhzjcno.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gfioondhg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gyuwksnmh.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gmxrxxney.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gpqpaynil.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gwvvqwuei.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gsdqgbnwq.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/ghotisvne.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gozkwgthx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/ggunqcbog.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/ghwevderf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggibulwsb.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gfghabadj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gerjopcon.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/giizgjqtc.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gsbmkvylb.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gkrkiyckl.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gwdohgutv.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gaxzfpnry.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gtnwkivsu.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/ghdsdymvm.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/galqqktzm.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/goauvvufg.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/ghkjriozc.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gpvurjuzf.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gopcjqadx.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gvtireqil.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gvavytmwu.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gdnlijbyw.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gfxlkndcj.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gnixuhpaw.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/ggtnmwndl.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/godunytem.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gfycgcajq.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gnvcegcon.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/ggxuvmjqq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gassmjvlh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/ghgkyyxeu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gqovesnbq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gldedpllg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gbjuoiurv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gkpaxbgmw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ghvlcvegg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwbhqzqvn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gpeyfkntd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gpqfomsrl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gcibtodug.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gykfixcyo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gfyqaaltt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gpkkneuok.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/glakmmfqa.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gjinmpkmb.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/ghivlkqrn.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gbshpfvsm.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gpghoaagh.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gqboagtih.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/grsgrldhx.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gdsbsamti.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gpdoqwimc.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gocvmjyob.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gjuzfdzse.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gsgwjwmkm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gocuftdfe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/grsnqutsa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gsulmqyjd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gxaejstzr.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gtogewlfi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghyldwuxc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gkvbwqeob.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/ghdpumtpo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqitgybxc.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/grymrrbik.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/grfhceekh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/ggbhjjrhf.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gzfupuhzo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gxitlbaos.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gpkgijkrl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gafjnznyk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gdjkiiqhs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gnmpbxenk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/ggidsnkhg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gnackvhqj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gczufnqpj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gyxwavsko.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gcjalottv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gtcuzpmsr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gbgfzvojh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/grssrxehy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/giyiypumy.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gaysnuhnd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gskemavay.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/glulxhrnc.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gqgqhvyjl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gfhilqzaw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gwdlhaiuf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/geobaxeto.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gafxhrvqq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gbzjkrggh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gymcayttq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/ghlciowai.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gefbisfhg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/ghqlrjxtw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gjtqnbzgq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gyqkdzyos.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gdkwjnvae.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/guterxgps.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gecnbqygs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gfpoffvlp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/goikmlmpw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gqmojieqq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gyymbbylo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gsqvzuigx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gpibrdzqy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gphrfgswn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gkfbkdpyl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghnfravhd.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/goqjvsfwk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggygbeqkk.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/grhixhtmh.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/grnsxxlfu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gckrwidbx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gmztxdewb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gwcvjkgei.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/geurslowi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/geizpvkia.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gfcoiugmf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gtaezbjxb.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gvnkicsaz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gvhternsl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/geepbufza.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gvfduifbo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gtipurlgg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gmjeepzro.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gzjrwbqih.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gxlmrllyj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/goyvhcjmo.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gdydenqvc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/glavmpcfh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdndvlwzv.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gezcznlqw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gpebqoumv.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gjmibrwcr.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gytongyls.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gftwbzyuy.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpenzosng.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gzluaviuh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gcdsemmwq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gpdrauboz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gfuygyiyr.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gtexkbokd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gkkgedvrv.sHtML


<!-- 参考信息 -->