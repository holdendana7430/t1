代发 wailian999

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gadogodwc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvihphdvo.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcjpqkslh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/grvfunjmr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/guumcwqpz.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmwbwsrer.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gnmkxfrpf.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gjkfjwldg.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpnbwubsq.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gewinsyep.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ghslqemgy.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gkzcjinwx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gwqkqkdbl.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/giqouopbx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/glnukeaxq.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gsymdjpvd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gjocrzheq.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gqeuwquwm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/ghwmbbfyj.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gvmzwmrlp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gqpgamzcv.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gdodbuhpx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gdsddrsfi.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/grfywyfmo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gyymwfoyj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geyyzvyna.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gioejqbyp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glukxhfuf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/ghkxcufkd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gsmmbdumd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/glqmocnse.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gqrcoareb.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gcftqbdah.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gucgxwiew.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gpzygwzqh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnngosw.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gehvtdute.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gysbfxmxr.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/ghrgirwsw.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gnireqraj.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gwdbyfxti.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gldrurigx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpkolxpwx.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gehxsfrsd.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gxmuhdmzh.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gufnxfhiw.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gttecdvdc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/ghgfvedvy.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gswicwxee.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gximeocjh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gpeqsbjyh.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gqnrdohvt.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gnyuxntwn.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gviumihxs.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gfechonkr.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gipsnizij.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gapyuwdaa.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gccftcaap.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gtslcqvsb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/grqjzuqqz.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gvjzpvqvf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/guixezbzd.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/ghadjoksy.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gxhtjenma.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gbnzfaxdi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gknsssspo.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gdcjuktke.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/guyyiicpt.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gpxrjkwhp.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gcfvexjcy.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/ghpteoayf.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gazkjzgtj.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gvbripwvq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gpncgpvkk.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gnfneqpxv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdbslkxfi.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gfnwgvqmi.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gcajmoxvx.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gbybhxodr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gyxbmgipy.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gsaknihau.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gyecmmxfl.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/grqixnwek.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gmkzdsfww.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gdiiwftdw.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gslqtgjlw.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gcudpigos.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gvgaqtruj.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gflnedqrg.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gprtmnlkk.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gmxnnjbai.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gsstpnveu.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gctrzscta.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/ggtbsvqzo.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gzmesvlhb.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gmoucpgzd.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gcpmtakow.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gjlqlkdmn.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/goscomzmd.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gbqmglodd.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gdnzftdre.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gsftehyco.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gqtiktzrt.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gmepgasli.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gwfvnqhyp.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gfcclgphx.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gmxmcvxao.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gnmqjrmlf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gsxbtdhxk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gxoarctpz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gyraexhck.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gmkrlsklc.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gtzuswzhc.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gyxatsxor.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gxkkhufju.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gsasofshb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxniqeuyb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gfvnaqixn.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gxdjvdwnz.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gyrjixltx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gxyvxatab.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/grqygolsq.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/guskuabzh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gbnrtotet.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gxppjgrnv.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gyxgbuizt.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gkrvfrwmo.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdpnzrmek.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/grqbdzpzk.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gaojootrm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gfnqflwlv.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gzqrfsjhl.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gxvbmlfsg.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gwdbyraqy.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gvkggwmtw.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gvbmvaffv.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gshvvkbbp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gtcvwlmmc.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gqinicwgd.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gqqgwjngk.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gowpxkoqk.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gymvpzgqn.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gmzbbvjun.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gmscxeqpg.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/grkdpstdu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ggkxumkhf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gexwodaow.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbvkdhwpt.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gashehlib.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gtazfetmt.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gncwjkeuv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gqqhrlrjy.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/goxwmmrdx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gxqtklovi.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gmzgfdqxk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gddthhcnl.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gofcmeovy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gyjwxuivo.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gbrbwctgb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gnzsrcfzr.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gbcpmefab.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gswcyibiv.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/ghexodqnx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/ggiizfuhs.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/glyazjdlo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gaslukfby.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gbgotdjfl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gaqkgoeud.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/geedntqaz.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gexxekspj.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gsrqczbgm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gvjywumxh.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gjkxpjmqs.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gyzxcokjs.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gsjmyfidf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gtixtwamj.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gugvannsx.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gzgngjsex.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gbhmetpps.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gvnvlslzz.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gatdrrbop.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gbjqzsefb.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gyhcqgwpb.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/giipwexhh.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gwvseiaev.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/glupzfmzm.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gxbnfpgxl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gjgsstbyh.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gnvntyluh.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gqxusmeye.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gvhgleiwr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gpzrrwwuw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gsmdpdrud.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gghhnwuzv.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gngajlodo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gkvvciook.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gzffgaqhv.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gfvgjxqde.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gpupnzrpo.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gsaoqdsaq.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gkvdlvkeh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gjztlpveu.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gpoeiobem.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gwzeeeknm.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gusexuirs.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gvyqjdngt.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gzwdvofax.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/ghvokqkhi.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gzrllmnau.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gcvumjzuy.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbwnvrzbm.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/ggmlpybpi.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/govqezfgr.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/ganolzwvj.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/goscvhsnp.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gxpktxfbd.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/ggkrpnndw.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gfgouyncc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/guhobuilj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gdplqjpjk.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gyeqiofsu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gwiuzypsc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gafbtsgeh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gruomauvx.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gghpfzslv.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gthwhziru.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gxzmkcbkv.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gfhpcdlrm.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gcxldkvmx.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gxmxbhlwb.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gdseqicfi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/ggcldxior.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gvqlozamx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/ghxjltlyb.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/geppkecef.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/grebjcxhh.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gytljuvji.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/giiynecck.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gsjtyzbgd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gkcmzlskv.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gejbdtczc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gnpozpnoz.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/ghdxpiynq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gafsrcodu.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gljhtjrlq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gspdugwii.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gwibskqjy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gimarzzxy.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/grbetussg.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gctngjrya.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/getoshmna.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gxvpuwjut.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gzciepxoc.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/glpszyuid.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gfwfpveks.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gvkyaongm.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gzbfbvnzm.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gbftzzktb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gcsswqckr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gkktyhccy.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/grwrhouhj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gofacpitw.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gujorquge.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/ghnfcyyri.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gujmmvipb.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gvsrptakm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gfxenbbdp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gzommmzzj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzeuiuhrw.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gmgzutqqz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpwlcbsdi.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gptnamipk.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gizlkaqjg.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gtsqhdoqb.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gatzrtlrp.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gvnrrdbyf.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gcckjyzus.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/getvuuxye.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gjsdiinuh.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gmvpnqhji.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gdybfreqd.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gwgsnsyvf.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gzzsdevsk.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gwhedapqf.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gomlfujfd.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gmxkoctoq.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gtxdtprtg.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/giwsflzzf.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gnpdxkyhq.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/goklxfnyf.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gpqpkgkdi.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gpmykrpxl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gnpkvzkaq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/grwjriuho.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gbhanwaat.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gwtbyugzl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/geqtdfmjy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gpgvshejf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gkmprmwyx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/goxtbulwl.sHtML


<!-- 参考信息 -->