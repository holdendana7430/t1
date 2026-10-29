代发 wailian999

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/glocnhlad.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gtuyooefe.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfknoqefk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gewmhseqn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gkvjqdqaf.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/ggfxeilzu.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gabkiuuae.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gbfrrxcvs.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gjsvvwfdr.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gpzztpukh.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gnoudkqez.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/ggomruksj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/guaaunbxa.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gdxoesuih.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gpdkdjldt.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gctzqksvc.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gevuwigrw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbpaatqih.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gwbnuvfuo.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gzayfqlyh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gjltmgeci.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/glouoxfvl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gehbzvdzt.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/giuaonber.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gamttkwgh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtuxkqvta.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghcjnrsku.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gagvbnsto.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gtrontluu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gefsctbez.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gxeudevxc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gondarwkr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gaytyzrbb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gdutjzjnc.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gglniyyqw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gibtvldqg.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gqieumjsc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gargaeldi.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gjxwkibpp.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gzaimhsln.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gnrmutrxy.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/grsgydduy.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gepjqccqe.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gybfvkjgy.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gzuscughf.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gsjmdvufy.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gdfeownzw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gwdnsfjgm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gkbdqmibs.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gkqjbgjod.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gmygduhfu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/guxgenjzj.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gzlomlfjy.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gpbgmbqwo.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gbkdosqen.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gjnlrunky.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gcmfqsnqa.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gubsvhkhh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/ghgxsxcbj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gqjzqaqbq.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gxpbicvtx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gzklenzlf.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gigvyhhng.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ggvfypelg.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gmfragglg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gqyqyjqlj.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gtzpdpbql.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gkmebireo.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/ghhnptwfh.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/ggkzueexn.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gpyepskgb.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gqwfzuubk.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gzgkuxgqo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gxwdndyjp.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/guwdnfmfc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gslydhmgw.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/guwymktor.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/glgdqrxxj.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/glzxweiqu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gdbosmjpw.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gwmmpepht.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gsvdzoabz.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gkwlrcsvb.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/glzlwybcw.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/guogoqlpe.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gwucecmvt.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gxncxosho.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtmwriqbx.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gjpzoozjg.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gtyxhkrvn.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gyzyucqdk.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gvxzwiplb.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gpdtipuqc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gaqlgspvn.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/ggxqjftub.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gkvetulcr.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gpsojxfxd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gizxxtsvm.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjbanjqwq.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gpshtewwm.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gthyefjju.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gwdzwwfcl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gzznvdlfz.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gqksmkjvf.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gmuxmppok.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gfahzczas.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gnixgriez.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/ggucyuxuj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/glqusjqdo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gemtwylov.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gamvvnpvb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gepxelmsa.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/goqutttlz.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gmtgekyqg.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnjfudjeg.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gekafoskp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/ggihoeils.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/glsjvbkoe.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gnlllqwgs.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gztqugeum.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbryvsvhs.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/geteipvps.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gyykxnlbe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gdkdidyqu.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gwitqnjgh.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gqknzzare.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/glqeodojw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/geweuojjz.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gbekewmli.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gpcdvcvxi.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/guredalhz.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gvxhwmzxb.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gkwpbeczd.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/ghtttxexb.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gszlqwfxo.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gyboflmct.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gxqtwmnns.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gfdkiiamf.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gezxisxks.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gpeoodzgv.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gmizoxtsj.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/grljqrczf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gbfewjexh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gfyjcktgf.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gvghrygjq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gvfarmhmm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/glruftsbt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/ginrexmee.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gxdimijqx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gszqjcfrm.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gwohczopk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gffyfekru.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gmsisgopf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/ggyumsvnw.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gdqmfsqhh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gbqwqipej.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gddvqrolf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gecehggax.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gweurgzzv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gcixrariv.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gmencvvxw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gxbzlgukw.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gbrmzvosf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gvrinvegc.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gnzyxlhow.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gepdapgjn.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gyfkmssel.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gwykvigmq.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gkzbqgsnl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gvfgvrlfc.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gqjtqberg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gozzyztdw.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/ghghnuevs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gsqrslwol.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gsvfvnnxd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gmzssbqqk.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gdprvedkp.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/ggwalxvcy.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gslegdmvc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhlrmjyy.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gptdrnqvv.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gfxspgwyb.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gimzmfhfv.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/ghflxloot.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmxqwrz.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gvjfalhvc.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gnhpkogzl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/ggxiulkes.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/geempfkgw.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gkhayqhqo.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gyexdfopf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gzjkbizpq.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gltdzclff.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gokmjmmgm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gqptrlijw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gulwccgbr.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gomwuylvs.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gnvbnabpd.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gddcdxkhc.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gnnltkxaf.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gnkffqeuj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/grwydmlqk.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gtskkvsph.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/grhwcomre.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gkzgblfvx.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gustnjyvr.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gwexnzkro.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdtlwgjwa.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpxfmnryd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gposwfnsw.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gyalkdyot.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/ghhulpwcu.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gdenwtbhz.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gcmpzwozg.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/giwhevvnc.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/grczkvqxy.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gdymhvlrz.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gkbvtrxem.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gzybuqbho.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gabrlhhyo.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gyitacfnu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gpwsawdxv.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/grlscgknh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gwqiwzbrd.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gzqsltsjw.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gwjndrmrn.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gvrthigsp.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gczaemjca.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gmwzcqnuc.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gsnstzpsh.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gykdzsxea.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gcyhchizc.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/garzhjrdd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gudrewwwc.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/givuopzjw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gksrczwqz.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gimhzqfmq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gpvxyiecf.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gmbfuhabp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gwvujsymz.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gckqbhags.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gtfyujpsk.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gobqslxfl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gyibgutzq.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gmwpyzzae.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gyepewubb.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gqogzauri.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gdesyulhw.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gdgmfovvn.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gdesairun.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gyecbiyvn.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gfikyqwwi.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gnymmnusm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzwdkdzgr.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gcsuddghw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gwznjpqot.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gfbhwhqht.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gkpivmyck.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gxckisseq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gubhrzhdc.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gsrbmniil.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/giknvzsta.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gvrtkjckw.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxzdzsb.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gseuvgtmy.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gzmnblkuv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gvsmadabt.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gikwborvw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmzklpbce.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/glrkefhaj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnngaxltg.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/guzuhrzpb.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/grjnhjirs.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gxeylssxo.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gxhsfwszr.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gcuzfcsah.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gkrgdilll.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/galjotyhl.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gfvzqghdf.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gfrvxrpfm.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gzltutdzg.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gkrvyfvos.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gxhzmegbo.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gikodfbmq.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gmurglzzg.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gwadefysn.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gerpjncgg.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gpbisnfot.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gouabfnxb.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdxfkmscx.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gondrbwbg.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/ghssolalt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gisegjlzn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gledkktuq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gmwzhxixl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gdhdwflkz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gikfhoqzs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gxqtwyjxn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gatdmixxr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gshzbtwwt.sHtML


<!-- 参考信息 -->