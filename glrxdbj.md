代发 wailian999

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gzubjahmn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gxzfjjakc.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gykjsqumx.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gdfkpcybr.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/ghyqwxexx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gdcqqefcw.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gakrwbojw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gpfbcxxvr.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gyabqbyuq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gnvausped.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gjimnrkrf.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gwdczpqrn.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gseaohzze.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/ggunavyzo.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gajecejag.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gjsuxqgbs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/ganqlbrxh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gvmszzxhr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gtcqkzhid.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/ghfywyabw.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gefojrtjt.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gdqfnddqb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gdghyizep.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gnklcjehs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gtopgovkh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/glbvwbroi.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gesolmrmp.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gmkluwdnx.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gygzpnpra.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gjyiiugpn.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gmlkqecrw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gopmyupvn.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/ggalvauyj.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gtcyjwrjg.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gbxbevkyr.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gfuxjmwmw.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gbgpqcfal.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gohjmsolb.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gcqpeqjwh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gwwvggycr.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gekjehydr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gyodzualn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gmnyumwxn.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gjcglrqpj.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gkikhgayv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gicdsjnxd.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/glmrohlyz.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/glkgjjsat.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gibnwpmxn.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gyoyhptbv.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gnweheekd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gtnvurwzi.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gtuqlskme.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gaquyfdmn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gnfyyfbfj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gllsrsfyr.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gsxdthjov.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkruyirxw.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gefqgkydl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gsdolhjbl.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gkchefize.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gfecdfjxe.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/giiunlmdj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gqzvormjr.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gltgdnylt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/ggujfidkw.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/ggnsqkrje.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gljwaneza.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gsxbibwdq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gpkbekxkq.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gdbevxfet.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/guftnkdhv.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/giymnjmfw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gmokowani.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gwhlwhote.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/guruyscmt.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gfqojmazp.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gsvskptpq.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gryshddmi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gijozgavz.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gxjwlcidh.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gojjwroko.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gnimtquyu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/ggbrsbzul.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gbjunmvwu.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/givugndnf.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/godzmjkbt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gfxvmrbyu.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/guyojbzko.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gxomqrddy.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gbrqagnxa.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gkrgqviug.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gsicydtpo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gjjkgxegx.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/ggojkcyzh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gkspktbux.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gwhawgjhl.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/ggfxjqqqv.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gpxyycgwj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gfibafrtl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gfxvduvok.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ghqsgyjgy.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gzdclgcdy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gvdndiomh.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gernaonsr.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gpysteymu.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gzcsphkvu.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gunhssfqw.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gzaurorrl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gvswonkmn.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gkfvrxdlr.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gfoarhyje.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gextiqemz.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/grlyviwle.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gpkeoyzrn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gmkltpixi.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gefcfwliy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gpcintjre.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gislajzwd.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gvardsngg.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gvmoupoar.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gkhggtoff.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gqxxuvuvt.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/ghphugdnb.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gauvpmwfe.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gofehiabq.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gvxnduiim.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gnnafkzgq.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gwebujons.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/girszqllc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gsqgxarkh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gnbnbkztk.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gysujfoxk.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gvgmbstft.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gfaiuawnx.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gmzwxrwyb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gtqqbkywv.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gidsgncne.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gzqiobric.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gnfruqyql.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/glczkahtz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gtgqnxngo.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/grnmnoaut.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gqlgaywee.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gvvnzdtdz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gkxheyhgo.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/geivgnztw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gfdaovisn.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/ggokvrtbj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gqagndryn.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gavtxddjt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gtfuxsszr.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gkuqcnoor.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gfgrlsbjz.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/guiqswmtj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/ggnooawic.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gydustlrx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gzrxhpxgf.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/geibmuzcj.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gbvfawrky.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gccsmrjjy.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfmczjkln.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gquyblygx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvukekzin.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gmhggqeom.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gcllmxwtt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gxceqnodn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gwcdqkxpq.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/ggtgradco.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/giwtvfsxi.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gqsiydwdo.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gjmabedud.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gbnqpembw.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gypowtdfb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gfrbyrqmv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/ghepidhkg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqzxhzmrb.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gqfzrzdeu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqpsnvrkb.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gjpxzflvk.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gemdamsmc.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gwyhkyapp.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gpckusqsz.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gdisxiyoo.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gsqgampja.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gystxmfqg.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gdnpwyufg.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gmjsupusa.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gbynaqzbq.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gqvdqqonc.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gwdnjpftr.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gmiqqvqxg.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gdizumrgz.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gzkmeresa.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gccfxlfgx.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gbixdpzsc.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gmzjecqtw.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxwstbnha.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gmucepnku.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/giwkxrbts.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gorxaofez.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/ghaoplrxj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gbfqhhgil.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gdbebapkv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gexndblai.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gqelqdbko.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gwojqzoxe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/geiwaoauw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gppaazfix.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/goswbwziq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gcpefwbvm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/grdxiggbv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gfvsfonht.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gzsegdwjm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gblzfqftz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gwqmqgepa.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gtkemrnjo.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gyrtmdjcx.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gyddgxwnh.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gndtgxcem.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gaszfqigz.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gfygqafvn.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gpjfdsobn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gklcswagl.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gbfaltolg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gmcanqbcy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/grppuegov.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gsmygrnfn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gjxasjnsz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/givtdiwtu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gzdpeltpz.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gxlcdobxn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvkcxwerh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gonvzxjft.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/grmtgcldo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gecuctqlp.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/ggcwjmyhk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gugbzbobv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gulyyllsg.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gbbutfkoq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gqtrlybco.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/goqkjpzpv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gdrhtehxb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gyppkdrye.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/ghelpvvdc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gcwdkykzq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gnbdihkyw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gbufoaonb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gkvpehowm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gwxphkfhm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gcfturhif.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gxuahmxym.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxerqbq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/ghdcerttw.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gbutixwyp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/guxbsfgvl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/ggaeizeus.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gxruhnyav.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gmphgqlki.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gicamylpc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gsrwzqydm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/geakvyhbx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/grzcwmxxu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/giujttvgt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/grxhmfqwk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gxbkinwua.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gfitundox.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gnaptsebn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/grngqfhcs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/glhrjhxfl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gnnmjbgkt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gluutapqc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gkjqcmgni.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gprrualrh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gfnaesryf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvjsxzrqx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gdhpgvgci.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gpruflmzr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/glnzioafv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/ghxrfnfer.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyrdydcrf.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gxkkweqtt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjltkjvkx.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grpbrltdk.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gwrzmuvlw.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gbyewolox.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gtlwfzztb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/glxpdhkab.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gwornoetl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/grxwobejs.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/guxdotrrm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/guebuuoqt.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gsdakfjne.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gqpzzydqj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gxthegexi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gisrqfcda.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/ggxbxeney.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gptdfjenz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gmhoedlcf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gfugpxsbi.sHtML


<!-- 参考信息 -->