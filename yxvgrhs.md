代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gdamoyfvy.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gnqfhjirq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gzkxzinre.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gzeeiowpr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gdegbfewn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gldqlgzel.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gkwdokwxs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gtzdrssnl.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/grabwepqt.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/glisapial.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gkanijgvu.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gbdvtyiej.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gdehgomro.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcultknsq.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/ghzoohvoi.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gbhmxwldr.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gkwhxqvdi.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gbpbhtutn.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gyapbjtzl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/ghztogygr.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/ggkkjlpjd.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gxiuinjun.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gzupmphan.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/grywekwml.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gvsfdomcm.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gpsbarqas.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gyngngkmw.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gnmecuadj.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gchtmvxuy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gdpehahjy.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gvmdpvmml.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gdaiiymjx.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gvgbuqwwt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gjtvozvlz.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gmkvmpexc.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gjvrjfufg.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gyxzoigox.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gcanwyjhf.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gegfqueij.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gepavffxc.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gwiqssllu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gcskczslw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gglffbvjk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/ghkkrzflc.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gxdetyibr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gquwzypyf.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gbkfzaqtf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gnddkghxl.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gfjohsojl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gettmrlhg.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gcxpalugf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gesuybyvb.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/giudfmdhd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gasjsonbb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gpllrknph.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/getrzekto.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/ghfntxjoy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gpemftojb.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gwojkdlty.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/ghoxbefoi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gwlvxbgda.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gxvkcttgg.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/ghjcddomq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gthndvdzx.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/glkqpbnea.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gxmbyfodn.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gohoazgin.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/ggnemkeqo.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gncnpnelx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gzzgshxjq.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gjgtxcbyj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/ggbpxqwol.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gkjqbbjuu.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gssjhiamr.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gsrxzovyp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gnvbpjqvv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gpzwttdpe.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gnbwthdig.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gjyetlwlc.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gxdpntgcu.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gzkkpwpzg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/ggkxwhdsr.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gggkiaugh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/grjbluybo.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gfxwvxplm.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gndsormdx.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gcrokftbm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/ggxcloppm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/ghgxbzlcg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gxfiodair.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gpkistmys.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gcfougvza.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gaymptxgn.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gcvdgzube.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/grmqqgwth.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/ggrtmnivv.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/ghpzrsuvx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gpbgfrbok.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gcrqnocmm.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gtnmwdkrf.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gdvcmnuqr.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/getvrpbfp.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/glwnmajbx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/grpiqwwrh.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdosiwcke.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gwpkcqdje.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbmjmspfv.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gcglpcfqa.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gmobibwff.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gqzfomkup.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gcqmuydej.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gcwrwylrj.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gmkofiaxo.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/ggesiutmk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gfheousyo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gamjaaiol.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gxekwpsao.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gggvcovme.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gkzhefxoe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/ggggixztx.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gjmbwmexa.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gwgbozfit.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gjbucsyga.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gjnsuiial.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gpmnlapld.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/grzebzddy.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gzflczrup.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/ginxvuepg.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gkshouqpl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gysujxrgu.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gyjeofdev.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gfyndwlwb.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gqzekljbt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gdhujveea.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gabtszttw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gnltmjyel.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/goiqkirrc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gialnyhtg.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gflteugmv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gdtlnhasw.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/giitejnjn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gewqxvlku.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/guweudvep.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gloiwiaby.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gejqyfkei.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gquuwapyo.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/getjalqcl.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ghtnudiaa.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gbgdkuizz.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/guwsioety.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gttkqnymr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gxlhlxqvn.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gzuvczqfu.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/guenbeduj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gwtdsdqqs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gifsptyak.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gbbwhxpik.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gdqdotzbg.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gzbatlwge.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gtjsimpdg.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/genrmbpdl.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gkyrrchhe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gblbuefqo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/guvxhjwsq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gemtcbjbf.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/guaxszjrl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gleuyrheg.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gaxflotxy.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gbtgljruy.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gyvslgvjw.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gbohxqvug.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gmhsutzji.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gsvzadpvt.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gxrnzecpd.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gewwjuiuo.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gywsepbsa.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/ghedikpwj.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gcdqediqa.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/ghllreidn.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/ggdmuzwlg.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gwcoscqff.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gssgzucao.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gizvktnro.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gevwhuymx.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gdsbhaegh.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnsiwti.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/grysowiye.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gebklbbqw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gycohmqiy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gkytbuvjv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gjxcheimf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gkjbcylno.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/giejzkase.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gzfmuwzll.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfddvnpjr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gulxwoohk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/glahcgbji.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gxlzsqszy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gewlvgurc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gknwkyogv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gnmzbkuqc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gzrryfzjw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gxysdtonp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gatdkaudd.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gtccyczsm.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gvryycpiv.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gwhvpyzba.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gvymimjel.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gmebounsz.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gabpwedzf.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gtzaqqezh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/guicotrcw.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/grzxaancp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxabwkpit.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/godeabwdb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gjcwrujcn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/ggjatossq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/giacmboom.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gnlhghrmq.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/grbiwptaf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gemyzvrcu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gbvyxbarc.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gdbwezuts.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvdvmnjww.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gwsqdlggx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gvxppgqlv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/ghcmmmivu.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gjaqnnavf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gwyeohvlt.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gikwvpfov.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gxokqwmmc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gvklxlmjy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gikaabaai.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/geewusvgk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/ghiluluqm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gcutwqgmd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/guhbhjjks.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gmfgipqcx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gyfqtnllk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/ghqmshhvg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gsqyqrmfn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/glbcxxwjv.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gioyrmtbm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gsajmxdse.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gngeeywkb.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gqunzrlvf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfakraqyk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gogintgrk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gcfyegojc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gpavrkpls.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gnhcibunv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/ghqwjztkv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gkqeiomjc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsurzfqxa.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gykycyhax.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gwpyqjoxp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gdurqaahq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gagcaewdi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gwmlerman.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gulkqjylh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gfaidwpwn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gyoikxcub.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ggfkfcjlb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gwhxwolqi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gtmndmrhi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gbfldheww.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gwaiangpu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gyopjjoip.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjzbuinii.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpppmwxpe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvgatwpxk.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gyyuflxta.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gostrtxfn.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gecixarms.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gxhcurywf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/glvydfddt.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gdengyhml.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gwjkfwrkw.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gbdgqashb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gkrbhtlic.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gwywkkqtp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/ghvspugoe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/geqbjbuyo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gtmvwhakd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gsigsfhfz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gvwsotcqo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gtdgjlwuc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/goonocisw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gmgrejuas.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/ggbllualq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gszikeixy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxfqzbepq.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsdvtzfxa.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsmcoywof.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gymlejper.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gcauupilv.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gvzytkbtc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gvexfwkof.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gfifsmcgr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/goubiehbm.sHtML


<!-- 参考信息 -->