代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pxftwxgy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ijqbsgpf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3khpdjzfw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hnzuulpz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jmbengnw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dzshqkzt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rurxgnol.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3giihocdl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3csiyztlm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hmkvxrwf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mogfatwc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3iznjkpep.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zyensgxp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrjhlhwv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ovaxrrsk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wssqyfft.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nibgttvj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3plfzaekx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jodcikux.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yjlinwag.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntcbalaf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cesgckdp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pjzvnwdc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3lmfopoit.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovudmltt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pkkhrzuh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mohlcazw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nqamkzyn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3clcbbpew.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ndqplihu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fhhnwrfw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bwjejuob.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vnvyffvn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vztkzkfd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dldzjbvw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bvauyzjr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iujudbgq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ukmckzta.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mhkfsbdc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3qoirdabt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3nbukoeqn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rkcpebid.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3difquvxd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hlddjfrm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rhgvnotp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vybhxbso.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rvippszt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkzgcjdg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vexghpeh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3euniplxn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ovxqhvbg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3odordqye.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sqqshltz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ipjzcnqe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3azwplstv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uhivyyqo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3orqlbxgt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mtoheheh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lmokufgm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qboqseoq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3psnuanzy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xwmdyapc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3cgixsvrm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hqdpidvg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3fjhymfna.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ddpaotby.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3fnoiagpx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kjshcxbf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gkgkshpb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sadmvhht.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3idfwdvsa.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3txsrxcbc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jborkqeg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rxjxmleq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ssnjeqlj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3deftiaxr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bjqmghnt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3yjdfvlci.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3awwhhqpo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vokarrrs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dxubbzdf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ssjujfoj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gumnjosi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ilnhgsmg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vscgclnv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzttoyev.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rlffierh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dmdnbpyo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ltjchxxi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tvecisdg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3llinqskt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hmwgglhj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmpqabbq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3azfqbkld.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3drnpvpqk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mvpnazwp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ygkcygzv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ordxugbd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jpduwhvh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tmczjctd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lrdwcqhm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lifgjoei.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3yhdkrtnt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yosivamp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3aubdhhqn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gedtyiou.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tyqogwsh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3gitvpiff.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3bixldjuh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zsixzmaz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iyzzfeld.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zcxytwil.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3meutinli.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3yhcuzipo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3oozbdmwa.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3yjapftfs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fzvhlffo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3osfhikka.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kzauwgjs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3iibiubqc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rygosbqc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dlpngmwc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fgyrpcpu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3yqrpbgon.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3segqcodz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yllgvknj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3yxdsmqnl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3eyeiikar.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tyzotlrs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mnaqnkid.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3piermbsc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zvecxoyr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mrgitjsa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3iclnfjws.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tlftehbg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qsdusvwt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hsxtvkye.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkpacirw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgrzybal.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jhtiimfy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fnwouvmf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cushxlsb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kqblmiaj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3appioafc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bhxvktou.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jcnpfhzs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uhxqkxga.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elsuygcs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nwnylrkq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wbbnimep.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajiuwowh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dupmdfxb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3aechkool.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lcyttgkc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3npovhemp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ewzpkdgg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ygydskhu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gzijvuqr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hgmqsxoj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cihiwsmd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tojdyjgj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3cuwhbeqc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gstcngje.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bzewgflm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kpbqeooa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vthashwy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3tdgxbdgs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wppctzqm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3derirphq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwunwphw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pjegodta.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tgyiwzit.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gwupcjaq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zoulcjgc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gybjvgjr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cfifbbwk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pozhlxix.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ensihguc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3lxetaryp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3iymcjrkr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bacxhnmj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3curdsdfi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fpjptekx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3iqctcknv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ylhgfcbq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3kheklhrx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zyekyuzs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hekzhnaa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3luczpnpe.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3aaakynrp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gyqqjsdg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dnwgdbtg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dinfmxug.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3khuqwhrq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ffsktogf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cjjvbckn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lrqcmhzf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3okrzljdm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3pxikvobg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xslzbbwp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tnogiqhi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jymeifez.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yvifwwyt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wgekiqzo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pffmlusv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qqpnpdij.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bqpdxwvk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3hcpmqdsl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3qsbnircg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cmgcqetl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3twczbvnw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gmiqifrf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3nqnrzzlq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yluoruqe.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mepvacpr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3aygaczso.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3azawcsuk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xszenyae.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lqqctveo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3cfjrciht.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fvyagraq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kcihrkgm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3uydfxsmf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3priksfnu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3emynfskp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kbvusvxo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lmhuchbj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ievawnrf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sfiezmmw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3iqbfacph.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cdjxxris.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cqgrjckw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ouuyfekz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rubbhnjx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjpypnyw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bfyjgzpc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qwazusdq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3otpjfksv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ljqvhdiu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mbsgrdec.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ahbaalpr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ghlefamr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jbbvlnwt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3zrzkxjns.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3bsixxsvm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3opybfyyi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3eockbuag.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hmuojlxn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wfzjsvae.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dgifwcjg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3cxrrpitq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3huxhkwmv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fmevjlgz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3kjnbxfig.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lgusmkoo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3urdvhaqf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3babcbech.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vbppkhxa.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mqqbvogh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3uaekvknp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vrpjfuai.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jkojfsfu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3upgkuwwa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qhkrspwp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nyuzdfgi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lrisqwjp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zyydefpp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3aiujmnzx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3lfbdzaue.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qbktarme.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3sspkliha.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wakoztre.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vxhnoizh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jlqgpdye.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zmpwjpxt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rbkbrpbk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cxyzjbuf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ojsabmhj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3aijvoygg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zpmjgwsc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3olauiwiu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pjxvktca.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3tfjzuoxs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rlttfnev.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3frmcrysv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kjpsgxdj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3icupfojb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3asckyasy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdjbclhm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ykyzkswq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgrnwkcz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ledemkei.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3akvsmbca.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fuptmaue.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3peyxhrvc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ydrtwgba.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zolqakqz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ltghdhho.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dzskepon.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vdkjwopo.html


<!-- 参考信息 -->