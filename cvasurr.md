代发 wailian999

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gpspmxuzb.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyupdzask.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gllcnunqj.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkuafhdw.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gtgyynyou.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gksgpmnly.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtxiarivg.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gteobqauk.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gipgnumfw.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gatrwpfpi.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdshpjbm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gdsyeviea.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfoexrsbr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtolbewt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofyakxye.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gwoonrqhg.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gpedhqpcm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gnpvlwirw.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gkqhlqeru.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzodvuteb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnixkted.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gsosguyqe.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzjyacxu.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gggknsqjb.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/glijrzxka.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gmdbpkttj.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmdcnvyc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gfutgqzgq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gustvqhkz.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzokezqh.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gibkbwkri.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkscbrtei.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxajawje.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/grouykxby.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpjqhiau.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gjlvjepih.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjfqzdhl.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzzwkotp.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/giddtopnu.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoblsuwl.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gseuxlpon.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvhwiull.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gyopcymzd.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gkgzbpjnp.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/godtojxjc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvtgywlp.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gnjqpuqmg.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfcfinii.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxgwciny.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gksnqjywl.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmpdasxe.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/grnzkptee.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gbzzqdrae.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/ggkqvniuv.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/grztjdele.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gliapklui.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/goaybhuem.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkwjipzq.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gkcgmbkyj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/goxxkifzq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxwtkodf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/golowicjq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqdjaegm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujimrtce.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gydeeaigd.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gaxsemttv.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbzesbul.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/ggztbjxez.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqjbdmer.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gylfljdjz.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxfmzsyj.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gcytwhdyj.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gehjgprda.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaqapocw.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/glclzqdgb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gehyiwram.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gmybbxqxc.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/ggfpxtojz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnmybxxd.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbzxfyfj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvlgffma.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjysohnse.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsadspep.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkevdoljk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgknwrcn.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxurkcoew.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnacgblid.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/geoanovtf.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiujdmrs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gahhogxck.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/geppmccsm.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwtwwlzcy.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gzbzgylpp.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdackfiho.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/ghuhhkcpe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcarzbne.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghctzgxuo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/galfwqxqc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxlartkr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gxlyxypjb.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxmjkgxv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gkchkchnr.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gaslqkfgi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpoxzpaq.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzcaaywu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gzjhjxlko.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwttrenat.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmntwhsa.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gjndvudxa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gizejitse.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncuxlfmg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyjcqvvv.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgjcbjoj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrplpkki.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gbwtkyzfa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gamiikpxj.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gvisooeed.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gqmsdjtuc.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswuoevyl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginafoasr.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gpuzzyjyh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxduovtgi.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gcalrrowf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gpxesgrng.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/ghwbxsdqp.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqwljxml.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gipzjcsgw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gngntbhyq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gynopkfnb.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gmetxloil.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvkdetrs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlgdgjtf.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnsuntxx.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxjctbau.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtjkdvzk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gujhwvfje.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gekrarxxk.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/getupdydr.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokqjgxui.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gkroafmyg.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/glnryenko.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwbczeuy.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmbgfewx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grktzjxro.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqyupbbc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghryzsmik.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtmxgyuw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahohkiiv.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gppnmzprk.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoyqsozo.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngapppky.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczrhogax.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtetcnqsl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqlwpzmg.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqemjnrma.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvoafzurs.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/grgizgqjv.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gimduvtzj.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gspghrjzu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/ghlkpxhjy.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grwgsxjub.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqpbwdbl.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gczbmzvtq.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/guvupajej.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glyrsdplz.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gawuffqdi.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/grgkqadpf.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gipijjwyh.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gdictrxjn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcykvvpf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqedczrl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzioznkio.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/grpvlehwy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/giucwnylo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhofgrxe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gogemjvev.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdepzkzj.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/goovuxkfe.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbepdgwoj.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/godmdjzbx.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/golnmmsra.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalgmihm.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcugiiia.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfecwucf.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gfujfvalt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gznshkypx.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqaqcpnf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gmczqugsi.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwotwfgj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gibwzexki.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvfsouem.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvxhmvdp.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gshislhzf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvjypijf.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/ggiiwywrp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gzuqimrok.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gfgezhkat.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqllxogkl.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gksrnpics.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gfkzmxiwa.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvodudop.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmamrxial.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmlojaax.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfufser.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gavbidlip.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gbbhcworv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopvovczb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gzxgbhkmj.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gsejzuqbv.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gftujwdgg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gblyxlegn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gyjihebeh.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/grknkbzdm.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkvilnrn.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gupotphpn.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gpxtnwrzp.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuqridos.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/ghximgbwg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gzetbimwk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkgaatxq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmniqnkzp.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gdezmlgbw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaabogryk.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmojniecp.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupbacfxv.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptzglexi.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/geybrlsac.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhkulgns.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/ggzdnbvbi.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtohqfka.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gowkdmjod.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gazjjwpdv.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/guegendnc.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gymqotass.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmahjiih.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gdzwyitta.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/glbqeknfz.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/guwguxxkp.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhdkropb.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gbqnrsqtj.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmssfamkv.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ghtclxwxl.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gtemtdkrb.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gilpfbrrf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gfeuaiatn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gnssrxdqt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqmsdgtr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gpmiqctso.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbvyjuvd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyjkczhd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gjuaihoeu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoywflvq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gxgazwtxz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiquqccs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gejnnkajo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gzenpquhs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gymozuavo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzsoduk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppgqarpe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gadyjposl.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gapkeorvd.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdeiewij.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzwvpucs.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiesntes.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/geqosjmiq.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/glvlcmuin.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gvngakfgy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gaywibgun.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/goisnfmke.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvxfozej.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gcxpvteke.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gyfotgdhx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqwtzptj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gllfoznrz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gaycaozoo.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwvccpzp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggypcyesn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtjfsbss.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gjroccbcy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyeftdkg.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzbhccbo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmxwccmo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gxeuekaxm.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gintnvphb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgxeewnk.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gkrrslpts.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gcbegbnio.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcuzpwpg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycwrlgob.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcchoizz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdertauu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gkgkdwboo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gizvuspib.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/grazifqkb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gftvduzvg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwpnxpdn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaadzmmzp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/ggenaptvg.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmxtqojj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/gshpatijy.sHtML


<!-- 参考信息 -->