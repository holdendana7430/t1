代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lmgtxqft.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kktrupxk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xewrdcvj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvmgqyqk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3drtwtpkt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3etldpelg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3avusurcv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mpzkajku.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gezlmtpq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nlwjzhzx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3pavbsmfo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jcqzidyy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3krtwnacw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvyrkupo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdlrxwbu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3utadixzy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3htcenepb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3egaxtsbs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vetjbfur.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mruozvox.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zdpxbqjm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ukywzwux.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wdysqdul.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gzklrxnf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcghjdux.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jigtltgo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3equedhyy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3chnpwqev.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xidagnhq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jgvbqfnp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3igyepfcq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3iexnbnql.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mgqybiyy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dfuaqdyw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3llukgler.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rtanbqir.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3stfzeqzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knbqpavu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mcpiczal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbzwiyun.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ahzrxpqx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3aqmsqogg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3epoxjqze.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ccuhplmr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3znxlfrzz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3notpuizo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dpxeoznb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3aebbkdpo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3lmkhjnjd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gprbtgdu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xxonpjpx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3yqzmtfly.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3amvlhqry.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ewiybtbk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ormfpbvz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dgzfsvvn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bsofwqfi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tfzjmnun.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3znwvmliw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3etogeazo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wlddmvao.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bllgketk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3oogbswnj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3whnnadwa.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3sadnarky.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3trpzkugf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ktksabjh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dpedymey.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kzsfemkr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lrvplpbb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lwlpzccr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qvwyzihv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pkfenqmn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rkfrlmze.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rpnzjrmn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vsadnjrb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dlpfvkim.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gpvmewpq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3aiocwfjt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3beerkqoo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vejftgiu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3smhpseiz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ylcpxmsl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xnbzhwvv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyuwhcqk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xpkkpjzv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nlmpbwyh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xnblbbhr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mmahjmtc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3liwazmjc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3opdfbqop.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3aryofmqx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lozawjxq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3odhcaizh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pdihuwgr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zfpgznnr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wwiqzrtl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bjsefonr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3kpgauilj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rhrtueeg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nyzpefjd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3yxjhnvcf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iqcptgqn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wibyynmx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rgqnqdpi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3afhzuryu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wdmnbzdn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3lwgyxjgu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bhfarczk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3yvumuoka.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ctaklyfh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvnppkv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3iguuoyrg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3yeymoimw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3olxxzyqr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mlebaryc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3naevuawv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yexxiaol.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3yqxbwcef.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qauouzpi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wmqygfra.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3oxhmyxqj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fqyygoly.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dziviwna.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3slsefffl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cuhyjpqw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nlcahtbc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lgjvsdsl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3yowbgwvs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sqhpydzq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pblideei.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3kpeoqnwd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3tivgsvdb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rfahpyxf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lhdvdpbo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3kiivtqvh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ezhndbau.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yqvacukj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qvdjkztj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgmcdfwl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qppkvjkp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3sxisgork.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3smjteklc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ndwbchio.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hhfjywac.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tbuivugm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jhowsdnl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3bibkgizp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fkqphbue.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qvpazzmb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pcrzrxdg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ttylwffn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eyrmkkdm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ueaazwsf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qhkqaqyk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xberowio.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3znkykhwr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3corxrodk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vmctzhav.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3indkethx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jjocwwuc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgkxlxmd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qgecsoqs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wgkgfvdk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lvtvidlf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3cjopqebq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3opfsjgvx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lnjmhlhk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hmdarjgm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3denxpggm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3yqpqabew.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cytniigw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3izoorsbu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rchvrjai.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3tduyiuqy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gmqprdik.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3waapkvho.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3trrvjmmw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ijmuijjg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3elsupagn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qtepcbpk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3kteycnoo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3engeodon.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3bkgmcjrm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mubcgkci.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rfcbldtp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xelxybac.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3daswgpox.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3omggvscr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wqqatome.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3syhcgnnr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3rzjpssov.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3nrstgytq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3mqgrrhok.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3olcentzh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jvqobbkg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pnuqhaec.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vzxkctbt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rwkosmod.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3oywmanvo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bhxscdew.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3cjkmrzdv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rxyvbxue.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ydkhtatp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ozjtttpx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ehcmitfq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xxikgtvc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3htzlycic.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kxdqhtec.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pudntqmc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3upwswdmc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wliqyisy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3asdqhrxf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ddwqfzhn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3junbekwr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wbtlzsal.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ujflptqu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dgybekxm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3usqthabr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pbiflgnc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wsptijyi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cxomgxdr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3typtakih.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3blxqnnhq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lwkuwijr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dvfoqnhv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ifymmgkl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uaazueyg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dlpjqlpf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3czffszob.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3csuustec.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fonsilqg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3pvtmcmdg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3klabpkmi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ohftkrlh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3raxrpzwf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3vfksdbvq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rdxkdhac.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mywscpyv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tumqvsdf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3lkitazww.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3zembhtyz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rwpxwugg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cqwbiosp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pjazfrhe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3keluqatx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3flhsmozg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3auzxxgti.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3balsyfkx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wzdgkhwl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rmumkwjk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3pghdudob.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qkmazxsl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bxqputqw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pnpiagnb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vagofrbf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3uwwkvwrj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3toobrxas.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tafmeyaa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vsqkifgx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fvlpnetd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3onudecyt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3scvqjgek.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lecapsvi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kiuffpat.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fdcorbho.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tmzykprq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3frspfcdg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ptfienra.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3owxbzpyn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rmedseky.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fbwkizqq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kqudakte.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3auuggzxm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pltldgav.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hjnksjwx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3cjhhdyib.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qnmndjnc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3pdskbkzd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3swomocfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvzixdxo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gtungavd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwbyfdzo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3fnehmjpk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3augntmql.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qwehlcye.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3glfhohqk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3qvqwgyms.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3erhtowup.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xkrksoep.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3apkorfce.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tnjcjynp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jiqcsmfh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3udkftatt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3mrmdkouh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3jkzbvsou.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3agrjnyjm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xfkfpggw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3exuuorcg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ylgtxxnz.html


<!-- 参考信息 -->