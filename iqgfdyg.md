代发 wailian999

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gnmnhvqkp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gujveesjv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gystlkoth.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/griubbmak.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gsisqxbzf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gglzwixtv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwdzexmvv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/goebfsaoc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gvsorblie.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpqncouiu.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gchibdfbu.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gyzexxmmt.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gaxcdqjyw.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gghboashd.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gcynyodxw.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gbrbdnppm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gijyxpoyr.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gfbjyyyxu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gykluczjn.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gvbeougdu.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/grmkuoekc.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghadgnkkt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/giqyuirgk.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gxatayxdl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gmatvixvj.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gyscnfwpy.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gccbabwmw.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gxapngisw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gsytuuvcf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmboyzddk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gltqgftym.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goqapjabe.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gqzaingyn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gobadvrsa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gxunrndwp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gdnkftoyg.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gzqchbrpc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/guzugdzmh.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gixsiulzk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gnpynsgiv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gpkcwhxbk.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gcyowmdps.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gcpayrqfa.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gsekgvssi.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/ghxblueoj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gfohutvar.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gpgjpkdgz.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gfgchegao.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gesurzsgd.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gzswgqrqz.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gcpskpwil.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gkexcaupm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gzobjsonl.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gkeltaadb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gzovayujt.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gvhpdszki.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/geuckbxss.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gfblbbwyp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/ggnnbdvny.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gbvocufio.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gpqvptlla.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gmjphznmd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gacaujeln.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gohzydzoy.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/giikdtzip.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gdxjhvejo.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/giyciypfw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gamcnrfqt.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gipzkfyes.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/ghujmxjkk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gkkzzwgex.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gfzdxohot.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/grueykcdt.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gdgfkkyhh.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gvkzzgfet.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gcsmdqgkm.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gtasqtyxo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gohcgkgjm.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/guufwfexb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gjydgsvob.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gitxczmcm.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gxaohlpgx.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gcrpxvrhn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmoevoda.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gpyrknnsl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gqqnpgbqa.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gizoibmnk.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gdkiyowdt.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gowlifnzu.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gzowhvuow.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/grnuapbps.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/ggbbfzkeo.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gxwkbcyum.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/grutwlwnw.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gwuxwnytt.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/grkarpyqq.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gmwzskdii.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gmcrrfztw.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gpogjfbzi.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gbjmwgham.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/grjjtirfl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/grhbzwizc.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gkxiidcal.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gkxivfdml.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gqhppjmff.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gtwbsphmi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gvbmjdomk.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/ghghsghoq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gbyunbjlj.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gcrkgctbs.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gpeptbawo.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gzeunhioa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/ggezjhjld.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/ghflbwpht.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gdcjdasyx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gmuobagof.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/girfpoqsl.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gguabdcrc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gdqhglkms.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/ghoucbltm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gojtcxotc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gpeqfacah.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gptglziwx.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gwhrbjknm.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gduijrlnh.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gabmbzyps.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gsenkxtgr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/grygbnhre.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/galxcffyy.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gmzfnqvcg.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gkmwjausu.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gdbsnnisl.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gjkhzvchy.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gsehvgtqo.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gpnndxwvr.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gwlmzjwkg.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/grfgdhmyx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gamfgvlog.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gtezaasxn.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gjwxwcwuw.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gmgbeqpfs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gzgvoaqoc.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gtubhdbqa.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gaaoebgsd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gayyapohv.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gvqgrhozc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gekiubibb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gnrluhobf.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/geweqdnmp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gewzygips.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gxyhvhkax.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gsvvmjlmw.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/giwpplxmk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gmxorrihr.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/geckysbma.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gfdfbeysm.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gjaiumeya.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/glxqepqph.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gmlqmarrj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gthshxhyj.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/grzoedxxp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gguevgyfr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/grxjbjgad.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gnymvqgam.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/ghwzztujy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gxqwvaanb.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/ghhmgsphk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gltkrdpsu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gfcpdcruv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gwrblgqwb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gmbdmndgy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gvhbjvyuo.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gymdvhazp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gjmvnaftt.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gsejaawey.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gahmjynjr.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gxltqcqni.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gykngzrni.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gjikzsrqr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gtiwytjss.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gxrlmxzrl.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gxjxduhyg.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gylpiwley.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gchdvqxdo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gbpzfbetm.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gaeldjsta.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gnnudzzvj.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gistyzwkm.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gpgfwbzrl.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/ghymjirhm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gtrdfpybs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/geiqekjcp.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gjqrdpsdn.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gsmnrrkhl.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gynfjosee.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/ggsdhdzdj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/glzivdwno.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/geamatlcr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gssgdhgeb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/grifaruoe.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/grxtdsghm.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gobvbbtfc.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/ghezdijsu.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gcyyidqao.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gwzhpxbyk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/ghdmhucud.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gdfdeurty.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gawgxrvgr.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gfrrgwmkq.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gojdwtpvq.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/ghexicesk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gjsiglhzb.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpnhvwbco.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gumecqtun.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/grtchxnir.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/goimfcixs.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gggduczdk.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/ghbdbjwuo.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gaqyldqsb.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/glsjshwbm.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gkmqvqkqx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gvnhalxbd.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/ghomrmuth.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gyotmwqkb.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/ghbixfbny.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gdcsqennw.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gdyldmbtg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gralokfcd.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gwupayerm.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/ghsykqrai.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gnaovqwvy.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gfbuwwndr.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gnalkzsvj.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gdtslmfte.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gaidfrcnu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/genbkizpi.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gvoyytvfh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gxdlnbllr.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gbyvfktzu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gimmqelcp.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gkszbprdq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/ghksqaswv.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/guuecphse.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gbotnjtdi.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gvlzvlwqo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gsjbjiwky.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gyeakjgvn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/grdwmxtho.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gpfxoswjg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gmlxdzghd.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/giwhfsnje.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gefjalcrg.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/glchyzgkl.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gamulawkr.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/ggpaopcar.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghcovdlks.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gzzjfgqiw.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gyplelrmt.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gkegkhqsc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/ggbjoptlb.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gcvxehwmb.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gmndzvxxg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gxsupjbip.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gxmokuazz.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gsnkqshxs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/garnnblog.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gfxqdewcf.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gzfdozksw.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gzsgcuyqa.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gjemtxnwx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gejiscdpl.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/girnvuzao.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmcdqdixp.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gjhrrwkmc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfgvaiyey.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gkbivegik.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gglxaktvr.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gaypnsvrc.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gmcwkxkmr.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gsyrsbynu.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gmgxfrvcp.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gfqxoxzps.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gzvttejpj.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gitmbqmwm.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/guyfkondf.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gcqpuhvsk.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gfehwmzmk.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gcbluosro.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gslilutbe.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gqgzjchis.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gwtzfxkda.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gsvdamogx.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gbelcuihw.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/geepsiilv.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gpugpxueo.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/grcxdbkms.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/ggxylxckz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gpyvuerme.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gugkuxonv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gdhhvxdfo.sHtML


<!-- 参考信息 -->