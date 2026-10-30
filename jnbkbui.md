代发 wailian999

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gswnjieoz.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gmuxobvct.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gjvcywpky.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gjtdcmxlf.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gzoftuwoq.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gkzpcxwsy.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/glsbebofl.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gwjaklgxn.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gzpplddry.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gphkmectb.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/godlcgfzw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gxifwomcz.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gcqqdeqzv.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gvswilogl.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gkkkbyucj.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gnrxowfkl.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/galljrikx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gcsvqrzlw.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gsnokhxze.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gbifwghmh.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gaijviexq.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gzwrqwfri.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gqcgcbcmo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtxuvtrlm.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gjmmqowkp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gsnoyoqmz.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gblqtrsuh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/grzgihuev.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gluvkjnmc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gtdlhxgna.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gukaqwqsz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gjibkdlom.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gwrlkskyt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/grllkjehh.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gadmceepg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/guvxjrovb.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gyvidymfa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdidllrcj.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gvtrxbrxb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/geviknmhz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gtlvylhtn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gwamavapv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/ghvqjgmal.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gjgtacuvz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/ggvlywjuc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/goivfolpi.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/glyhbpbkq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gnijnebdt.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gielmtqxt.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gpnghrazb.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gujovblsb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gfiivmkva.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gunlbfglw.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gxpsrurqu.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/givjlilbb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gupbietkt.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gzddjrwet.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gsfgcallq.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gacjcvkcz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/ggcrrokpg.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gkzccgejm.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/ghcyaqiom.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/giqqsbife.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gdqybqhbr.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/grfmusubr.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gkgjblnei.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gbprzsope.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/geslyzepc.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/grmsefuxs.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gsmpxbjjr.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/giqnhgzfk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gdzfztcib.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gcrczzuwh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gvybpsxjw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gfztaudle.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gpkbwdqfx.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gxtrbvvsk.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gpbgpczid.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/ggvtdemqw.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gtzgyztdn.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gudozutfp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gjonqoprx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gaofqoluq.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gdedijrzp.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gzaphbgzs.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/grlkazfbd.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gqbdpqkyl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gaawygewh.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/galyxqqwo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gpnomkldh.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gocmkvtii.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gabbtpjde.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gkvosrtdq.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gvubusmed.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gnbpkxbma.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gcfermcku.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gibhfvwqu.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gepuzabdm.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/goqllpnje.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gegpnhhkh.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gzefrfdcd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/giumkrugk.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gbzqhmqhl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/ggnvqivxi.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gddfsestq.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gnyukpjpc.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gmldzmogz.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gsjtpmlgr.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gjdnhzgmu.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gyesvofsr.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gdjuddeux.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gvzadlrkj.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gpeylpfpb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gjwkkjsqt.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gagonqnvg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gagqjeptd.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gtiyjscdp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gdguejurz.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gpooulznb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/glorijlli.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/glmwjqooq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gxbjrrrhd.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gxglucroa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gullprkfw.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gzgyrmaiz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gytcxtvbp.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gdojcatss.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gjcetsdri.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/guliumtmj.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gdfngpjpn.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gkbdilsvv.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gmkeieucu.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gbgwkdibd.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpemgqqnh.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gelhjbbfv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gcmqnrnwv.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gkljophjc.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gflchwzjm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gcaybcsip.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gexsaldsu.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gnetepjff.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gbbbeotpt.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gtrvklloy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gspmsjgaf.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gpwhsbtla.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtbmody.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gfqmmttxt.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gllcuuaug.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbjmmjmlu.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gmegekqtn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfelcrzye.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gvsbpmswf.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gvsqcxrqs.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/genmdelvz.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/ghmrulasc.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gqpthnvbr.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gvlqljniu.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gygcjvmzr.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gtjhaldzo.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gbgwbvvsa.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gmypcehjs.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/goaietrgd.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gahgbbxtl.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/grcsuqzhx.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gcibmfftb.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gtzhowyix.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gvjwyhdfz.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/glnalsfwj.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gyclqpdsw.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gpkixgrka.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gwqheurli.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gbyfnvfgy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gbsswfhdv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gtvqmtcth.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/glkzjujmj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/ggpwrllnr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gaibtelwd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gnpamvumm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gngukomwn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gnuealbul.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gawpvmlat.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/grprnkcmg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ggkvigzpi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gyjinunkc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gcgmuvhku.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gpefvnafb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gqiqhamkr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gzinxebsu.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gvoquhxzz.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/ggpgmxbot.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gnsiirrgb.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gtdwqpwfj.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gddufgoji.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gibxossxa.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/goyrmhgmn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ghaevfiui.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gtfapjiib.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/grnlriosr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gnmmpbbnq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gugkttnlk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gobihzieu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gthmllivi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gjzwxzdvi.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gyvqfujcb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvxjweftk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gylrbdzuh.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gjsqbwaej.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfwsxpvul.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gmokknmfv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gacervzmn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gkhfiwpir.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gcnwkjkds.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/ghjhzdmzk.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gywrogavw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gflendzqq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gdnxzhpni.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gfswqptor.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gruvgcjdj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gaesbpiuv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gzeqjvnwp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gbmpgdtku.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gmqvnncln.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gskvuzcmh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gqfjdgajz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gescjpqmk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/glcylwxzf.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gkplfcaxz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gwiluzegp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gaktybnhc.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gosnzdrhk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gqwgfhces.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gylcvkyzk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gicrdfscb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/ghkencrxj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gomqceeos.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gfzaxeemm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gnkyimyjv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gozaykbgj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/ghldldahx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gidxvkkjx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gqgchqhhu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gxbvrvvzq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gskytcdxk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcpmzpumq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gcxcrycpz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gtjsszopr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gqmftzuij.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gsouyukpt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/givtqatqo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gytdnixko.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gawuujfqz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gjayqkvvw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gftqfntvz.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gsrgoqsan.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glvnyjvrf.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gplecytns.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgqxhopz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gyylqujso.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gpykgmtlh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gkzljaors.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gkjilhgbq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/givfogvkg.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gbghsijmr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gtyaytwqs.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gcfowsgqs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gvbsrjwiq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/guvcqyfit.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gqafxvnva.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/ghhvissnr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gllbjdoqs.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gtgqcsykp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/ghkrkidkv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gzlycqbzu.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gnehsgnno.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gvzqpjrzq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghqnatsaw.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gchlyeelq.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbyhvenam.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbqoteody.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gbozazkjv.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gduezuezd.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/geofpyzij.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gdkawursq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gvkbnviun.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gozodvcku.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gkpajvpck.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/glvpwxiky.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gkksyiimb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gnobvlftp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gftgirtpf.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gxxamkkew.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gmrwnqhxf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gkaethfpu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gvpcqtcyk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gaymgzuqr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gjvyhaxdr.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gtryocjnn.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gxndwafix.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/grcxmlcag.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gfmhhtajf.sHtML


<!-- 参考信息 -->