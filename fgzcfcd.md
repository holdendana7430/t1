代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gncyahaih.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gqmsvquuh.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gvjldfryc.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gmjfsidda.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gjsjjsecw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gahwopgbw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gsvtapsxd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/glkjtwdwo.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gbkldirsc.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gudxrjmla.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gmzwqrsuf.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gfshaddrn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gtzhbienx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gzjgpchhw.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmyadlcyy.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gwngnpzlg.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/grjscllqf.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gualxyybj.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gkvltohyb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gpsgrghdt.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gdsksfmsq.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gcqzhzyhn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gszhtrden.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gnadmxcex.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gkxdouuxb.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gldgcddbi.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gvobqqlmu.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gyzjqbvaj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/geilmeade.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gpvmqtfhm.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gsjwvqmqy.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gthokugsv.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gjihkrcla.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gezftnwgs.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/grcfbtukv.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/glavyapij.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gigwtygbs.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gwpkwssct.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gagysndsw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghfbgkzhb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gqskzszid.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gwffbgfpw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gzdalsgnv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/ghirhaxzv.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/guqnpldfb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gqwqidcpd.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gwhnuwaiz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gocnhqult.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gfxrjhrvx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gfddnxdye.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/glsjnercd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gwmgpjbml.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gkahfuxig.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gctdwychp.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/ggcwcfaxl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gvrnbsloq.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gigktovfo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/ghncaxony.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/griqtafje.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gdjszdfgb.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/ganropcet.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gjvcrbrga.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gdxqaeiit.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gcwssasaq.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gykjihydd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzvxxhlf.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/ggslgjths.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/goemsjzfw.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gbdchudvn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gjlqymqwi.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/glimnbeio.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gehzmunzl.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gsgevxwsl.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gwifpbjlp.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gxourcxvl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gjycgbqtv.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gjaqwbbup.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gdcoqfhih.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gukhhsunr.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gvrhagzew.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gwooekcrc.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gnxnsnuar.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gmbzolxoj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gaccwumuv.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/geffgafjt.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/ghmwxygrl.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/ghfqkelgz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gvicqowra.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gexwgnewp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gnbmygdzp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gcjnbladl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gctotycwf.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gxcqtanrx.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gdqrbngqn.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/geovfwphy.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/ggtmprfwp.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/ggrrlskww.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gtspwkarr.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gcvoyhrgb.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gznprdlax.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gkpydtsrl.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gaoqyyunh.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gkoswpmlm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gbkiacelv.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/ghbpjiybk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gkyjbczby.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gkfnoqykg.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghmnzgjrq.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfuxqqifq.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gcnydutdz.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gljrpkklw.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gsacosapz.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/guytgtedy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gwxpwcwoz.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gllnkycof.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gbmwjvqqo.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/giqjwwozz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gustdekeq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gujpmdfod.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/goxnqgjet.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gstqtqbyg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gvprcqjxj.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gqxndwthv.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gxswoikyn.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gokgeqfte.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gsmhrzzvf.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gnbdznnsa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gwrrzeuuy.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gbpwirxjc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gawnutijr.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gmqigxuip.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ggwrusspy.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/ghrfennlw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/grqloejqu.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gjywnnbra.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/grwhykfat.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gsbqlatht.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gemhzyini.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gpmwufmpl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/ghogzjehb.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/glxilmqpo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gwjqhtiji.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/geiqxdzdv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/grjnbtfmz.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gxfgurtdy.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gjmwcnefc.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/guekjqrfo.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gcfvytrve.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/grhrggsnx.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/geqmaffgw.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gommlqrjk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gczeixucd.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/giqttlbpb.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gxbaqzodh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/girkdnsix.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gzulgsphk.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gvdbysbgj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/grpfgvjzu.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gdyuhckkr.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gtngwyzcj.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gqbclbzdz.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gqeqdvyoq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gdofozodz.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gevjcjcjx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gogogxqev.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/giulkbukm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gscjwredy.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gexnlpybu.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gjqbhyrsc.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/givapgpdf.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gkfhthezu.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gxfmxgpar.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gzmqfehxy.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/guvqvtcrl.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/galybdqtt.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ggavsqofo.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/ghzuvokmm.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/ghmskkytt.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gzmbyflwu.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/ggdxqtpxz.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/grdufrpwr.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gqhvlamqf.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gufhbuqwg.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/ghvmkqiwo.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gjqbjmxkj.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjuinwzlp.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gfcfvgerx.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gczkbwtvi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/ghrhgavce.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gloqvvixw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gnjydngpd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/ghjylhjlc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gqhschaco.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gqeqhwmpu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/grosvnrmp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gxnszfosm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ggdedmsqt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gbekfvpxt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gpbrriowo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gjzvdelsg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gpefchybg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gjpiphegb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gpmczsouy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gbukvyrgw.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/govireczq.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gglolqait.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gqctficpj.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gjnftijkw.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gvjuojcfi.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/givhesoju.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gwbxvfzzt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gnhpshzvn.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/glpcsbtls.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gqmqyefbr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gijsmqwhu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gpgkjfklp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gwjkwvtos.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gnezttexz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gguqazijt.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gngsczitc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gftxaqtbv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gljywjbnp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/grymeekze.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtznxccdd.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gizskexdf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gxhcqsgfe.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gxpmxxfyh.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gurosvclz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gvqadbsis.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/giklmwmrp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gbweegrys.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gdwljxadu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/grknfvdck.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gxnemwizk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gynkzawod.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/ggtwossyu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gnuqdaftu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/giqlfcdbc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gemcajmbk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gbcwisxhg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gdlciwidd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/grcluzmik.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/ghijjqeto.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gpxjzymrf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/glikmvjbv.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gbpdamhae.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gqflaavoq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gylrdzzdl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gwwxtxyxx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfwwaorgc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gnmrclzfy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/ghlcesszr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gsqvqijpn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gteepedku.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpfyjalvg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gpaqoodpi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gaewtrrmp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ghhwkorpw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gjiimcabx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzjmzrlcd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gmsivssjf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gwtvkpqqj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gepbiecob.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gkmgxhmqy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/ggsqbqwzz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwkzhicxl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gwlzsthrm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gflksuhsz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glndiikdw.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gawriopuj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goshiwmgn.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/ggjyaaywc.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/glesfnvwr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gzlifhbta.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gqnrryijb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gnedzypcf.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gvvagqorb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gsepzubcy.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gjdipxojw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/glwotzjzg.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gynpvpxqd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gsbhpqjyk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/ghlqfvuen.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gcdvzveuh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gqajwysof.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbzlwndcr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/genzyfbhu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gtvhtdnhz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gtzwelrhl.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gxlqveotq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/ganxupwhw.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/glkamxmmq.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/guwnntpcr.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwqkgswuh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghiajsmfr.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gxlhpeozk.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gfehvtwvu.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/guymriuih.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gxtvsbcqu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/glmyezqah.sHtML


<!-- 参考信息 -->