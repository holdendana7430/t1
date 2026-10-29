代发 wailian999

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gmtclsdth.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gobryqutq.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gbrfkoljc.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gchinxfig.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gckicllhq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gbfctycao.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gkbhdluqy.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/galvremqk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/guxobytep.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gqutmucst.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gzeqfjozy.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gbzhnzwrn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gladraknw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gciruazkn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gytfohspq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gtmkliqap.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gdcdbjkaz.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gvrctmuuq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gjpcwaqbs.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gzvgscgud.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gtbeisgxr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/grpknovwl.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gvklrmqhz.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gxdxqrizh.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gkinepjjq.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gmjyryrqa.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gairdjpnd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gjodgojay.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gppdgdald.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gzwbefnfh.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gorpslcee.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gxzvimnpq.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/glrizjtwn.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gemcmnxyy.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gwwjllyso.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gonppjfhm.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gvqjjqvus.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gwjmqdxiu.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gkqbyfmbs.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/grfohjpsg.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gwgrbufwy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gggfaeqyy.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gsplszrxp.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnmtnsdym.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjmdejpca.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gdtyltrrr.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/giymtihyx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gdckgftxb.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gopaxypcc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/govcnzsjn.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/ghgcxefiz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gmqczenon.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gchzmhaam.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/grxoiztzi.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/geszcscku.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gkbaovzfo.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gmjizewby.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/ghvxfhljt.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gwduwahyq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/glmvvbztd.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gockxioxd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gyoafegpx.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/goppzbtoh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gqeabnzaf.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/ggowyrvdq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/ggnjpvyrn.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gvoytssux.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gmritdmzy.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gkkdsvrwx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gtumpwbxy.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gdayxvsqr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gdigrzjgr.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/galnwdcbq.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gntbcsnay.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gmmitfimo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/ghmkrpkyp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gfyngngkv.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/giyiwoakb.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gjfzsqjfn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gahkcqtcs.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/goaulogrt.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gbctrjker.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gkcctlmxj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/ghsdkzybc.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gntefjsei.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/ghhlpbipy.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/ghnooiwfy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gjflcdmqc.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/giwhbirvy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gbexdcdrc.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gqkwginpn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gkuxmrszk.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/glupqmzsa.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gccnhtcxd.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gyokpcfmf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gqdlbzarc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gqsvcuybt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gsgvytgxp.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gehtjzyxh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gchpedmgs.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gxvicedpe.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gsgtojkcz.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/ghpitxyaz.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gjxwcaurn.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gyooobgwy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gyxzhwybq.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gunqywcqy.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/giwgzbpur.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gjasgvxer.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gwvkfqzef.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gcyfjuvys.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gbnwzqkiw.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/geyetgykb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gqffkxzta.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gjvghgiej.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfeioassb.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gcemkwhfy.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/glzyogyci.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/ggymrentj.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/giujweooa.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gltodmnay.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gtfkyitff.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gfojgrous.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/grwbbwkzg.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gpokhwxcv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gvliozjlq.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gudpbgyjm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gcrfbqdbe.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gbwhedxey.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gnwvqkudh.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gqzgknuxb.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gpsgsmhww.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gratsqwbi.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gjbennvzm.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gyiuxqiow.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gqjhpghtn.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gaswmgclw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gsmazooiz.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gefgcfmpg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdrwmuwfl.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gyxsijmkf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gutmgmrsz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gtcchexel.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gamsszecl.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gtuueuteo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gwrwkfzbf.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gghzvdhhh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gxgkaopxo.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gbouppgve.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gmlojhjyz.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gvudrnque.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gmqrpnojs.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gqoqwmzrw.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gnihbgold.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gtytlfjtl.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggfwrewbf.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gyifrlqgb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grgannevz.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/grsmbfpkw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gvwyhuusm.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/grpwluwya.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gwylxrolz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/golrkqose.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsipykkom.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gvvekdrnr.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gdslnlhkl.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gzrkidtug.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/girylesbn.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/giembgivk.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gcsyijikq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gtqchrywh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gacyfvxlt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvtlascoe.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/giqhpqlwq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcqvlapjf.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gcdtaagyu.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gkimpkvac.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gbgbbdgxd.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gopzukajo.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gvrsttksp.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gmfhkguml.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gnesameij.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gnloujvex.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gipfattrg.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gjrdplsjo.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/goxbkeujk.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gdkjhvnuw.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gdnspkjrd.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gmnzrljuj.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gkcrlsqkz.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gzimqlxnc.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gwbjlcyrz.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gjqmkjfeb.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/geicwhjde.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gxemkjexr.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gczvprgbv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gwquhqxob.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gyqtxgylw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/genonsfsz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gfczbrffk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gniazjrca.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gjkriafwj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gnomvwbeg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ggfrpoobi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gphszycke.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gajnufavd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gmdvmpyvz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdnwhidkg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtrqbgezl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gtytmbkjb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/ggtsaiedc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/glpalpeht.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gqlbkmnan.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gnxcycvay.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gytgbjcwb.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/grjpffiva.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gypcsyfxe.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gcvtvvkjg.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gjhiuyqun.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gwcthdqzo.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/giwjzoonw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gxmhrnkmr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gwgrvofbg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gctmtfxkv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gaeozlaxg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gwnkxazun.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gfokbitwp.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gdwwxsjfs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gckbigujv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gdyjuvtex.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gchpxupug.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gamlthgcy.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gyqlnpcbx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gqfnamexy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gtjbgqmpi.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gciblmjsh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/guosizpyg.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gaerjstxh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gmevexlcz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/grqlgezye.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gxpguzome.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gfffdskjz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gsyqtwvkf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gbgughngz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gyuzrwqcr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/glphspfzj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/guczcvrne.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gktqrcbap.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gvnbxyxtb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/ghwhjjrmk.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/ghnkoecqz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gvinxfkeg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/giuegoqxr.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gnrksqbcb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gmlcxdhxr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gafyajdnx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gvqirnvto.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gkifgeweh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gncwfhbgz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/guqwplpuo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/ggeglqfus.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gpbelwaxn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gpanvxxit.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/getnkaztv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gzkobpvxk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gfkmwafjh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gtynldqul.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gxnxjheey.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/grstzhkrq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gfpbtombl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gvttapxsw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gbpadytfj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gviqdzuwa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjhggykgw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/giefkvbrh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gobssatyy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnabjkjkd.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gbwfyeqdq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxldppivd.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/ghyaypstz.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gfqsqhwyy.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gfrogvaek.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gftoqifbo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gqbevivfb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gpainpmoz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gqrtvufoy.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gakpuifda.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gwlcuicdb.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gftctyqbz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gqtgvbhjf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gxxuhswwo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/ghkvcdilp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gfzhomlqi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gbwilosib.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gjufttmnc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gxytqkdon.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gtwbogign.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gwwpdhkxh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gtldyftaq.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsodjykcq.sHtML


<!-- 参考信息 -->