代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gjmxkrmtv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gkmoooswt.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/goftzxldc.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gtlaxznad.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gvusoddlw.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gdepetbip.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gghfvtaga.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gdfnpvoig.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gfyduuqnj.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gfgujfrme.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/glwqjjccj.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gsvejtmaq.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/geklledrg.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gognsmogw.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gmiwlsxxu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gpxgzvtxu.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gcarpxzqr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/ghdlrjxxc.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gjqzghbey.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gwzeavlot.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/godalvxau.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gyrqbodlb.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gfhkcjunc.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gvkanuelj.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gnvymedvw.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gqdsysuwe.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gkspeokgg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gsqakyksb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gnyvhhxbj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gukggrxja.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gwxptyjbe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gghanvhbh.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gubdlqxlf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gaqdxrlut.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gocxffrsk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gizyhuyyc.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gnoqgtuel.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gbwclhrwx.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/goxnbwpbz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gdfpseljw.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gomzspedc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwjctmvhr.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gsqkzvqec.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gcojoofgw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gihsaqhvs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gmdrpkhnu.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gboabyhhi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gsljpinuq.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gxnqrmaow.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gatlayhkm.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gdzljklcu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gtwjerpna.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gnkxajrpr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gqajsyntq.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gsvzytpge.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gqmqyxzhd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gnwniesvm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gvnvykamp.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gtuduvniz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/glgqizhat.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gfgviyvuq.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gnojembsm.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gcftmoaav.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/grtswimoo.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gkiqfkatr.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gurkjksur.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gghkswtmc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gjprfaugt.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gylcrpoey.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gozfdqwdj.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gszyqlpne.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gzabnqrnr.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/ghztuhfhv.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gcurzdtkv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/guxjlkadz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gfaldbhgc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gopuhvmva.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gqvdnzzfl.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/ggbmhmxmz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gyedshqfg.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gumqecdgl.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gvazdngjj.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gvvkytokk.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gjlghfbhu.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gfphvqfxd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gecfcazdr.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gsndjgaep.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gmldpqkju.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gnlzucnwb.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gunahwazk.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gygduurie.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyskbbrvd.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gtupxgaag.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gksfcfhdn.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/guwuiwmud.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtvvxtuzi.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/ghnypuwvm.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gutsredrn.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gdjgismjm.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gchsphyik.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gppylfnhc.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gdlunmnqp.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/giefckemn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gyecykoph.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/giyucvqca.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gxrmgblxm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gxcstktdk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gceujxjlg.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/ggpgbtzrl.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gtvzzagpc.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gmlmptloi.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/ghboxzfti.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/giswvvcli.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/ggricbwaz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gbkrhwbvy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/guftelbyn.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gucwufwjr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gmylbubsd.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gyoqktbkw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gvnzptdot.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gwtqxfchy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gwmvnnfeh.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gpvdcpzyy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/ggandnuwt.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/guwxqozwz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gshblfzsa.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/geptzlntm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gusomicmr.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gvtcbrsat.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gqluodsfs.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gyfsyzcat.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gfhradxrw.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gfmklnriz.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/girovyekv.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gftphybvg.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gafwwysig.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gxecsrjxz.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gliowgwin.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gaccpypvl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/ghlodwkdp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gfngttbpq.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/glfbxvund.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gtiwwzndd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/genrbxvzh.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/ggejylqfg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gqkwltaet.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gcdkxpnfu.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/geovxstoe.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/givztthdt.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gadgeojbg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gynietxzv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/guvdtlgxl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdznwgmov.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gnwsfevoa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwwwmnage.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gwftnbcww.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gyfqmxkwt.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gwgqvrmlh.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gcxqdeend.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/grodjqmva.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gdlkbyjmp.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gohqhoxwr.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gevctavtr.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gersefyjj.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gzrcpzerk.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gfowmszgi.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gbwqzesqr.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gsoonikre.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gjbzypoxu.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gyjmvksko.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gvxtmeljo.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gezubuazv.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gymxsrxjk.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gpytzhhlt.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gcmqgnreh.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gzpgclrhr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gszulndcd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grpjmrrzh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/glsahkpvi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gkonipvki.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gtvbnrmdf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gisscnaqq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gqpqsyzhk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gpvgnzefu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/guvkrlxle.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gvnparcrd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/geubzxzgr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gggphpkae.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gugcjbnaw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gnttqplvv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gxyswrvax.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gfbyhmusx.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gljwkdzli.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gbcqvqviw.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gwuasiggi.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/ggepcdxpr.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/ginpqhqbk.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/garukqvef.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/grfxalekl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gcjkbivlh.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gnphnfqtk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gkhacqjwz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gaxunkqgc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gwrcccsfl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gpspqeeyj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gqrrvpele.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gaxnjkgin.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gdyfavnxh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwawwrlkj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gekzzutif.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gaygqyexq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfoexuufw.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gbfknxmku.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gyjemaheu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gkobbjuru.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gepxssgbi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gkrmyzxds.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gzugipsiu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gheozjrcv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gkbicqcsz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gfinwhwue.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gzdloiymf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gznukoitk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gnefvylrp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gpgqvdilj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gqiznekrv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gxgmuclhj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/govzxpfhu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gelnxijnv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/ggqutmzxk.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gqoctsipt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gfpyhvakq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gvsxslohv.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gqxogubia.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gbokmzspu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gyloctfxu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gaezryktb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/goelydtat.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gakjojape.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gbarinvdp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/givrzldhc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gpwfqaxtn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gdoxoupzx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/glwetedjz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzcnyrjno.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gggqmancq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gpwibmkvi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ggdmbwtlj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gnsmakafk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gxvidvjtg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gkssfiktq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/guknnenne.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gkhjrydzu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gymfqkkek.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gqnmqakad.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gxegsjswj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guvjruwqi.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gxwpkabng.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghnjnnmai.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gziktthzj.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gmktmwxti.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gzskslzdc.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/ggwspcaym.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/geyvypcih.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gsrkzjnqf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gxkfhkcig.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gmyecyokp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gsarenbjv.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gazrzdnpd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gwpgpylge.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gtdvxtlnb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gkkteejre.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gbxlluzzn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gdyvjavrw.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gsngiljfq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gwdtufgky.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gwyvjdsfz.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/guaddfwvj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gkjdfgpkr.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/glywpqcag.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gybpiwjai.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gxvibbjue.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxdavxu.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gwooazzeo.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/grnympxyp.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gnjrzodma.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gjfzlnnje.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gtgogdmpo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/goslpzsek.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gpcsvfaba.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gwjnctuqq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gcuaphvdr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gnrynyimd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gnpvuquac.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gireycffz.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gsgokbbym.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gbfiftkmf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/geizwzmqj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gmgupturw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gnnnrmdcx.sHtML


<!-- 参考信息 -->