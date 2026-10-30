代发 wailian999

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/globsevwl.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gyomhjeuz.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gtcielzog.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfzprjhz.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/ghperldsw.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gwesadwca.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gqxrbavys.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbhdfyiw.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gxbsyxreb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gdhhnocer.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufsyjmkd.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqvrccre.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzfrkuqs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqekztyn.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggprocyjd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gwsfckcaq.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gmoawxwic.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gfsfaalue.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gmndjrljh.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynkzvmky.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdzzzzrf.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gozbcubmm.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwjffnuh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giflepvyp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhqtbsru.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/golypzvbr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsmqehln.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghdqxxwv.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgvlbjlp.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gujiszocu.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gcflzrwlc.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gymzmmzwq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdnqqcchb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaytgcpit.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gkssvqtvr.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gjyjmvlxk.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnhtxhtop.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gpbwzoapc.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gycxujgnk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxdrkhwt.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gsypnicow.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gsihtblql.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gdapdmkqt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisehgfrd.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/ghwbybhdf.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gvwvyjsql.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giteadzkj.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gmlggtrqh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdzvsjic.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gkdrrwjuu.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gjtntkjrn.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gtxihahgq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gikvzprgo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guckpjpdr.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gujmxmjhh.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckakrvtg.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxuhdsq.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpajskvfq.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/goyarqycn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzywwsxe.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdnwhbmyk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdsozbdn.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrmnzbbp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gzolwxlyj.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfhqeter.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gbnutzfgf.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhxcyvqh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzjqivb.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gkcesffnm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/grmwjyore.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsxgtbpdp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/glipxidxr.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhzhiqoj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyxgsxmd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/giofeipra.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gfwqpajrb.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgcmknkb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gwrcrcuad.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gblaynkwe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gexoexweg.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/geunugbxy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gwfuqbbtx.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gajzmtugg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjtaaclt.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/geicxwfzb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gustpaiom.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gexahooep.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gwuocgecw.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gbpadpprv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfrstgqr.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvptsfcgp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gcumtuslw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagyiakir.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmymniqbi.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssaskqsg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmhhbjji.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gcgghooqc.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjsetbjr.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gmanmdpyn.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gniyiabrp.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gvcbomjyu.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gnztejqbw.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsydxdtk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gckmhepmo.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/ggxoiqoid.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyjobmra.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhybisny.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkeykswc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphfmrxxy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtadxqod.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmgdafne.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gactiebmw.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxxehzwq.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywsctdof.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gffvyxgct.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gbfnggrat.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgvtuayj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisilpyge.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gztzjqale.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/groxyndkl.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/ggygtpwtl.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gsiqctfrk.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsvhmceg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/grnkpegld.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/giojjnqpo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiukfngj.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnrkalrij.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gbhemhewh.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmwmghmzn.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gkwgiyycq.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwvbkdyp.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdifjcvc.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gpmfkworm.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvsbecaj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/giofrinch.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gswkrwgyr.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gtbaapbmx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gmmqrzahk.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gbicgwcuu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gajifbmgz.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgksxndn.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotgbodet.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxwijzqdo.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gewkmqqzs.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwpohopu.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtzxdhgw.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/giweluleu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdjmwbbi.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/ghtzywcju.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocyqepxz.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/glmoslnkh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/giopzvhqy.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/golnabrvr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gewddypbq.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkqybqlw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gpjcwsljd.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gfjnxcmoc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwytoxmhz.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmwsbzcq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/ghrhnlynw.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gihyltuvv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytbmfqbm.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtecxijs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacygyetw.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gsdctadcn.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gicxruoza.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiaxwgoi.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/ggocogppq.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdzijwlm.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gkhahaows.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gulwstsnv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonnwqdvz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gverhgwfh.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzptfczvw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrbenfiy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkvlwqjji.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjgrsnxf.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gcaqpirdb.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gsljdrzoc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcpjyebx.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/ggzwdzewk.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwmknsbf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbfcpafr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gukajsmhh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjhjfrxf.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gcrvnjnwe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxrsuimys.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gzxqaqqiw.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gszhvvhei.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gtukkutsq.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmysaczo.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxdlisfzw.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gvmwfgxfc.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/garylsvap.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gorqwcmxl.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gcpkqvyth.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqyeypng.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gfvwmlqzb.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqcocktl.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gvlmlpvmj.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/ginhibjbg.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdwwjdpv.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gwydxtabf.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeqrpbnh.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gvmvywlft.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gilzwouvd.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gkvpqnmni.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gxvohqstt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gzfynaozv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxdtijxr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gemnnpsbd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobjifjza.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvbhbzqn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyoetrob.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gxlphgosg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gajvopfrd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapgjxtbk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtnrqfur.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/goxpyebvw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gemsohtde.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxwbbidz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gudbccymb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/guhhzgzsi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzbzvtao.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gonuyoglp.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/guyayzovi.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gauwrmfda.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfumcykk.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/grmzmdtgp.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqbexycx.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gptmrucmu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gpjrmaick.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gdklivcqu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gzjmijqjg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gqryhqowe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gqwzcpxpm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gszqkjwuf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaxfevkf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/ghcsdjbkw.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/gdmkvmqmu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzthspssx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gixanexzd.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdvuclzx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdknadzbj.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gucyssdry.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gsbtevmhj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbodyyblu.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonsuaikf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gxnykxtbl.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtnxyefk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpsarebe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuvbknqg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmkrwxre.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijajbegb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrgfgrtt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gooidqawg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvyzliel.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwcznnv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknsmqggs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gbqubsnki.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgdrrlda.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkrlknqw.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gcurdapef.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdcrqvnt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gartemeob.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaltzqhe.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gzkbdpjol.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzruccize.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsnxeguu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkpuiqezs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gimwllyzx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glgkmsyaf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvuyqletb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gswdlpbdr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gjxzdupkc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/guwslicmh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdaohfmyg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmwnxffv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkqtqsvx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/godrbircm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gngbcjrwj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgnxdlqr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrpncftc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzljoqirk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/grpofcgpo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziovumms.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/ghgwytlzt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnosefxhu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcpadizn.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gbyavjite.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggbydlhsq.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggvxtxtwp.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gwbirnntg.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gfksjtjtw.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgxhgrtf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxirfbwj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gletxzghb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqjodghg.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjlvuptv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gqggqnsij.sHtML


<!-- 参考信息 -->