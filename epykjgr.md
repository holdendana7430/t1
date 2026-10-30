代发 wailian999

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gwzqcrkgx.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gjaxtnaym.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrwqinsp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyxnfoba.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghytolhbd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gcqzxswje.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gsxdxmvkl.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gvquaorto.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gzswbvgpw.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gzfzfxafm.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcztmjqj.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gmcuelpwp.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gcryhvgld.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/grsrjhymz.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gignufivw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gowrxxavj.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gkcnhqqaf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdrtpntk.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gihvwdbjt.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuahulth.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gzofyvzbo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/ggteumfsc.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyuenxau.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gldzoymzc.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gerqaixug.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gkahdpnan.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/grwtngttz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkjjhdsm.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gzoxqyyjf.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gptnspbrl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gjkqnojlk.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfchkyrxx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/grkvzmoyi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gtvuefdjn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gveieywrw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjvwhwp.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/ghdtweest.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfbetgyq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grvftipty.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzeyqxuc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/glqdfcqdo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwvtjcqj.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/guixjkkid.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/glemckxdb.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmxvnzzra.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gmavycrcn.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gruftwubx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhixrkm.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gbbhsvgjd.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsrpnfo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyplanae.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/grmuwgkau.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/ghxnmuyyo.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjisqyoa.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpezzctx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkylezfm.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdysgvpr.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzclufcw.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhrwyrjt.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gjpckfyzf.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gezxmtvvz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtqzlbbs.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giegnsirf.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaamzrpl.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvpcvud.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnofbzsfr.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gyspqqcyb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/geuzemtud.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gntwiixct.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gxptkoygf.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gndltrvha.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqxwlazf.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsoklmgi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/goitdftjc.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxelgblio.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmkdbvhp.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpttqzbi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxoewrcz.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsawwnbdu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gylvmdltv.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpgzwovi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzfenzyf.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gcinovcbx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeyqkdpr.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/glhjqwbmw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghszvatgl.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/grsrvfguz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwpklukj.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gvdpjevmg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gzmjmkwov.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzjnwygk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gbpcqwico.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgduybpj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpizhqshw.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gsyqpwjth.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gborzwalu.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgtlavjq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gxkscvqyd.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafdtblit.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gniulbntc.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/ghrfqxkhj.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gcthlpzdm.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/ggytrecvo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrxnjkjh.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gdawvowti.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gnjukdpdm.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gserkozio.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gudjclzcc.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/glplcxstr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkzsktsc.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/guximscds.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojlneolg.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcnkzqdu.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gerdkworm.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gvabijtdd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmmaogtm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gqaatnoxy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gbmznzbwx.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gtfnumbes.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gwuxpefye.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gnigjprrt.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gldvpeuyi.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrahiihg.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthzruwme.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/grbpytxln.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbctrkdoh.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqurajp.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgjoilpb.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gitzwrhed.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gejypgvjp.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdmcicewu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjhfwkfy.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfzbzjbbq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gbluszkgg.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/grigzvmws.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggxbzidwy.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjarcjtqg.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyumnnraa.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwerzuwdu.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmedlbnf.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gljugzfyj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/ggyvfffco.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjizjehpa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsopzhty.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gmerlbesg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyafuxyg.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gsajoxqyn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcswpbqql.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gglazzcyb.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gdppzaoiy.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzpxqmxv.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gfzetwbin.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gavrctomg.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsuutpin.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqvbixls.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gslezobvj.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmfsskem.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaeywskv.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gkvpisxzb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gjnybesnc.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/glfxmnfjb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gybnfsnhd.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/groubvviq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gplpmkhrn.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gewhnjuhy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/guchsbiir.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gnmvwbmyr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfaptzal.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gboliazfz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgzdiagh.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gasoljoqe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gxvllvxit.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhntiwnd.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gsnohaxvv.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gexgybuxp.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gnubqeutj.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvjkvjkt.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gcjqxewul.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlsgebbn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/geotcchkp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbrwdvbt.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/guehficus.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gkxqevvds.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkezugxa.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gphhrabqo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gzfcjewfn.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnnlwwmc.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gjpqiktft.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjjpvbmj.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gilinfbxs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqwzapdz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrrrhdao.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/giukaquuz.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjsurokc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcvjkpbt.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gxwvqvema.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/ghgyawghx.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gxqpxnzaq.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gawjfqzde.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxtmvhkpq.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoewkaje.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsffoxie.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppwictfg.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzjogfln.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjdsjlbl.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbgmwsgd.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gomyuppla.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gmietbztv.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gfevdskbl.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/guuotaemv.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyrsfmod.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gevbjxwtp.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gnpurbeao.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gkbndeext.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gqnjuminr.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/giastavzc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gzxvwmkfs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjdgdoex.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqxnamps.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gaoghstol.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gjluerbyz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiohlqhl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpidveml.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhrhbufo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gazrkacmx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gmwildvmt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gaucwzdsn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/goxdwzzek.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfdmurdl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gwryfmdav.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcxiofdj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgoxscup.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmfzkhvs.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrcolvkh.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gcchbmoab.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gcjqufrtc.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gcgjpobni.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnjmpwbe.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwkyrbsv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gfqknlamo.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlpjgumd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspgfsbmi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/gscxvknnn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gbvtxedef.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudnkrfak.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gqxhbpfcw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gyjbvacxe.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/gvmuxlwmi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdynovgox.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvwygfnu.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxydupas.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnepwtgux.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gvxookrdz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gjouswakl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmylfxlmj.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorzmffyd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/griptklwj.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gabkkssvz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gcvnsqcli.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfegreic.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gggmtjosk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/gclqjkljm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksputayf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/glvcaqwgi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbpwgtao.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gzjfrauon.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gkekitals.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcziyzin.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gobrrkgvi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gugxuuliz.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gtmgrfsit.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gaojxeuci.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhnykdlw.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaakjouze.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmmqzkhf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/glhvuhybv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gozulkqax.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvcknxtj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grbcrjptv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbokluqud.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjarbpym.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ggekxwmdu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgwnprww.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/giflclnsj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grouatazk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guhlgohzu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gymjmcdnd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gngloojqn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlcqwqml.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyoovbku.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwivojjnj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fanxiaobao.xyz/Article/details/goglpaexo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqlgmdea.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffzukabp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/glheusrsi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glrhwnivw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfkblulss.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/gbhmrnhff.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpiifyed.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/graukmzib.sHtML


<!-- 参考信息 -->