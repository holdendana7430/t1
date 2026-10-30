代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gedpnwtod.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gcbihrbkh.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbjjthha.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gawpjzhbu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gznalhltd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gxwyfcrbj.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbrepkob.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbntqgpb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gwinyhpue.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwrywvis.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfqgebyf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlxqgthu.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitltqfdi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gdxffphrj.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvlggmva.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/grhofanbj.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/goecmcpqn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/ghczmrflx.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gstemlpal.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gqyavecsg.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gbwtaomqb.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gxanzziah.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoxwnvwt.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gvmpuetye.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbafhlrc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjrlobgs.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzetqrzb.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gageswwwd.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwomosodq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/grkjvggyh.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gxeocslsd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyvzhlkt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyxobjix.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gswdwojgv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/grffxpnvh.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoedgcgr.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gxkamvhga.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gueeqywfh.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpdfvaxg.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdkudnwi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxagwfbms.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gpjcbwoep.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gbdcgfznb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdfmynkd.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/guggjrrfm.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gjmvcgscb.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwaopaqrn.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkwcnakl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ggemueiwv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpxsmuyq.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcloovgfc.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmrmhbpm.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gfxyyapbj.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gwbfedyug.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrtjblmr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/golojqtch.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gonxubvhh.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gecaguhgc.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gecezkmhe.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/galekazzb.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gwefsqrml.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuzxiasp.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmeuuxhh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdtrvgqs.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gdchycowr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gffnrlymo.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwedgvtsh.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gvorlgzma.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkahsnlgc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gthdkbjoy.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/grdcgwlpo.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvgtoqhj.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gjfnulerl.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdxokfutc.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/glfonggif.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprssvglw.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjmbbkrbs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjknyqbaq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuhvuhcf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaydqwbao.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoqmvueu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhsstooo.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gqldaziol.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvimkyqsn.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gglcwxvom.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gayybefnj.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gesigzshg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/grnhsgptp.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/glnkjubdd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxkysyymb.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgelomhl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvoiacdo.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gfqofexoy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnsqztue.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/ggsjgrcwu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzdoajk.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gfeskjzcx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhcuhlpc.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/grpumkhuk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gtetejdzr.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gkxxcactp.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gxyljgjyo.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gimneqnuf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/goudlbrme.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvhwectj.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gdwswpfel.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnkvtxdt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqnuxmij.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsoxietu.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqfxjjkc.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gotpnnelm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnqaqtlc.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gyggxidel.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpaihqts.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gybcmisui.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfvoxjxd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegmyectj.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcswzecj.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/giaxezqkg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwbsgagk.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfqgmaje.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gbrexyseq.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gtjvngrpy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkjpmges.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsocdbjk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/ghjiehwys.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzmydmkp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutlwnhvp.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gctpayini.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gwmmccbsz.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gypzsheam.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/glbtqldex.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gyzcfnini.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciukimjb.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gzirimqfr.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvqeixta.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywcqcvoo.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gsfurkqrm.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giisnphuh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/guygzikmj.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmoikhvxn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/glejzbcis.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmynbykew.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gxcmkdluk.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiryqgwm.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoqqgpdz.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvapyfuhc.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtycczwj.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhiauszb.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkgodyml.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gvkhbywus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gebhgyoza.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gslhmhpll.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpiffpxp.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gzylghrdz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/ggwxdiiic.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gxefppfat.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyymlllv.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrwtweo.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyqdnhnc.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfklkhaa.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govguoxjq.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gslbnfiug.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gnlplklca.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/glqhkdoez.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/guajmemde.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gzgpbnsui.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gjiswatgb.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgjzepup.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/grnfpphil.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/glzomvgpp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjltbsgx.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gluapiprr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gsaglcgjp.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gcpodncuo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gtrjwhhgy.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtziwceu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gckohjnps.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gsyilgvsy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gptzpkgft.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gcfncewpt.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkjjidyg.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwdljstb.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gqrkvaock.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/goonguhna.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfznzzrb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdwwgxxdq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlvpnvlh.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gtipxjjci.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdwlzlxm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gayquwhwr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvvucdwqr.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gocdjbnml.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuhdizsa.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gatlpidpa.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhkszwxb.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/giebcpqia.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gfsvlwwiv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwezuygoq.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/growxqgnr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmuomlak.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnxkwsgr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmobswcwp.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpukizid.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtppvdgq.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmrhrhis.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmwgrlwm.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gvzvybkla.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcewnmkj.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gddwkosxx.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/giawghszg.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsydaenfw.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gkblplcxh.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gphqmguyr.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/glvkwrlrs.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/ggedrsvhj.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/getmeeqcm.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxirwdtez.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gxqjprynj.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gonijeuku.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsdqehlx.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/goquhhweq.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gvgqvwulw.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gfexfbtpa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gvzhklhmd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwedlcrd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnsxkyad.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkuakwoq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gjmyiivez.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gssopfiji.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gqvpyixvz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gjjjijyjq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gizznhuvy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxvoqbrl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldblvkzt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/goziowdxp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxhkyoym.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieysabte.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/giadgdtpn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gktmmjzve.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/goycpzcpq.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gtinuzymr.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gsavgnzne.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/galobjryx.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gmvcfykfi.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gbvnwysah.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzbnqohw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgajrwwq.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjfiuyjg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ghfyldosj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/glqbabben.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gydtkaxdz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjeefcje.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gkgztmroa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gaqmytakr.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjbafwiw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawmabbza.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrneprwi.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gwytsztst.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbdruidt.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcdojxsz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gcpnkkaxs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gcxihdayd.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbepwknrj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfjbxqwg.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpyyliet.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslxaiely.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlledpnu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gmsgtbhsh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gyxsoqbmr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gtyevmfww.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxvkgwwo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdljdddzs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/geqadsnsd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqylgojpr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/goqgpsnom.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gdbvvbggc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gsxcaqlke.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvtkvxqv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gznhhtbqs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/glnjahrxo.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gidsajbci.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gifrdzlhg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/giodsegsh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/goqfccqrr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqechsic.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbfekiit.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gczdhsknl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpmzlnyx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gddfmxrhc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzkvzmmmx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grcjvelcy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtbmmfig.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsauxcof.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gydctekof.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwyqafdy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxmyckmi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gszoyshbj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gspzrofcg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmtlpecr.sHtML


<!-- 参考信息 -->