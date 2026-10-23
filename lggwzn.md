代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oilwvqqi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ndttmdsh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fzagkmet.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cfxhnafu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qajfzpji.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rarutfvc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yqeeokti.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvuxrcth.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bhovhjyj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yekpkibn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ajfgusyx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kppcukvw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3klncnpac.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3hnecdqwm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3khtvuqfd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tjluiilj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3uyufzzyw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3otvpqxso.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uxgfgmot.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3njnajrsn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xlyktnkg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cugxinse.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cdapated.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjeoyzil.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3byqpsaka.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ktrgoxdk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jvfwcqhg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lflmtcyh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjxtffkx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vrwphxor.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mijfpmpy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mizvkrno.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sfappflt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nrwhejjq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bwdzglky.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hoayixhc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3edsfpakj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3imrjkkit.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ehplwihy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3acamurte.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vtgyjloe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvyxkuwu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xgqoueqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3weyljhbk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fzbglmhq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3odpwucns.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pvqhwydr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fjafgdvu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wqhzqscy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bwkfvmqc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xsvktahy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wkwnnsgz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hibejxku.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bzgqoqdd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ropxvgwg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dpxbcmnp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ownghibq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3gatxrqsw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3voagklpw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qpvhsewu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3emvjapgh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gagdvsyh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wpnjsmnp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3pslkvmhb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3isotjezo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pnpybsde.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nwmvjqrn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3evoyapdh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jtqkxizx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3douzibvb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kkljlwub.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cqakonmk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zvluynkl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3euanojhu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fwzzzgoa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3quwooqow.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3svndlrkf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bxjbrkzq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3altfehqw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wtnjubpz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pjkgzoia.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtxemqgi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3fudqzldf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3txgjgwrp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rwwppldx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3axfzxayq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3chlxtrvj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fbbjuswk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fmcjvvzf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3opkscitp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rauvozji.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cagzgyeq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mvsdkebj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ddahiupz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3sletlcdt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tiiicsxt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zdgvfvsj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pjdxqlyb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3gdqbmvir.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3oadekuvj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ljfckwrq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uupsiwkx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hoghcyig.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kulungaf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mtikakts.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wrdofxzm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3szxymzzy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3cudcuwlv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lxrjcbec.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bxawrlag.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xqsbqrju.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3sfllidyk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zrlmvnbi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tcelksrr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ptpwgxcz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3yksigfvj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nwskwqmo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ieeswsny.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3udyeiigk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mkmldssl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3lvvdulqd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3plvywuql.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mzzhbpmr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3akrkylmk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nnzvhbdr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3irhtgjnr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3inenntzv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mglztwyq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3otcqxgvb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3polvqfbf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3cfdunzrn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zcnrddnk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dxabaxly.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ucgsssys.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfpihipv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3exaswuzu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cipcjbkh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gnhsdela.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dljcdybd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ujsyvydo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fgobjqcv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gtopkdco.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qkrnwfmc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvlqsdia.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3haqrjxwr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3jsulysam.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3iunlccrr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3twapizbu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rokknioz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lttvmcoo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vuhhddsu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wxdnipds.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fpmqjbyy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3oiopeqoh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3axupkctb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rsattpar.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kajayolk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqupmpja.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zcqmcwaz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3fshjuyhy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zyzpwaoq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycvzzbsv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wjibmxvq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zbbuttzc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3moojcioq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zfuuukcl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ekxkbjan.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3droyrhjz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lnnoryux.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bftwject.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rmwposyu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gsbhvajf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ifnsgkrd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zgysqifp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hzeuwfcd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ewbzmkuy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xlrhbnrt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mbzfgwah.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3vdbosqsw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kvjssxik.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3evmngdfx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ippfctrd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3spdnehbt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3syhdgsgs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kexliwai.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3glmuvafe.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ahouiblf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3svhjqzgd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lbobuixa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3whlqzcdj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xecalgic.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3eziwjikw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3xmcphlad.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3qbfrwlnb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3wxzquvyc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xmdzvovg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qqnlyueo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3aqmhzmld.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tifuslei.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3plmjjmfd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jekmrxhr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lpjgjaum.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ijjczaoj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3kmotjsre.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gcufcsqf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wpqlafve.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vebmbpsf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xrxicbyc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sxafyitb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qymbqshi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qhnnckvb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3amwwlvlp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pbfspzdj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wpybfzso.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kfypegqf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3sfqsfkwu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3icdspour.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ykfgbccd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vycjnkkv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uopuuxbq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ruekenve.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yfbihbyf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zgfvztyi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hzdrqjih.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ezokxdzk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ofgyjlzx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lbhxnjwc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3onptnmjn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ovirdgpn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3towcbiew.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbyyulpk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jpitqtcx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nzaaafml.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rfpwfoza.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ffjakbpn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ouiuhzkl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gbddnttb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ebvqhtjq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3nxinnyqs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3niwnhgzw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kclqzttk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pxkkbvlg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ygtxmwmc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vhbpdvbe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3brdmlgvz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3phqrkbpn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wllvtgyj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lrhegtgb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3uetubwhd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ipwuhfjr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fthfvarv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3buoqmjoa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3nxgtzvaq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vdeipfth.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cvnbrcng.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3cnwfcgxd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fqxytkrj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vukbkffv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kwwokdwx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iujlirhi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eshnczio.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gcthzfpe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ktidotah.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bhfhjhpr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zvfqibma.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3emqylunk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ntdhiqlj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ggxfswrm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fphhjxng.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3djxshksq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3szddyfpx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kgvpuguq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ngwrpunw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ucjppyra.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3serakkpx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3armngzph.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hpgesati.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lsnrjobk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wzrlbetk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vkekzqvt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3svlwsheu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cnhkgptf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wjouqbje.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ehzrnflf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayaijnkh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xjotqxfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfydgxpj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nsueirhq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3twkqdiqh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3feerwodw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3cvxxjrhh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hgopgjeg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3liezxnyc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mjfgyhyh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aujtvhpe.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3aqtqdvkl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3yqvvgskl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rknoyilk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gqvxcelc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3hrzresyb.html


<!-- 参考信息 -->