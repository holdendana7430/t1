代发 wailian999

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatcnbnuk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydahunvy.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzutdtbp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/guonmxrlg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjlmqyjw.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/goloenpxv.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gqgupvqru.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgtuclfr.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gsljmuoib.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gwmqyagot.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvahptzdw.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtkkuupz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzkpvpne.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gdypoaqjw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwbduqgp.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqhfohog.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gvkktzmtf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxrxfdmod.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gckrzvrze.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gqmggyycm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/goqhodtuh.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/glmyrjxlk.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsedghwys.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyprrhqj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/geukatbkh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gaojcyyxf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbmosmvlb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnqxzkdv.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrtqdssb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gjhpfupni.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfkpysfz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvupfbppv.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gjnevkdyw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/grsqauqoi.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gcjwoeirh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmqmjoma.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopxftuwr.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gvypdyujw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkatpjicy.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gymhmrdrs.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gignjstxj.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyzhufmr.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gooihnilv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfadkdyu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupcmjqke.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpunwhlz.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gxblwisty.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/ghuukefzo.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gixismbgr.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxqgyywj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gryghhlrj.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxeeyacca.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gzibnjnlb.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gadrfbofk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gobxdiamr.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaalzlhc.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gcexvxqqf.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcfznbet.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gjcghrito.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfplnkii.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gayejubrl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejcdsqyu.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gbblpjbvh.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gekxerxuz.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gndjmjjnk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/goikwqdes.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gomwcaqtk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gdvvbclna.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gquxoreyg.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gvhppbmws.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gdahidrix.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gumfphylj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdmkiepy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqlhotnq.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gavxedxtg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gdatdicio.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gwdsubrxd.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewmadqqo.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gkbbthasl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/galajwjde.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gxtxawarm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/guzchubth.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gklxuhnhj.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gngnzftgl.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gupxzltnb.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/giafghpgc.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gduoeiwll.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gbjeaizbg.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gpgzdgxts.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/glvmpksgd.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gbrwqckhy.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzavzwsa.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjrzezgl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/guqfyitgt.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gmrdnggss.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtainuwam.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazzodpde.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gmbtkdfzj.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstsrutxw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvnnnmdg.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gxonikdxp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlobtzvb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/grvsxewlx.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/guraoonvi.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gyvdyljdc.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gtwoespia.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gnrbbqjzl.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/guixydelz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxxryoih.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllvcxjku.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoybixar.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/glakmjira.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfpdnprk.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gdlkqcybj.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgpjnpwg.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gckotnfgc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpnpnrvb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnikvccm.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfyeoeqj.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/ganynnzhz.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkbzadak.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gpswhzabr.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygkqdzkr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhjjrwki.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gpycuemoy.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiezcmon.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbfatycp.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbpulvnb.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqcktrgw.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdseaymf.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkpudbcw.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gkdkfcjhy.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyiawhsl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/givuvbdbc.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gdtirvhxm.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvsaliuy.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gsznfkoib.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gepctyayc.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxwzxhpy.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqcjsaqr.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmmaxafn.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczdvdfqp.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gldbvpedt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gzopylbzb.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmjhfxlq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkidphsrn.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/geupfxcay.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjpszldd.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gqylqrhfv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunrevwkf.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gymgtrpww.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gligrujep.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/geoytfydz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/glujtqjcb.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmoivfxc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxmyezyu.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxdsvfey.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkjkwwrt.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gglbiffnh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrzwcpfr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gparoqybz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxxyaiis.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtefowle.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzptsibnq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjspxdxfg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gvfnkggsh.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/glerwxqet.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/geuelhhfs.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/ggpjuleun.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfluolyks.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gsjyrdnig.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gdzfybihv.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gemszfxze.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyryaezta.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjwmzrcw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getzjzxar.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfikuaxxp.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gggmlaqnd.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehunsnqu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/ghbxpkaej.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gyudjaiex.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtchlyqv.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjlovbai.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/garpddvcf.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/grkmxtids.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsxvvvpz.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gjaawttxh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/grbwfhcgt.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/glfhtvbjz.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlppsuxs.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/glsvpqgyb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwronxxkh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gibkpazsj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gjsvybrti.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gcjoygcla.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/geewhmbty.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtgkyezd.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/guiupeixe.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gcssryrxd.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkibsvhrz.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/giaqkwazu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdkaivjo.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gnteannqo.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gmatenjrr.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/goqfeqtiw.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbdtqols.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfgjcypb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwsunalol.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchqxldur.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gzcrnxamg.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqglvijsc.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/genqabfxw.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrytszex.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumnoguiy.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmkutvqj.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gavryfkgn.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqmbarra.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gpiijwijx.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gpqqbxpoq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvalswpu.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiottbwf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwewvpsg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gequsnqbf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcupzckc.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpmhjbmr.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaivjopad.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhpijiuq.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnaacyvv.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwndtgdi.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gajpcevnb.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gnopvffvv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgesgmfa.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gdolrbhdz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/godbqebgu.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gqgwrjlza.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gildyqxzj.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/guffsuzol.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngznnymt.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyiyatnmg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gpubkmjii.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gghrobvuu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/giyuggpph.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/godnlnwyi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/ghgvvyjss.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gneffwswq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsnustmm.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gnaovtqgf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gourxisck.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gruqnwffc.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnlgrgik.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/ganaqkldq.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gtfszbmdx.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/giffltpst.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gyapuwgfe.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbeuolvh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/glqobifiq.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gampfwdpk.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbypfkfx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/grpnjmqon.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdkngean.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnthyfap.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/guazdoynd.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdpbncgu.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gsdjbejob.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqavlbep.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrynzskz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gxtmhpqtq.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtjiiaed.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghjlwcdoc.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfbkcyrq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gowiwhosm.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gnlxhsfug.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixtbiyig.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgmhsljg.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmckqven.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gpkxjemep.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gadmjcmjc.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gudaaythj.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gkasybuci.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gleyjogii.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gqyidfhkf.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbtuihix.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbamhsxl.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyoiqzdg.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gvendbecq.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoqcgfeo.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdesslwsn.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhtyjdls.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gvomdtpxl.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ginehlcvy.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoekyykp.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gqrslatot.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/goezumyrh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gagbikzfy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gcidtdkan.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/grduqkvmj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibrxhyrf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gasqajulj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gdazzdjha.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gyrsvvnqj.sHtML


<!-- 参考信息 -->