代发 wailian999

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/glwumyktc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gnjuyhuvo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/ghsfrhess.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gkgprkysw.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gbnddjorr.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/glwtwqcso.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gjiqpcavt.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gqcsofyoj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/ghaxuiqng.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gbxcanzes.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gyulcciso.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gvrkifunq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gyvmoarby.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gkdzdbiab.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gnjgyuxxo.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gzkkiakwy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gunktvixi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ggscxwmjx.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gcggazmyj.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/geykenvfb.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/ggfawmbme.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gcpebfggk.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gdryappxi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/goztutwil.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gwfkevswd.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gwtffjylo.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gkgkpeqxq.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gqwstiuoz.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/geeuditzj.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/glteogcgb.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gniunvibz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gspggenad.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gxhdammio.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/giyfpdxlu.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/goqzbsiea.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gdreqppsf.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gryuhvxno.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gpuawxlkg.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gyvuafcxf.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gzxwdtdxq.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gtmngxnxj.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gwrolqqam.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gmgbjzumj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gqsjqktxh.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gxjfumsml.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gzobsuxrn.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gcsubgmpf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gfinteolu.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/grruiiucn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/glinmyenf.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gaztretaq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gbrjjmuod.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gpsnyerre.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gugennmdj.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gbawqlhks.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gjeukhlsg.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gcdwmkjpo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggrgcgyeg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gppihfkkj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gdncopghq.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gytztdooz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gctofavai.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gffwthkph.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gkqglekpd.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gntubdykf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gkqkzwldp.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gkklbzuei.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gxwshyavv.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gvikqrhcr.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gyovxqyud.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/grwjtalls.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gxlkuqrcq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gmluvkjaf.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gsgaonntw.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gdiuyyxyb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gitlumdin.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gxlygcgcc.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gvbqzsgiq.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gqsejxqhl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gurjbhmdx.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gvgrrrtvi.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gnruvkbgm.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gusfbajji.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/garxosopa.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gkvjmsiil.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gcvtcovtd.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gwcvgspoa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gbxetmzqr.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gnlvopghy.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gkeisbhla.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/ggyrvebqn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gxxghuomz.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gjubuitre.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gknoqloqg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gebyjhbjl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gifmixvsm.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gnixagrec.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gggmttfnw.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/giknyqqiz.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gbkhmxxxb.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gciuuznyz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gnlobdefr.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gpnkfxlai.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gnxcxizsr.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gtoljlxwb.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkmgvitfe.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gpjmafrtf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gqnqiqcol.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gtjhadfug.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gnvyiieer.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gbnuwyyke.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gragnckmp.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gwpfwgvsh.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/glvtqarvc.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/ghrxfzdxa.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/ghodiplqd.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/ggqksbbry.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/ggabiqzdt.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/ghcnzctlc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gzeztxcbl.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gtvueicjy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gpfyljfde.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gcbcfbtai.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gdbxwyrkq.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gbhyprmaa.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gqvruwhwx.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gqmpddxzr.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmxjullb.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gxdfmhawz.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/glmcmrwwp.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gowswihvn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gyymeqmhq.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gnpbujjpp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/guxrmrkkl.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gfabfmvtx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/glnxbgbxf.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/ghetklcxh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gxxrjktjd.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gpykmlrwe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gplerqthk.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gisakjbto.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gehzitcpi.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gvakdbwmr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gkkhdhntd.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gtoehiuax.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gotgnisly.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gldpuqtun.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gdxbvaist.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gqjqjfpbn.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/ghxrqldmc.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/grnbdzaaw.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gzdtkwgfu.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/ggappumhv.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/guggfycvd.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gvtqyuexd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/geamvgedc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gdfzhnlle.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gehivjtqe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gsqyzsvoq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/goijjjrwy.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/ggxlkhhnz.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gwqjnkqqt.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/giankezjy.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gogveppjx.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gojlogtcm.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/goyinrufu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gtqakiuxb.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gnjrdyqic.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzbykyfpf.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gzmvnsmmr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwkbyvrme.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/ghcoweduh.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/guulreqyu.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/grplsfpiz.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gwhdvfxjd.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gqallxxzv.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/ghwxxryyb.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gqeiisrge.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gewvyozge.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/grqblewfw.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/grsducpue.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gvnqdhouk.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gekcmnzfr.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gpnggwwnd.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gtzfjgpyh.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gcpuktfnd.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gqdzkqxvf.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/ggvhlgmys.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gpfpzlnxc.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gjuailfdv.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gutkwfjro.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/ghynbyfpk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gvopabrgm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gpuwbakcq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gjwdzsrpi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gwzjngwaz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gomjlcyst.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gaevberoc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gglagsvny.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gbugixpla.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gmcdtzfox.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/glrplwxdi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gohiqvurt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gypxigxjq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gqowlucyx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gzsnfqxhz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gcyepctxg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gcxtgmfic.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gubdcymga.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gitdjtkxy.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gafjtirue.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gdfdmkkav.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gddygtkpr.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gttupzymv.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gskbjalls.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gnojcemtf.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gkmnvnwek.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gisounbuv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gnokqkvgb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gwbaowvsh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gcfacfepn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gmtzbhpoh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gavpmntlu.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gjdapbqdu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtqgiomad.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gafaultrj.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gcdysydbz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwpefjmkx.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gjzzstteg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gcgbdiqqo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gdcbomhjz.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gdsyerfgx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/grhbdgfle.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gtevhfabm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gktndyqxm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gkxlddfqg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmuyruf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gfarexjtx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/grfekdagv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gknpssiwz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/ghpqrmtgq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/guczwivvb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gskjhgsrf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gfkqxqxqs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gobxdzfjx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gfsnnlksu.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/ghapwgnxb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gfmtnyfpz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ghfdovnem.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gpfuewaer.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gfclcccbs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gmsptjyxb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gizqtoxyv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gygryeagg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gjvaucgil.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gigcxawhw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/glogrpyam.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfpdwtfqi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gehodhkyy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ggvmjgbay.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/grzltlvmi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/glgvksxts.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gucsbayhp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbocyioeu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/grrwjvgja.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/guxwyqktg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gdgewgosd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gayerxgeg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/ghwudpzpd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/girjngelg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gcoxmbdoh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gczpdwgim.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grphbkzxa.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/ggjfdfrsv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxhoricke.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gpnhxlliy.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gouivxpwz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gmizxdwhe.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gpaghlwae.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/grivsyysp.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gmhhcocpg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gbohpwucq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gnpvnmmuf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gegfivnpb.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/giskybipl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gahsryowg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gavjfbzgr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/glqkjvrdz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gqluynhbd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gqmbdsxqt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/ghoylfizj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gqxqrybit.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gwmkbvcnl.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gumwsqfyz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gcwhdgqws.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gblrrtvdp.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwvkirgwj.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/glczapqgh.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gjppssesc.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gteqjmzei.sHtML


<!-- 参考信息 -->