代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cgogiske.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wsehxlwg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dreilvmk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guksgscm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kegzhskc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sfyiibvl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3aruzqfgn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gxnlsffx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ljgqosro.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dfcwudoz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rmafgjyr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3edbrhtmf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vsjvwvim.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yfzidhnt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pcxgwbjg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3clozgvqx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uktxwqew.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3veozworf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3udfoaaka.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3koonbqnh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fspbrvxn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hdocbmnp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jmynowig.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3latlqagk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrpbbqvk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3exjlmfht.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xnghnphm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jskyvtbv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wlmpcnfy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oefpgvhq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3evlalmin.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ncatxadq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vzppfdkp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3czhijqmt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tnboonqg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dyqiejms.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3uzfnoqnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mevqinmz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3brecpstx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovrlcymy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ttdrzbhn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3okfvzyvf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3sfxmzbig.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3sztlmhkp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hkdpbwvl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ubpxziub.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qzyupzpv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vduupmde.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kfgztorb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sxxswdnw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3evfhfmrb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3syegbowy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nxlhtffp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nnxpqzhs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3madeiddj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3goloqjuc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ezyqfbiv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3zmihqagd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3senfqwyp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3phslwfjk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3prhbqsbl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nfbkwllg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vtnihcrx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uqqepguv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pqpujgkd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qnhuojhj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nlyyommu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cexkepbu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vaqouvzu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3iwmfrrbo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rulbkbzy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3zdvasjxj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ptwnlxop.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jqskpvpj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ymuzvtog.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ibysqvcb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zxsoascl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsksqlh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3maildaoj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xvjlbukh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mrurtcyy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3djumjmaq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gcpvujoe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3knickklt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbfwgwki.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3nrcirqbg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lcgozurb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mvfhiwgv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3svymvcwa.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3svnkcosh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wjgbdqyw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3piytrlqf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ciciynii.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3rxifpclf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3sfakwkxh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xuqlnwkh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3jgsuvhna.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lbtjqgoh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hirpigor.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3glqegcju.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3cmrljxqd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xpwsexsw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qmfinxtx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ojsnfryp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zqlfbuji.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vxtposvi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qpimxutw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wheosire.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3uacdppbc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gepnawmr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3btattmta.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qewqpetr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dvxmjjhj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3iztnpdcz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zhmnxyzl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3llqpdfik.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jwgehlyc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dtrbzqiz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vhlykrxs.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3okgeadfp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ntddtbhz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3atpnwgqy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3pagtytph.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tjvvtrku.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dlysmzpr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3itrpsebw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3cdwhczoh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bpaqkokt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nvuiidxa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kgqpprad.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kjcrhaeg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3sdhimbcv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3toheulez.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cxgjhrmg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3qikbniwa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhmexocv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ykqosrjd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wdsybhgz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tgfzjzix.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3possnnfu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3bgbbrsue.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3aatfnqvu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dqbvnqdr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tbnlvszt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3npggfubn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xbtdgzgt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hcvrswsw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hbqqffsj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rdcrwxjk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xolvpwav.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wyortybz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ccrycqhd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xufkggxs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3npdwuqyk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ozylxota.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lzlcirvw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qcddiedz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vgxlneeo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3aekdtqzw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vxuecmbq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ogflwxon.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjpjikwa.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qhyhvdur.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3osjinlyw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3plybsoyq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vqrkgyze.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ovhckwnk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3naqtrxmx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sqwgtpmh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vidbuifi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xitofzyo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jnzbicat.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3pgezwiib.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qitdzwpl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cnlqzkhd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3debcgwpr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3kteypcoh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fdabyuwr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3cjncrsiy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sjojpkas.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qgorvulb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yzafhket.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3shwzesjc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3tbtmrpuv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nglblaii.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dnyswkbx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zhhxgyxr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vubqwbjg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gctvijju.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rkvqnelo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3disgoxkp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3utxaapsm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pvvacqfq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rvvejucs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qslwvfbp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3axaoxmbf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jdotrlxu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jdieishp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3psrplpzl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3geknrjnv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3chdrnlvt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qwtcjeph.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jkvxqrem.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ljjcgxhz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kcmfestr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vpqgsvqg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3tqylbari.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zwzlvsuu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vynttvpc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3iyqjuvcg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zecmumyg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hpesdakj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qsyayujp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zpgqykoe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kipdndvb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3szhfnqhm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nggbmpur.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cflllcqt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3krzjhbut.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pckbiagh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3uxvixsvl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3slitfsdm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dqrxdman.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3idluvkoj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3yvaqvzzq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bamhvmxm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxvfmpqq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bhtxfawr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3sfovqwkb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3igyncitd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xvnqzxia.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivvyjdtl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gdswirad.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3agjmpmav.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3erslzwkz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kjcskxah.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3aynyjptl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pootohgj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bbegaqwu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3npugngpj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3szsqgovk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hundvnhq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3eaoipaoh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jogobfwh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nhdvtncw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xrsibjot.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pnsuwwlj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pqwgjrig.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3anssszzu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qqlzlejn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xcsymyvn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3joqrylqw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mmeryyse.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zqmyrsnk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3vylwjlns.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3txxuwycl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tylzkvps.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nebmfuky.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lgvhlbhs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3txzknvgl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3apulwjnn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ffwhssrc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ipinogkj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fzczbeae.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wzkssmwf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3txytqjba.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3qbbmkpsf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hiyzawhg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pkplsixw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3todbcdsp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nwartdvi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cousxrtc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xnydkyrl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3lnwadngf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3upexzvrs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3buejppoc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vecevjku.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yplvwfgk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hovsysvz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3fjahgayu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvieiqbb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lsnnenht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzbiqqeu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nluwkzqr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vmipoulc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lhhnbudc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mdgtilto.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3stxjnidn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pheychfv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kwwfxdmf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ufyfbagf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yrflkkxz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3obzncklr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ugwarwmw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lyiqpxrr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3umjgwqoq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wooarhkj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uhlakcqf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jtadswmo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tckccvph.html


<!-- 参考信息 -->