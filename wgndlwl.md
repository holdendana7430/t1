代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gvsnfshnu.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gaalslech.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gehuejaya.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gqbmpapaz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gcyscymfr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gychspbdu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gjosgyegq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/geoqktfbw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gtmnafocv.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gzdyonykn.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gmhjzwlhk.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gblyjmgfw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/grzenmoga.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/godiquxpg.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gqufwipdq.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gxhjvezth.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gcgxjfprc.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/ghvrqlmqp.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gntosclmi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gqymemjrq.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gnmugtqdu.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gahxeqvqd.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gdzhhbjnz.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gjxtepftq.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gvgmkjmuc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/ginhpatxd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/glkaysgdr.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gndljryjk.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/ggdsfswuq.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gervvjrgu.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gpajguaqr.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gfhpkdups.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gavcuaoxf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gmcwzqoqt.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gyojctbxc.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gfcekfjxy.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcuhqaawa.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gyaynuqmt.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gxcbppmwj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gquuhojfo.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gesgaafza.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gptldmznj.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gsjxufyxq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/galtvjobx.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gbrbgsrzu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gpxtsjhyt.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gqokuutvs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gjqmwxmdn.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gqvrebdno.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gkciacywt.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gxsbntmtz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gmflwsvke.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gkzfqbjyj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtfujhbqk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gpebgytwv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gthpyrzux.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/ghbrueldu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/grddywplu.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gtkgzamqt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/grsjholzk.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gvrtilkfx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/goqzmpxzr.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gfhensieh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gflvlrljz.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/glbptfynn.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gxmuztyly.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gdsyluuwr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/guzamfbao.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gxxzoydue.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gbrockjjr.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gkynyflfy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gsyezvcyf.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/guthnrqut.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/glthogavt.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/guurvfixy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gndfwawin.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gyrapakxn.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gskqdnnoo.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gnqkdpbku.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gsjvmrycf.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gfaozcjab.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gwjkqqhbh.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gzbrhtjbe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gzktbrlmy.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/glfulscjp.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gpkuvrehk.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/guetqauns.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gikdnwipc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/goqhguqdn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gsvigacvw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/ghmaipyqx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gnmqbzuoz.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gsmxnjiaz.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/grylvjobx.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gkuvxwinx.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gscijpdbp.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gylsjvtkc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gsmswdlac.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gxeqbgqmc.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gykplncqn.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/ghavzhqom.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gyhprxdik.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/guokukxqm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gittetghl.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gifydcwxa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/ghwqwagno.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/giplcrmit.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gdpmboybz.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvppfcmoa.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/ggecaqswj.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/ggnwrhsez.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/giwykmkyq.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gyrrbplbu.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gvsfugwre.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/giykoomyf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gwgpibolg.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gvqwvcfol.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gxppmwuqe.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gyciqasoi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gyiugjbqk.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/goggvtdnl.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gezipljha.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gcanxahlq.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gepbpbfdy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gcmqyswfi.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gcfgnqhpk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/glkgsvdpd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/ghaincdho.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gpqinspzu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/geddywvgd.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gybtycbhv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gdcrpmlel.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/grbrezzfp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gktvwpdqz.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gwjedesgl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gexvowkki.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/ggnymrhde.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gafqkvalg.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gaaiwobib.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gcymlkmcy.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gfeddfgpx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gbmgzsndw.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gloqczier.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gnvqymbfz.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gdbimfksm.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gykfcbvoi.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gifzljgsr.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzqkzegsa.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gwscwbgnp.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvrinikqr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gcgylmzdu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gzonzplwz.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gnoevjgtb.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gohrmmbin.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/grdxevzap.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gzzegcret.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gahliythv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gprmaaupf.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gkvnbcnvx.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gbbffofce.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gmfqifead.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gvpwrbkqf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gnwfmxkak.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gzptyfvir.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggcvkmaph.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gzfwshpkc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glryhcrej.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gubcfajaj.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gjiqlwxvq.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gzbemxydr.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gvqqgxetf.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gxcsawllt.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gfnbcfmjk.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gdxqtbire.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/genjbjttu.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gygiyaciw.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gvkehhiya.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/ghbuyxire.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gfvqhlaiu.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/ggghphedf.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gzftpvmdp.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gezsdihho.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gbutigmmy.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/ggcgsrkmh.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gbpcltomq.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gnyuyajrj.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gfqsvlmlj.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gyaztbaeb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gbbsdnzwc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gespbmzae.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gtswbpbzi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gztkygytd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gboeppkdp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gzmqdkwjl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gvznyprmo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gqcqwtuan.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjdsrepss.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/grhjjyiic.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gqfegyyxc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gakkqnqwb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/ggkelmdtd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gmcjrbesz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/ghtuumoic.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gsnlogpwx.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gbvfvykmi.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gqvgjrbau.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gjdmazwnc.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gzwexkenr.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/girspyalz.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gdeuwsvpn.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gbtbayest.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ggbbemvuh.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gopfllpkq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdqkmbatd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/guesabctc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/grbttbydr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/giezjhpbz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gqcvjxyhs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/giiphmpxl.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/ghsjpnfdh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/garbfqitu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gvmniuxza.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gphdiqdbt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gosvgrbep.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gbgzppzlg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gazxahngj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gatipgbsr.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/ghxxflzeu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gfbusduwk.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gqlqtihgb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gwivbsnsq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gdugeawrx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gjdphkong.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/glwiscibc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/ghzibsayx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gjldagykl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gnmvytqcl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gxdkvibho.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gnwatrqqy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gkrqmezue.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gymsjcwqx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gksgwznkl.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gybxxhcob.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gxyxwecyv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gldfyhlor.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gkjfbcbbi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gsynxqser.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gmwqssfci.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gobgtkoek.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gblrfjjpn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpzndwcts.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/ghzpygccb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gvgkrjfbp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdtinwdnu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gdttmphkl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gwunrgdrk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gbgcqxaxa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gcdxsbijt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/ghywljsdz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gheyapqsy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gypmyobwa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/ggugmllvk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gabfqebyp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/ganbbsirn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gkpmiyzhb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/grjkhqwpp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gfopgqvxd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/grodbhgwb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gztfwzygc.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gslmvjriu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmwsipita.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvmcjsmch.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gtiwyfxfy.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/ghwyryqyq.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gprzmtxli.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/ghcxevjjn.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gaammqnzx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gmmjuqosd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gtkmxmiyh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gvwjmjxby.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gobgbumlp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gkgtlofjw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gcksbpyfg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/glwfwnvxe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gwvhsbpry.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gwjzyzjoq.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/glbnosvmt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gxxbyfmew.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/ggvzanjxo.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/ggmoadpfn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gdnjkpljy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gmireyqiu.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gsbbkwlvn.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnhjliugd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcwgkmawb.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gfvgzdhpg.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gijiayjuj.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gswmymjnx.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/grzhkglhn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/glhwekobn.sHtML


<!-- 参考信息 -->