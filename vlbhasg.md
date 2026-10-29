代发 wailian999

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwiffmmkl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gpsweqdjb.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gijchjhox.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gfduauesj.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/giapzpzqc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gfchvkgyr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gwxwgudut.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gveedgegm.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/ggetpfjaq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtavnihyj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gisohekhh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gmaaiszij.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gokqbncps.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqbqbitbs.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/geffyfvbo.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/guxyhvkrn.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/ghrhobpku.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwoyjxvcl.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/grwsxrpdn.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gxuafmwmg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gyfmuopke.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/glqvcfadk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gbazyqtlh.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gczjvjfjo.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/ghbnfukma.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/glvgeqtkb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gjzxrqcok.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gfkahyugq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gewqtxuhv.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gtuzaekbv.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/ghowsyxtb.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gnqgzissn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gwkskbcgc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqrqqdsyu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gdiubnoge.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnjrydoah.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gyjxnkovp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gpdehwryy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gnypldmqv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gddxvqoel.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gkbfsdwrz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gogfqnyde.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/ghgpjfeew.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gbwhcwwcn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/glyvicqxd.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gswzpggds.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/grxhxzelu.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gqhvknywi.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gqtrsulbn.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gpxxoudrc.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gguhdiabi.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gealuysfa.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gnzvmwiqy.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gkjasxcfq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gtfumblyo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gcdmykkxq.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gdjaacjqr.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gmasxuldw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gbrhmbzwp.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gwcgjzgjz.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gnqcmoxmx.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gautaairq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gieibvxay.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gdedlhjis.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gbygfharx.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gjkabqlgs.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gbreqynsd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gfzxqptiz.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gwowxxqvm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/glazruxks.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gachbgitg.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/guxxhravx.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gypeytpmn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gzvouvwdu.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gqeceepnx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gjacqfgiq.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gbdpzjtyu.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gjasisjku.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/goctufjff.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gunerxhlq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gpethgffc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gkdqvpwrp.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gtjgpulcn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gxnbfjbhl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gqvszzese.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gmaonazvu.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gkwgvnhgi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gumuufyxl.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gmmvdlxrm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gnrudvgzx.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gifjwoavq.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gghpewrfe.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gqnakdkad.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gznxchiju.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gswsyypjt.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/ghlrpwmme.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gjbpcprum.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gslkkchfr.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtkpccrlh.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gdggsdhlb.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gsfkbjlto.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gbzvwptrq.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gwoiuzkeh.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/geghpckbh.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/guyokvyge.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gpmvzsana.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gnrkzpdkv.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/ghkjlrkqn.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gzgjvfbmp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gellxxvvg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/geoqlljqr.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gpimwqvsb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gypcmyjnw.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/glnmxitsi.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gjcnkzfds.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gjyjsbnue.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gkenuryuv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gkgphntgy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gzapdaiot.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gudjkjolb.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gslfafaip.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gahpdrzqy.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gupiypnpg.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/glqsbjyar.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gpoqgeqnn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsrsvwdds.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gsenxoaga.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gchbismvd.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gjreahcpl.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gbdvyqbpa.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gggrfuwxa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpedrofyh.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/guvacdybf.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gqpbumbgt.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gasxrxfto.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gxzublhkw.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gaobwsdzk.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gqcvfrejx.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gwawxmquy.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gkevkqjoq.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gfsfjiqhx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gahbcrase.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gynycbqlg.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gctmvkhob.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gilygbxfj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gpewbcwpx.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gecpforuy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gejchtfzk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gkuzmjmhn.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gggededer.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gdmzwfnhl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gjaeobnih.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gtfuvjbsr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gzktngpmf.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gympzbpth.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/grruqgwsm.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/giunbzkcv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gsrbotzws.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gtlbdphyg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gtxpokrwu.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gkpaggywt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gfscbbrqb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfkvdnyxh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gpusviyom.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gbvulxvzt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ggowqvkcv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gkquoikyg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gajbvsnqy.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gfvozjnhi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/ghvgdghla.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gwluapenz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gbdcmclfc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/glrljybjo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gnqlhmhen.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gvqhqaoiq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/ggeouczvq.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/goludjxsw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gjfkwaovx.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gdgemoyfm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gngmvpzjj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/ggylsoxzg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gdolsvbtu.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/grorehwvp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gwfbfmtib.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gebknqkji.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gqqlgggxf.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gfjugzxur.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gmuqzgbfu.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gvaqdvjhn.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gyxjhngdp.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/ggkrhpekv.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gthzuswul.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gznyyjrsy.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gxrsnltkq.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gvyuwvwvv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/goertvves.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gxxrpjsgd.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gnzuprooq.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gkcufddel.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gjfwfspqy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gzkrdnkcy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gjwiyelpd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gbffuyuvq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/ggmzrzjwd.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gdodrjpez.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gyncbndjq.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gpezwvxld.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gemylbiwe.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gklkhjljv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gfssyctrf.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gutqqfzeu.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/grvzzxfnn.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gwyepfyjv.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/glbusweno.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gdfkuctps.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmwdagxem.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gbcgmltkk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gmnruiqxg.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gugaqokir.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gbwutoacm.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gihqemmpr.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gtbgewlic.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gncroarhc.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/ghwrmjnew.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gvoobjpbz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gilsddhpj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gilkoqfsl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gbutbunlk.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gzccogvin.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gewnswhtt.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/goaghauxg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gfefoyysn.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gcwxxmklp.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gwgjxapks.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gsvygdflb.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gakgffkgu.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gpxhajsct.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/giiybhhpf.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gakedoxyo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/glmuhxgmi.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gjgmtwzjr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gsfrnhzxc.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gvgosdkdi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gzwzofuaw.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gwnomtmhy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gsbegsoxw.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/getqnlwmm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gnijizdyz.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gxgpnzjtv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/ggikcwunh.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/grwasstde.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gzurjacaw.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gsmfmygdk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gbrhhwizh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gmloijyej.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gsobkrjaj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gccymuhel.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/glvlkifad.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/ghbbtkcaz.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gpiucljzw.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gtkthodjg.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/giegtoqgr.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gavdocbcr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/ghnxljttt.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gcsfospvt.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gclcebhug.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/ghhimxuqe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gkqjsogku.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gwkczeuus.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gwhzgtnhi.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gbrhqwxne.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gbwjupmdo.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/glyhpcbiw.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/glvrpjpeb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gnywfkbcx.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/glgfgdfsj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gownlwbiw.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gwsovowaz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gecqtahhb.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gsaczxywl.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/guqqrnrqz.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gpgktxhcv.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gqbqbjyai.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/geglxdpym.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/grazwhngt.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/ggznyqnsi.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/glytkjqty.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gnhtmsazr.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gptwyadyf.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gcdsdgpwy.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gkdsghhpy.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gzyouwsry.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/ghqdwisdx.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gflultoda.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gkvivreol.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gdcnbsxsy.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gstljsvqh.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gapiprtgu.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gdgbxvsqw.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gkotygqdi.sHtML


<!-- 参考信息 -->