代发 wailian999

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grbpkebzj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gajikaoai.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwjcqvta.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhnjbvox.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwfmpbhkj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgxotbqb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gutwbalvj.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/grcqjbkjs.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gaahsjlad.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghodkdigo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuwzuzfc.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gwolvunnf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gvuuyxlpp.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajibmtai.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtelkkjot.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gehejjmzj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbxppqjn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkkinbrls.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjpesbncd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtcmxgrh.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gbqwawvlo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmdqtlyj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gfqxdxjtk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gclipvatz.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpemtmfw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpccacjnl.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwyrwgji.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/geslvkjjs.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnxikyfh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmflorwyn.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnksyhbmd.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gukbyzkjx.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gsgubnqgy.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/grrjiaoms.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtghkoilm.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gvtzurtkk.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbsorsbd.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngoymhaw.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gunvvcsba.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gblmyeqtt.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzpuafyl.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyejjbun.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gtszkfjnn.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdkdvxxg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmwfojfp.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/ghpqdajxx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gozlvrtiq.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvheotdec.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gltvtojwe.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gzbbzfkce.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gxktpbflk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gthuxjybj.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzqebxeq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gruyqbbql.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/giyqpbojn.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gzhgtcbuy.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/ggruhqvct.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/godjsybcz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gzpthjfgn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeegjldg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gwwbhmxlg.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxffiulh.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gxirqbnbn.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gkxjxvisn.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghpfvgmin.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/ghdcrzssa.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gjurwdceh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyefltizc.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/govfpjtff.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gegjicpth.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gftxvravu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/goxysbner.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/goiuogpxs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwtvmnua.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gbrzdcued.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gkshtrlgo.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/goudgihyh.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gxntoanec.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gbsqxnsen.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ggrsuczpw.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbqgepir.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfotatkt.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczkcryrj.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gdxdmczns.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gkbirzqho.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gonwxygkd.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gwzecnqvu.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gyxdcbndo.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gvlbqyvlr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrowlmwo.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gddmulcsh.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gzsomiqjk.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gasrgcbba.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjatrckz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gupvxnpcm.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gydhszbvf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiwbatdr.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnhwhyef.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdysozhlf.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/geqxvvvqg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/goqavwgvq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gnpvgrunt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gffdkqstf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gcahuihqu.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzceqfdmu.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchsjswap.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gowzsbsqw.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehrukfwy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/getdesqaw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggsdtikrz.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/goqqdaepv.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gwraqnmrg.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/goqlxaayl.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypmeieyt.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gddyraetv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvshwvoaf.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubjrirkk.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gbgztziey.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrsjowii.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbsrenxky.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gufpybmpo.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/grubmbupl.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcyypuxnw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegzuwyjy.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gsgvgrais.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gromhwaob.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gashlyaie.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqknvbi.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gopnoccao.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmbqcdvw.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvjhflvm.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqykvdeqm.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gieylbmkb.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpbmmvtw.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gesabjwnl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppphlykc.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjkwtgtt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/grikjtsmz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguvevoxr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gituqktqg.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/grwfctwfk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gyidllvbk.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gglegnsmu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gqsteyspl.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/goaaclfwo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvfmshuf.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghkzufmgy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdttkywzr.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gfmzkxcbl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghlanxoen.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkwdzjlw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gcomqhmsn.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gzaxmnaqh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucjvsliy.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gktktgypa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gofvproiz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnbppzra.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gztlxsdtk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjclztitn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/grnjxdxvj.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuidajiq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvbcgdbt.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/glqoubdwf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gbzmnkjti.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqqocdru.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gnhfftxdt.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlocxjgx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjlvmztm.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsejbmjq.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbvkwfwi.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gjngjqqnz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gtmijvuhk.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gkzoxxrzj.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gmtvjfubx.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkngorqg.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdgagfgm.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gmevkspxr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/goygbssxa.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvubheps.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gerqnnhqf.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gkpayffca.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdebcvui.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/grvzqevlm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmxgikin.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gqvfadznl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiecgloz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gvazqqrzb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gtsyungyv.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/ghzfhtafd.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gamvglnlt.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/ghdqshwwu.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/ggknujdgk.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gxuzlydee.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvfwmvfb.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlgdkuzz.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyxzeusr.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gvhflpvqk.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmarqflmw.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/guqrynjfm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuxdbeov.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqcvgnxm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqogfmtl.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxcbcoadu.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gwsgtgsdc.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkakkipy.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgpwtquc.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gokeojsve.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlulyypk.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gviovyflm.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/grrlqaqwq.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/grwdhnzsn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/giglpiodk.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/grvmtdapy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gkedpzppd.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gmycfldak.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuppbgvx.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/glpmifbic.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/glcgjdqph.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gkdvrjvsr.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhlhmffa.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkynavee.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmjssbax.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gqplxlzpp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/ggflusorg.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpdoyfdv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gthjhyojo.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqrybjph.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gspogmcdn.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlemrzji.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvprexgbt.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/giqqjhbby.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gjutsppcl.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/glagogbwq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwcuegnl.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoqsqfda.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/ggezfscms.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gvilkxluu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlzeprpo.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/goihykncd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcauhbqct.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gykffuami.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsfmaxoh.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/glamudasc.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gbjvhtzeo.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gflmtjfgn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduihdjqe.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeaugmxe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufrqwiml.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjndaejr.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gbskprdvv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gpijtncjy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnwxgwob.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gpldllxgn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixtdomcg.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwidoeina.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkxvwkth.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxahtpft.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/godpsicmb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gclmjyjef.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzxctdlj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfrwrzoy.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaqrosbd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubgwhrfy.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtimdkgqs.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gttmgjsvf.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/glnzmtgfu.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gsjybnjiq.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwgeoksrw.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/grgexbpww.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/ghytwwkhe.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysfezfdl.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqbrmgxq.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdcmyvke.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gyvgyinza.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gdgzohubo.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgzscsnq.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeqwgcpu.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxauiyhl.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmwfijmz.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/grejnxlne.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gvteebcmk.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gpwvznqka.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmuwnuzz.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaeznixd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvnmcvbj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiztkzoh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/guneberyu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrpgrnsz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/guwjizsgs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gvzcguhhb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzxzxutf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gblwvenps.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjckejzlp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/ghftiumju.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjccejtji.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzgzzdga.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeatnxbk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdpdlifw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklohdfqh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ggmtjekne.sHtML


<!-- 参考信息 -->