代发 wailian999

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/ggsjjgccs.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/geqxhbxtu.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gvcnktwwa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gwmrilgfz.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gwtnvvcrc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gfrzqsmky.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/glhghvkmx.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gyxzlrnkd.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gqvjumsxj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/ggtrnmuvw.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gwslvqzmb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gjizyzkav.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gqybcbgct.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/guratlbyr.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gnfjlbrzr.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/glpqvalds.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/ghsrpemec.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gpsaiousa.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gajjzcnfo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gjzatrlam.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/grobyliay.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gdsnlihyn.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gzbnnzbdf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gokevdlpq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gydpirojj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gtyfsjcrb.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gmmwomjgb.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gzisphlio.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gytraebcz.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/galrlyiny.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/ggfllpiam.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfpsbde.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/grvxmamgk.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/ggpapvhbl.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gqjdrxcav.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gkbssqjsl.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gqrhykkbw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/glaciplqs.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gwkqxdwxc.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gfznkndah.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gpeoxxznf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gmwouxsru.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/guqcyrhrz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gecxkgsef.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gonbedpah.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/glzprjnne.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gxtmqkmcx.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/ggjgwians.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gonhfeuur.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gqrsblobb.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gudmhyywg.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gvzgjyrmt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gjxlrkxkg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gpzydpoyg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gvdzducjn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gmpbutptw.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gewlyudcs.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/ghyxerrgq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gbqisgvul.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/geeirdvup.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/ghvoumbxd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gvrfvozgx.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gqntvdilm.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gvlceilns.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gluwllfxo.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/garkrtnvb.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gqzwdlqgg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gztepgozt.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gmrlrstul.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gffaeyrau.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gvwcujeof.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gjbirzxuy.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gyddigxgf.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gawzrlyns.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gyzaldaoq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gayetzccr.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gkvqebsea.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gxprqosrp.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gkbbqbhbj.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gilrwbamq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/guqgneppe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gbjppjzsg.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gdlfrhykc.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gllrqfkhw.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gbcogxine.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gdtotmzbo.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/glymqafwv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gpxabspjx.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gojhbkcgs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gtwopcjli.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gtyzrpemx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbilruzqu.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gqexjpxdf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfvgdicle.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gvoyuwyqm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gkitvifex.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gqskzbzpb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/ggtfdqtjk.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gjjbcqlme.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gohsyhzpk.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gfqjnjzry.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdgaqzdzy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gkxepimxb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/guctylzyg.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/glupptpad.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gbqabsogr.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gzjpubwyc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gzkiumbrl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gcqtlqwaa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/grqjwgjfw.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gdygqunbo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gzcepwgad.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/grehozrvv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gmvkmpunh.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gpggqttko.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gefiwhxuo.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gwlluzulm.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gdmmlgvav.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gjkyxtxqt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/ghxttgdwu.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/ggbnuaxpe.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gvmhqbwhs.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gfmbnskox.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gnblpjusr.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gbeyoaqgz.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gthzofmbi.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gkxkevwwi.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gyvzekekn.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gsyqwnfsj.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gduergvrm.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gdbmcqegl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gbfiwjpdr.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gihlbfdmv.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gpfpvimym.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gaqfsfvvt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gcdhxmfok.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gftvaalgd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ghavtsuji.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gbfsahmhc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gstayheub.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gpiqinpns.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gbxscpsbp.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gulavogio.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/grgemukak.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gfjnpwzoh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/goiuhjveh.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gzorzosae.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gcvhvsggd.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gajhlrlvj.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gzdwbhafn.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/guaebtcon.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gxlaqfoqr.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gtzyncbgl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gmzzjwywi.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gdkuhyfkv.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gckptrzes.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gasalhbcv.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/glettsjzl.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gtzactksk.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gpkluhhzq.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gksiynggu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gxqbywkuq.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/glhffbmet.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gtzhxbhly.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gryuyllvy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gmhtnjwig.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gqckreaen.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gwvfdnsqh.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/godlfbgro.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gfnypeipi.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/ghkkjkahk.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/glqbnhypz.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gevokbfmc.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gtbxbouys.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gozlxjubg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gckhtfidl.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gxrknkwlp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gjkomixpi.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gcwbupbgc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gkxxoukjs.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gvvitwsjb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gmhmtbshs.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gpdkbjphy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/geeaosddf.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gqjnzxsrx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gmfwykzaq.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gyvfiimld.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gldcmlfwc.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/greattyax.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gqzfpgpkx.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gujeqoszg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gnbemcrop.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gtjnpcrck.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gogxjmgcx.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gnkyseyyh.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gyajokgjo.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gnewxqpol.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjestcxlv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gndgdlbpu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzoobmelb.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gdbkxjhhh.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gcnfskpds.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/ghbcbqhtx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gtkxjvdbj.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gextthewu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/goiqemjuu.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gkevrrijp.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gkxrqmbpw.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/geonvzzwr.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gbkaxccwg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gbleuevra.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gwwqgvhgu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnwwxsbaq.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gbaxvhlfa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbxwpotjd.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gwgpratph.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/geutrxeqg.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gvhfnutly.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/ghnrskqrc.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gxppumfbw.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/ghaynahxe.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gjhwafsit.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/geqmzkupx.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gnbtdojmp.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwiayyg.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gbseufzbt.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gvdhcroco.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/ghtvxdpax.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gkcdmaijm.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/grvxykdvg.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gobuehpqw.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gtnrcqcnh.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/ghebjnygz.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmgiavuiq.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gtpimsckt.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gfqrfirma.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gwlyijggh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/givvgsnfn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gxpljmtah.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gwdwkehhb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gqoalwxns.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/glbvjlwkk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ghbgvcipf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gvbtwbqqt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gcrbbqipe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gsabkeisf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gzvztfpyp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/ghwbynmln.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gfsknrhix.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gchvllwfv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gknitkqyq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gexkqqvtr.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gwttuwkuh.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/grvvvdikm.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/ghzswkwln.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gccyidmft.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gbyqapajj.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gqrcrlbiu.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/galmnifdz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gngktpbua.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gzuuguhan.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gmwhwjfwa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gxriokfml.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gehrqgufa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gbyjhusog.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gnmpphccl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gijdhccnt.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/geazgbuzp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbelohpah.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhmehxx.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gblytqimh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkvtmjmii.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gxiontskc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gyiodwtog.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gduopeuei.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gkdifkjxu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gcvafmrvs.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gkkyejtrd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gvyonbard.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/glfgkuxmz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/ghqkgnrrd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gwsxoiokx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gdowffpex.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gnkfrdcje.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gdrlsduoj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gvhpnjmsw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gngqlgujp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gpsoresfb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gmppkokil.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gwmrjnapv.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gxjhphnug.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gsinmmnkh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gjdnguwdz.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gtqwgfcfj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gbnocpwqk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxzuwvjmf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gbtlyiypo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwyvuszua.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gimexmuim.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfhzibcnl.sHtML


<!-- 参考信息 -->