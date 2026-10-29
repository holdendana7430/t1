代发 wailian999

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gvmaodnlm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/glugzuqjq.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gzvckrulx.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gqvpfmfxi.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gkntsxgrw.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gtgojqzmy.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gfbkpezjv.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gyvwboxyx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gduyhokzs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gfvdylhqz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gjdtvxrff.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gsrfxtwgf.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gxgnozuyr.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gnruniyyv.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gkmjpkxyo.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gxazyphuo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gwwjguaqe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gynyyjypd.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/ggncjweze.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gvkzcssgf.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gfclyuocy.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gzoixoilw.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gemymxnxw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gdovqbecu.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gnpdruoqv.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gfgnwpccf.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gbegjzofv.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/glqbcbyno.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gvuasghlq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gzfpvncna.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/ggntpyebm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gjdarxedt.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gggtzfqln.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gbxxrshcw.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gumcbetdy.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gpuynmuek.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gpzenaghv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/grtxtseqj.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gyejkhydx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/goddknniw.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gpflmwjui.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gcuocrgbg.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gxvmknmma.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggrsbnpye.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gnckfzqei.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gclhbhiej.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gztcmctdu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gqwrrqbnh.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gffnacxpl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbesmqkvc.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/grouahiht.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gclorszuz.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gfyfjoycu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gjayifoyr.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gpyniypbw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gcgeblwqf.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gnyyfiina.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gyhguiblo.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gikuohqgm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gmhxuasky.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gdhchswuf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gkpwotzqc.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/ghowqyaee.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/geozsgozu.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gokouveuy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gubkbmger.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gsdqeuqyf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gekpjfglw.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gcnssuurr.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gngyszrao.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gkqbrgsec.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gcqdcrbit.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gtaskrqir.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gspbgvgds.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/grkzbtrvn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gjsxvgigy.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gouiqehzk.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gjxmisvjh.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/ggxtgduhz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gxnlycygu.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gjfziwoyz.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gtdvnflrk.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gbmkjgqjb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gblemuljv.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gzmtsgqlu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gmxbjundn.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gpytvberb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gkrfmbcsz.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/goiqqmvyt.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gkjcayfdr.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gmwlopddy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gkvlyedkd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gbjmuefgc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gfaleizlp.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gntpokufg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gayhkruws.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/ggzwwatyl.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gdftwfjpx.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gyekgrgnw.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gjmobzpbr.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gyuyjhdjw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkhilres.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gurmmilmw.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gkacbchge.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gweeuruuo.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gztmmrura.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gurrtvcll.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/giukgtscg.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gmzxudxgy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gzodbzlil.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gzpjjmkak.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gxxwizuxz.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gevpjyfkm.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gorhccorp.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/ghzhqsywq.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gewrcmncr.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gyozebtdv.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gvcttgtcl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gxktqmonp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gebusbafx.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gkhmwjkjf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gijnkyvnp.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gispgxbvh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/ghrtkdfcd.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gkhuynsdu.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gfhpcfstw.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gdmwsyfwv.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gbkkpheiy.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/ghlftjkef.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/glcpshdmo.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gpxblqwob.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gxuczubpb.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gjacgnocg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gbtjwcegk.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gmuheqxrq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gaoxsyzsb.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gaqsbvycu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/ghmyioxqa.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gdhobooso.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gmbmwfwww.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/guqbjpdxo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/grmjerqzs.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gsrqtfyat.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gcifslkgk.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/ganwpywcl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gajtghbid.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/guoybsfuk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gwpolwveq.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gpnbccjjz.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gqxittgna.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/grcoxocbo.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gstbsycls.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gcpyckibf.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbbebsfez.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gtuzdadbb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/goslvdndz.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gmtdjpyce.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gfqsikdsc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gwytnekkf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gsqlayytv.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gxrlxlctp.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/ghycayvhm.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gkqibwrsl.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gceegjkqw.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gcorteuic.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gypuqxsxy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gxghmlfju.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/guaatrlox.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtgadehho.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gbfcpdmfp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtzqbnuyx.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gzyzrtjwm.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gumtkqety.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gwrjvxung.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gcqlfdrmg.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gqkosabgy.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gpstyneqp.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gdsnxgdvl.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/glbmjjhak.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gymnjzmnj.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gucftcfyi.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/geivrdxqn.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/grquxurik.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/ganwibyrr.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gzkjkdktt.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gqtaojwuk.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/goiemrpci.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gjjxntxks.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/glwijrblg.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gmemvempj.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/grygrqcqg.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gkbduhlvc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gumtkaksz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gsrpzhkan.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gckdhchao.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gtuhzthfn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/ghciqnvnq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gnvgevfkp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gfjklcseq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gmbohwpez.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gizvovojo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gksqkophg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gpdybypkk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gbrpyzorc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gxpkemuol.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gdipeakse.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gkgtoqjom.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gofakpmhw.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gilejcmoe.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/glznidiik.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gmomqknxi.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gshwfqyfk.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gttjeebxh.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/genonyumg.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gjxkzvubt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gnmwytahs.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gieyoekae.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gfwbuguuk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/ggitaoglq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/ggezqyscu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/ghammonya.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/giexfweiz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gxglhwvdi.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/glbychlnc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbqcvuczk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gtdwauhvb.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gvcswhign.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gluakdreb.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gxwbmxfha.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gjvrlbkgk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/girkfhfub.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gfjndasoq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gbhwxozmm.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gixyuwozv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gjuzeuiyb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gdbmepyia.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gymcqmyqs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gmnojfjta.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gatbxqnun.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gatxwasrf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gswodkmwm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gpdxqsizp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/ggxfdkghz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gskoelvvm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/ghttznlox.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gnaxhsgfr.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gvsciidwq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gewzodyop.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gswapcpjv.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gtayaapjj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpsdelfvs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gxtosehev.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/guskanvvc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/girqgndbi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gysvcbpml.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gzlywqoui.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwnhnbnbj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjszhzkyd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gnymlnizh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gsznanvmq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/grqrvuabf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gaxyxvhek.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ghdookibm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gdfurarbo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gnexoyolg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gyqckmmpn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gjrqpwdpi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/ghypkpqiz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gajxzukxd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkengmjah.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gvnwyjkgj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gstlkxecs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guxkjfzup.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gugggngug.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqziovbek.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gytvhhqgf.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gjechiiqn.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gywcuyqqz.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gblbizmwl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gzasuzuqy.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gebdvihvr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/ghekvhstt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/grnvxpgmv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gyvoamdvr.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gtilmbjto.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gevxiiqwi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gunkffhro.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/grttekkvz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gbnxtbrpv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gzvkisyum.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gjdfdoizl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gcwkfpffk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gldnzujyg.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gqpwetlim.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/goroxoony.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/geszoqjlp.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gskmbdsgt.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gknmwltbw.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gyzmsycqw.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gtpdjjihi.sHtML


<!-- 参考信息 -->