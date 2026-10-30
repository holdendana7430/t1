代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gejijrjtu.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvjfqojp.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkqpmriw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywyfjzcg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghsyfbgx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gywkolgcp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gnijkrjqs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsryuquav.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gjpwgvguf.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkwxfzxy.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gaglslbbv.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gmukfzrgi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/guzkqofka.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvmgoeuhw.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gpnlmefkk.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdtocdmm.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/giszgiimw.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/ggmseuvtq.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gfngfkhgv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gucmvhyou.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gwyvzwola.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/ghmsqoqga.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/garcjsjnn.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtvlzljs.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gzobcldgv.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzyagqnh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgtecqzv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvffchdt.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/goygljfwy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/glsjdwpfx.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gmeluquir.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfecnxalt.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gazspnoug.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gwfutmoqz.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gtesgpyci.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghalhfair.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gacowzjca.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gordvyvlp.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/godwhqlws.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfyxiqcy.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gignxjuvy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhlnylad.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqpffsrd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqnwsgs.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gyunntetq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszravlnd.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcmpvcem.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcyzxvps.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvlezcxk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjztsoiug.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkdyuglt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gliwnmgob.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusevoahd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsxwonzgl.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gvjfcsxff.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gymkautxh.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gnfabzrxj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gknqznklk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/glchpkuzl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gtpmgszxz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfevgzwv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gaoadibbt.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjdboiji.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqjcwhmn.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcuijsff.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhiurpzg.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/grqjnkcjw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaukrykzu.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gsudxpqow.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyhshrru.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gybggaepm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gsdasvkpv.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gvpdzriif.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/guuqwcmia.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/guaoyrzzi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaqggnub.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gyphawzte.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gwhnegwbd.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnkpxhmo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyviatef.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gikzufbrb.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/glnefzgwf.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/ggznweuax.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmsyjjut.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhwqvqzg.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gxnriqmhd.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gkdhnnzor.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggairpztt.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfddcdt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gkonkkhcr.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gvphcgjay.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkwczodl.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxjzubno.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gkqlrpxym.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqqmjofk.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzldlcnrx.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghznwcmvl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhmrokeb.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gufdkwudn.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/glsrtbeqc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getwdpvhn.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gocdnvxzg.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gapcfqmpq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrtadfit.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkxjevbja.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewunwznd.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gcknjchmo.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gkpchoahi.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhmnjsou.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqzlqgip.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzusvqqnv.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/glpygrfpm.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gckkxpiqg.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gbwxikmrw.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbyyeake.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqkmmwvz.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsqyqvgc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/grpdziiyt.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/grsidbtyg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbehdmqsj.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gibcismon.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gpmyjsfjf.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gvhaahhoj.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvliwfthx.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpboiiptq.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gggeyhuro.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gfphhxbak.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gylyyhtzp.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbvmtczo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfrthvss.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiufarju.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsydivoer.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gxvfbvhut.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gdyvmzfrs.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ginidalmt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibtzupfy.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkofuyip.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gguemqqrf.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbypoetvl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjjlhmaf.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gbosssycs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskfzxwfd.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjupffhy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/ggaxtiiop.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxfqqhvh.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gypvdrxia.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwyfqfis.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjuxhcws.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwsvybtr.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjovqsrc.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdhkogi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlhkkebk.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/guhgitszh.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/ggaeuycdd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gzoxhwpqm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ginigolbs.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimirawhw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnhthmmj.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gqlrjftaj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumwkzraa.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gwqvcuafx.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfxjflhv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvubqikoq.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/giezezfpz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcpmedxtu.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gxiublqoh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzednhqa.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gojhmnzgb.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwiaexxf.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjddhzunb.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gmvrpaodh.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwasomler.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksqymrvx.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gkznzitgw.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gidhvyffb.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gettqonov.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpgmophf.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/goxavwbhm.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gyomyluuc.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujovwpvl.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givhqjqie.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/grdoxerbk.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gmivrmbwo.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggosggmym.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gnqqpaoux.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyccinra.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/glmioxxkz.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuksfxni.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/ghmaaqndg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gpqsiyvvj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbgllwwm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqnasyvf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gmhnxcoym.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfypwjhj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobrekgny.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gbapdzlef.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gorhkigse.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/guovlkflp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwdhhnur.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmyzfszc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimfdxllg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/glfybymwr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthouuqid.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/goywmzkxp.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrvovnww.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gcyldefib.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjxkupoo.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqniwcfw.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajntcatf.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuvamyjy.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gyassvzhm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gkjxveqmt.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjlnjott.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gddfdvevi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gnylhplob.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvhqjryl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvlqptyf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gbacjmheu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoaqjywk.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmwlisda.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gozlvczac.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfpksftn.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzqeysbl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcominrga.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdwzjruh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrwbvcka.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbjgghxn.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gopiuemfd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gwotdujpl.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhximzbi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzelzgkf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflqmsarx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gchhnrnqw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gthilghzu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfpnvfcr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/glnilbrsc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gehkncych.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyxrtxmv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyzqgilp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gjyxwemfl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gjczochbe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/giejtdxtg.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gqiscakyx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gottzooae.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gopizzzvy.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gmujchrnd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurmbzasj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gaevefwhz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gfoctgomy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gknqgcztm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbwmwmfmb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glwhmlrmi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ganntysmy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdekuihp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwoapixil.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/glzhdvgqk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghokrvuqm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvpdmjyg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrkvabfh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxglkdbpd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxbzazmh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwhwsskr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljdpnugo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpeahkjfx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gisywqdku.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghdssnunm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/glglrgzry.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizilrash.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geikhepyn.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwxtsbjso.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgbcmwxj.sHtML

[A01] Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnidnawxw.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeeaihmp.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/gfcgysepj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggutohrkk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwahxltjx.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmobbqjr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneoyzvfs.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczlwfpiy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/geaoggxcj.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/geboxuhdb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fanxiaobao.xyz/Article/details/gbnyecuuu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsaraqhh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvlgursy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gnccsyocb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiyroocx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gbebcygdu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gfhasehtl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gljqytpyu.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gpflpkgwb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/guuuyvogq.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gxhdfyfca.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gflxvlzoj.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjiqmgop.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdilalggc.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gpsfnbfkf.sHtML

Ruby: PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gkwkhxhxr.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/geafimwqz.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqoshjvk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcswjuhz.sHtML


<!-- 参考信息 -->