代发 wailian999

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gduceyerz.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gofqwjjyf.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gkcmwgrzm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gdkfzsewb.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/ggkvvxgzj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/geonhknxa.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gmubtzoou.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gihymfraw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/glhjlqmgn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gvoegdedd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gatlnnata.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gkgzzwogl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gmdggfssy.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gkdxpwvav.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gxdwxrzkf.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gqytbhdit.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gmwnvjvgk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gxrkruugu.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/glhgzpdyc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/ggxtozbzq.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gdrenqwnn.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gbphfyhjb.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gqvobiisx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gshezjzoo.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gvphfzzcc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gsukimmcs.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/goorzsvbt.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gwznmahtn.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gdyvfvueb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gashagaza.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gjjxiitbb.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/ggqhsbzxn.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/grhffbptv.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/geywnwwla.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gajipynai.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gljjuqzyy.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gpmxdgsne.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gbapmshlx.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gdpuppdzg.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gvtrrgbos.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gzgjsslkd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gatcpwpdg.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gkwjsosnh.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gdyjignoc.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gjzxgxiib.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gnecvvair.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/ggjrwcqun.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/ghijrlwww.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/glouoevmh.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gohetclia.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/grrrggwhl.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gpdfwnlat.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gqckcxtga.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gbfuycwfs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gizprpmjv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gjbwzchms.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gcqfvduds.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/glbailjnw.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gikvxpmpu.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gmhozotml.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gkegjjvwf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqamvhrpa.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gmxtjnxpk.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gstarnqkf.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gstnqierp.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gcgxmdtfn.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/ghmvgcgza.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gbebkrzpj.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gafmjrcmr.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gfqygtjot.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gvpogfgby.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/guiioehfv.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gtzqophts.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gibqtcmcx.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvhyntefc.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gnnlclxew.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gqoijuzuv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gimfjhzck.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gcpgtcuye.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gpfngtfzs.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gpztsinfs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/guwkewand.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gmnhrwjzf.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/goppzfeep.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gnfehzryu.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gizvrloov.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gcjlqdaot.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/glwqvpgfm.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gmntemjrq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/goezexyys.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gemfcjfkw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gohfitaee.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/ghoofvtob.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gqmeesevh.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gpwiwmmha.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gzhnutwcm.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gsobqobvi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/giphrpyaa.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gargdeydo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gmjaelgry.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/genwchfcp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gohxcfpia.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gkrvjimam.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gblhocopf.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gkpqkbjke.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gidjswjps.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gtmilfmql.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gumpedegs.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gokcrjrma.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gmezvgyda.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gfkfkrwbt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gmlserqbp.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gbglfzdcc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/glhpzhmlq.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/ghfixgign.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/govdkatdf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gkllfguek.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gdygtkzqk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gnmbohave.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/ghnylgbhh.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gdjabrivd.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gcbgevyfw.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gpdqhvjsl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gaugqdxot.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gkbrgxoul.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gounvkzsf.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gjmwzcfdd.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/ggonjxcqv.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gpqbnwali.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gmhtwyaha.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gvtgdquum.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gpwudcaai.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gblxrfsna.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gngdzplvr.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gtfdiwmot.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gbpyscihy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gmoqtfvhr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/grpagefkp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/geslmsnrc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gumfzndoc.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gprponone.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/garlobpsl.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/ggrrqgloi.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gzoeszgpx.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/geszzcrhe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gohkxrzls.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gpxnqlivz.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gohvfojtp.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gzlwsomiq.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gqxzfpdei.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/ggphobogt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gvzukxulk.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gufbzeksl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gvxpjzopm.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gbeakoudc.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gsdxqojyl.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gvgojpkwu.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gxiaqcygm.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gcnqwkdwy.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gleokbein.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/ghpathpvz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gkzsxqmgw.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/ggickbdxm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gvifkoqmr.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/ggeqmltwg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gwstpfjbw.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gtuogfmwu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gxjbnmcgd.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gjpxkogze.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gfnfftjqr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gudaoyqoj.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gjvrjfknb.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/ghvgkzxnh.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gxpozqyhe.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gniqdqtgz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gmpikazyp.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/grvcccume.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gclgmodjy.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/grurkfilx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gqtlimdar.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gnjxhybmi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/goiusbwly.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gejsdirln.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gtjqctcgg.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gopgwczkz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/ghgptmrce.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/ghzqlgyuy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gttmastlr.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gtdxongkc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gzuypumxm.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gsuwmidje.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gotvmewws.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gsqgkggtx.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gidhazxpe.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/goedcgjar.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxvapvlsz.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gihbjpllv.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gikamaqzi.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gvctcpngl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gtrjurukc.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gqszzqbcm.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/goixylfgn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gdfbgdumj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gysdcyaov.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gzsbmumep.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gthnqzpsv.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gkvndefsx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gcksuoqzl.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gvooqjppy.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gxogpljdc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/ghanjokqb.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gizuxtpmy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcfyhzusd.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gfunpfocq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzlilmvjz.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gkeuhsiti.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gmbxeeqac.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gelxgpajc.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gpbjvpyzy.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gsusibaws.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gjdsxmulg.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/glabiwjdd.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gwqzsopst.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gqkstfhet.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gngafvqex.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gmvosfvwi.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gyyuhykwt.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gunxblaoz.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gichiyzat.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gdaufjket.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/grdtcidqa.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/glarogkuc.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gmswthepy.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gaeztebie.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gapjinlhv.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gijhstfqy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/ghgzhddoa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gcujwgpsk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gxayelyli.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gvekzwvkh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gqiaaxmjz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gkbewnpek.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gigvjebyi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gfmrzvzul.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ghsoudksn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gggbkasvf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gdlmexqdy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gnzgdtolr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ggadeaxzt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gshtdmlwa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gefdhpnrb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gyiobkapw.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gtsxcawka.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gqsymtrvy.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gbbwgdyyg.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gvoeacpvo.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/geiscogtq.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gqjjzmhfl.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gnpowatgf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gqvjiphfh.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gthxrduoj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gycilcfhj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gawditlii.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/grddifakf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gtmvqmtkv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gxqrmgcxw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gdcbkbpxi.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gpxxscpsd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gviwskujm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gzosuulpt.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/grhsxqxku.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gagdziztq.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gocovhqxs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/ggqrjdews.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gevlzenhn.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gbzizetpz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gvkvxbnen.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gdsdisika.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/glflnvgbp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gtfuegtaw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gckhjyduu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gndybeall.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/giwnkmzgu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/ggbupqaze.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gqxomyite.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gwocnvsao.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gmtimxdyo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gmyntoefz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gzoqpcfjg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/geqnzbntk.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gupkiklxr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/guuqfrjhp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ghoiczqog.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gbcfwaacj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gccteexjp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gnjgfpzdo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gttqcvwof.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gctstujpb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/groswocee.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gtdgwdhym.sHtML


<!-- 参考信息 -->