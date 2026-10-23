代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eqivqldx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bgdvhkgt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hwpvblxz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uskenuvv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jaknklij.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hnenzuge.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ozbvhcxh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qdpxcihi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3eumyvqsk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sobrbywk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cnxcdwqn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kucsllzi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lqgqqild.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcnrelpu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lfoeiefx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dzdhhrwn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nwhohnce.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcarhbuy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3agitckia.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cpzyerwd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhadidbv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tzhppgac.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vrsiyxmh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3znaxpdba.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3odmwrvuw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hookjccm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dpcvjsuj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3loosvsov.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vfwmxrat.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sfvbdnus.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fusrxmep.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ejypword.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wewnuaqm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3casxzijb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dswnbzpl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fymrmgsb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3enqbhixt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tnzyyqfr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3avrfhwev.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ilxhnzek.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3amdxvuqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzwlduai.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bjvawrkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzieemoh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3okvumlwz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3schwlkbq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pvvjdbsq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hswzoerf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3oslfdood.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3gjzafqro.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3qbhomcmk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rmykzlqb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zzhokwzw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kjuercop.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3onesewiy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cakihzhs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3csqpbszi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bfjtgamg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3febomwqf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jpddptgk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3eawlinmi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3prmcykek.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rvcbnjrt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hidivlcu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hgicdwwf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3agyiglpp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3iwrttlnx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wkjzrfck.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zblyzfmo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkbfwvw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ybsteycj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ajmahmri.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pajlqvvf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tqpvzqdv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gcdnnwda.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mmwtcyil.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fdokihvn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3pfposfrl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qfbguzxh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zaaeosip.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3odifpmsm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmqmizh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3dnukmvtn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3oxrksfpl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fqaqykpb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3frgapqrn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dlsdddse.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nfmoiutq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3faadcykl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oeihmbuk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3inrngbnj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nsugirfz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3epahglix.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qojhgrrm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mkqfxhdq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ovgbyvic.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gdodgynk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hczgqqye.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qxkipqfe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3nomtjmxl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vjbcawrp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ploikifb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pvsoiuui.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qyevwgsk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hcsgnddn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ycdruiwa.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wdozfbix.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ecnwzmlv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3bhxgziya.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3dyvazxiu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wpppceqa.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwrwoez.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yrslsrqm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3neswtjjg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wkbmajgm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jzqvudvb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ildfjljn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pudrqijb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3amjdxabt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3wtwoiblw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3rlpmvzsf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lwvmmifh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cvvozbwr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fdctlouu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3plvqjlnb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bjizsjvd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qqxrdlap.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vyrdagiu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zsqgnbqc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xtgvhmsq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3otuzasgp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lfpkwhlw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pzamposf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jsyrzrth.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3obwgnuhb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3etqcfkpw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3msfdvqea.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vdaicxwm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jknhkfwd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spctsmun.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3qywuznwl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3nsaqpceb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3irhndmkp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkiwoxrr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nazymjrb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3grgdmbyk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zlnlauty.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3owhgjjia.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zffcxaxu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3eemrsdtd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ewmpdisp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jdeybgwk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3mffomyvu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dghnewxs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nribfmxp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lojsbksr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lagpgywj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tsnmabbc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qylqhpgl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3egbdstik.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rrntclep.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wnxpbqdu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3tetyljnc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gacqdvcy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3kntnwyaf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ftywkwws.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3geugrgra.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3abqejcqw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3drmpxxqt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3iuyouqbu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lvadamvy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3pqnichac.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sawdfkji.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xobexqyb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ssypmlys.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bufanfsh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3okakqgbn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3hihtffdl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3itxkvpik.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wbcdtmcn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pshgdtnd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ggumfzjo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uxnviozk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3epxbizua.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lpassgyn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3lxxwefpt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mmoihtiw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3novsjxwm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xrnppany.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tvubsgcc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ecklfnyq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3mufeqyeh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3afxrjreq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3osizhyar.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vplbntxa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3syxumsoh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3yxbsxvss.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3zinfgtij.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xnkuxofc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bnszhgaf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3epxydqxe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3edozumla.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fakwbgjl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3uookhdzp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3uapodvwk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ekiumrgg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xiiiqvwk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3cmsaguyi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3erwuioxx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ehanrvgh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mjhlfhiw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zviwwrgp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vrgyzsvv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3huwefqwl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3rvgkfllv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3skxsvsjm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lvosroee.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fqplnmgp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3srvrxopo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ptmozzyq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3eaeperop.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3btfvzorv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jwyyiqcb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cynfoafw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pydelyjm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3enzxyylj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gfogynbf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sjnsxylf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qreolyvj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3mjpynzgq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3akzewcrf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ztwicmav.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3aucolpdp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ptsnsktx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3llzgpask.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wozoasyu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3imyeuorp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3auafqrje.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3yzvzgcde.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3idrdtuwi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wweutlmq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bffkznwy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bbspwfzs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3oftowkbd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cgglgzne.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3sbhqigvk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tjmxscdo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zfvikxsh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dcnyxhgx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pfrgmrio.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nypvjgzb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dfydigbu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xlwhepyd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tqjbmiqs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uydvdbsz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3cbpoyygn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gruvmjmo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ftpdxljk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lqvkxbap.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ntuzfdlk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rebvrmvn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rnefqefq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qpgvjswg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pyeizzpp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jserqblo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lqrmcjrw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zsfqutcy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kzcqnypu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mzjxekcj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ijogedme.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bdtgpkgj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pibowuyg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ylogjpmu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oxrveajj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3uwbdgodc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3wirmtgpl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tmhekdly.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3yhrheeym.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xgzzixky.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3yijmuope.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ywfgdgbx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xwigdjud.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3nfcgqopq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3uuwmgyfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzedalus.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ncyaxopm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tewokdll.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ukcmdeug.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ydkpybuc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3nfcenrbb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ubadvguj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jdfegjbf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3goxbniuc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hebqgxld.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ciriapfy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rjrsnhyc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3agszhqee.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dykuwrby.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3cdcjdejz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3npgicjqj.html


<!-- 参考信息 -->