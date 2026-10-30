代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gxrcuwpek.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gaowxmvpp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/ghogywero.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gsyexukkm.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gsynnrlzr.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gztyzkyxo.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gpajjtkmh.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gswdlhujg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gryrlcqxj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/godsvldex.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gexdyldaa.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gnfvrjdmd.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gemguooyw.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/ghmgwmxis.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glnsfcrql.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garpkievr.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gehudtiar.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/ghvcmqrfb.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqsbmda.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsozbqvmt.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsgmzoqu.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gefphskuh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsyleswh.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/godajzjwt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmanzaqk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewqenrno.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/ghziryzqg.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/ghczczzyk.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gogkeeatd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gpqlxsjad.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gyudwvvma.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesxwqzhm.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gqavumzqr.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gllrgmspx.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gprjxhcph.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsksomjpd.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gcplgbwxp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/grpcyyyym.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcmiekqs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gclazumuk.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfibejnb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhtvbxdq.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeynqzqg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcqpprtu.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gconmblzq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhlkohjj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gugukchmo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwvrkzbf.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbinargb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grkyvfhwm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpzndlgu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvcsafsf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyzykzfo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gqgrtstxx.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfmlfekq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnajrwgn.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxgoseru.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gefhhkesf.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/guxehuxyq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/ghjmgcbno.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxkimxgq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzuobola.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnzqxlsj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/glidwiasa.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgkzdlpq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/grycbnvzn.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gadqzqhih.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaexrpfn.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gnblictls.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gfnkbwqla.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gozgikyaf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdzwyllu.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzvnxipb.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuabfzuy.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjcajjac.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gympismam.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gntkjvdbv.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gowhuknsm.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gryvjiqnr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcxlewrx.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzubxdeaw.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gokavxyvr.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gzcvxuraj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwldigneu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwywsfii.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggziqrrrn.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gwggnvqip.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/garlltott.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gascjlgnx.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/ghuihutoa.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvxqaano.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gctakybah.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gioybgwav.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopnkafzi.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrvhahuo.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmwiezjn.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/glbjvfvpe.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gybbivyfj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grggueiow.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gehkzxbpa.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwruacnow.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyupscjo.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzedsmwyn.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/glifxklge.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwglliizn.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywgomrgo.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gntjgnhjc.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugzynmub.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsqrsszx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtguuiwx.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/goamublro.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpejdxxeu.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulwwkmzw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/ggtchfnva.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gelllcyuc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzsmbwyh.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gjtvbwoaa.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gsamuuiva.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/grlqyjgcd.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gydezdcvq.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gkijegukx.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvybrtti.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuvzllgf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/geyptjmwa.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwnpekki.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gslschtjq.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpjmamhb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyvuurnb.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwsaqggk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gblppmsim.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gevfyvaom.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gnscopvhv.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiyztnsn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbfexnzg.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoycuptf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/geilchytv.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gtbsvpsay.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gnllqkkxe.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggivhvgvw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/geyblvhao.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/goeedhkpl.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbiiqvpp.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/giknxcoly.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlaxgyhg.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gscpcaacw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpqgfour.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdglzcfbo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gephxundh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvgvwwfe.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gweaacajo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gxhgyamgh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsegrwth.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqxaxpmd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahqfzuvm.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpvmmqnb.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxavnbby.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gcwfkzmhp.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmulmxhdx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfeoehoi.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gfdbfgfzw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwunnbro.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwfgevxm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwulctvjr.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/giwflijry.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gtywfzfki.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyhotqmh.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/grwcpyswx.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gbedbelbn.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gqeliuunw.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjncteua.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gtogvuiny.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqfxvbiz.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gomnebnze.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/giubvlhpe.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbrsvlhp.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwhxramr.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gmpmzhegh.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gslnslram.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/ghgmnsztw.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gykntdhzj.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gjjdqazid.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gjphnbact.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/grsfkvysy.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/ggwdlprnv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxepdvwex.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gsfdballq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gedwdbmlc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gxzwecgoo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gwoxeltsh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbomcfwm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbkijemp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqyklivi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcggtlhk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gjxiulpnv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/grqrmniuj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwqylekn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gmmrcccyy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijmsojxd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkcuwqcn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/glnnuoaxa.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gnpqeojac.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gdtgjwuol.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/guxifvpum.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/guqmbxzpg.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gpscpjpiv.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnklshgx.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gxapwleow.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeqqtfro.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfdkzhzt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gmmtinipy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gpapsfwwf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gkedbkjcc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gfjbwotbb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnnzvxmo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/griazfiup.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/ggdwhtqve.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkooyuqwp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpddkntfo.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gvssekyws.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwcvaiqq.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjelakkg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfegkgodq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/ggrlvgece.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gsoxgxnqm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/grcnjpojg.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzdgnltn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/glatmufpj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhvdiwyf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqxydohc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gsmlxfccd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcyrfxnl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqucmakkd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/gqqybktkb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqjrmyze.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/geqvdccuy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/golmjisvg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gqggkbjyw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnecqxpmp.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/guzncajne.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gixovprkt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjpyibwqs.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvfuqtqy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gltipyuyo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywocufci.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gijtjuruz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhuncjvn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gatmumydo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gocwxfzzy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmjiwdez.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwfylktt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqrajzos.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsetbhfzb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grsrlryec.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaczeydc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopvkmehn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/grajkvtbi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpejqehcc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkighinwm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnxtopub.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkfyxouib.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guwdsymvo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheuqspkc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmkcakvy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdpjmmuau.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkmfdlxv.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gogyxadoa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/garkunohe.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzxyzjjn.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzsezhun.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvczxfsa.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gbgmxrbor.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrgnhvsk.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gcluihpbg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gviuqstmq.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gijohqmhe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjjclutp.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fanxiaobao.xyz/Article/details/gljaplfyt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmsumitp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/ghaybavit.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltdjxjgo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkxfxczw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gmdwvuppd.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjbbykjw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwhkvdfr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gqmxqrjry.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnipnexx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/gydlupbkj.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/grjfllxuz.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/goayuibcy.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gbzbomdxx.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gmblxrhxd.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkbfxeui.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gquqyuzsb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieefzolt.sHtML

[A04] 判断变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsnpjjts.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gpbgsenio.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gswaobwgw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gxclrvrgq.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdbacjyi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuujmvzt.sHtML


<!-- 参考信息 -->