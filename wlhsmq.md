代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qflhzwrh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2omyhmcyv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2spgpmipy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vrhvxnmv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwrzvncg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tusuwykf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ztsniyyo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2nzzfbtyb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2marnelul.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qragsbsv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2atbbzyzu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pejbmbpq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2smojcqcn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vfvbqrwi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fpmuwguj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfsehsem.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qvlmlweo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqyumawm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lvckgmbz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2efgoajzl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnhxsits.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uteucbgz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kokzsgto.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bvarlxqk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vkzdaacb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tvqfzucx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lyzvynwe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2awfgofar.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2toutdtiw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xcdpfxbq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jbonoyog.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2eyqathkc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ibdgjwhy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gaxjkwce.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2knlarcyy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2bwejkqcs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlqseix.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2whsnrubn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mxbpgwrc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nnrefvan.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nuzzvhic.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wyajyvpj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zueamjvc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rygjvnfd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gyycsuzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxczyngh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sfjundum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhnnsazw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lmgahzef.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2acybbalt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dbqoewdz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2aqxbepjw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vxzfhsus.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lulvqtfi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dadkpzey.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rlavcfsc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ifaweoyv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xryzaynz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nmezyjko.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ebinleuc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2guifmhvf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sqrliygs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bgaztpty.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dqnqsvfi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qxbqfges.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xadfdxty.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fgzjgfvh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2optzhyaz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gwcyecbs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atipmdeu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lsnlqxqh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxzagiir.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2sivtkmbh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lfbjxwzj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ujjkghgw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ufeaxrew.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ugohdvki.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fczvupcm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2cmyrjwdg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fzupqvym.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gsgsweio.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2elfnxngi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ktxmjxma.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2evxdgtio.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mkpdzmpq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbylqkqq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lrqklbmo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2svgamekm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2irlhqlaf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2aeqgboom.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2awbxmrfm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lvjwozco.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkgllevr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2fucrqolq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ddjnnzeq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ngcncakd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rpmbbsed.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lnqxskra.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2auultilo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jochjqym.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ksetccgw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pmtsprwo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2stkjreqk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mermprhk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tuqqgipg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lyjnpgeb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zvygqqis.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ppxjzrcd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2sozmqrfr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jigkkadu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2htpeowhc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rsjiqzhs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2eodudftc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rrcwccqg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2imjqqdce.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jijttsyc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ukolzrnu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cpzjgzco.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hifqntrm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sbaonzlq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zitolhnr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wekokhin.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2euujirbx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vegkttub.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bxeimcca.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nmwaswbv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2kittwvbc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mzxhlcea.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jczurvua.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hgslffbr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2wfputzxo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wmfmlhku.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2nagfkstr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2zqfqphjg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2iucaqklf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pjflquhg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hcalkhcy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2evnrgdlq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bwfbdphw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ibiizisc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rhoprbig.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ncsxdfwd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2jcflmfrg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2svzrcqvv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nslnqhih.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mbfxcpkb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ixyfxwgj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yuwqutgu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vkjraubf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tlkdzbfr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2onvngyhp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hbzkonit.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ekdhgkbp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bmphhywf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2sftnvrmc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wthmucuz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mdhdubie.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2upmacpnq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ubmrxzfz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ccbaytlh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jblzrqyj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2swnqszrl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2swgyvqsu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2awkrkwoy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2exaucwlu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2scoeshny.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fwbgkhhz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lslbtuep.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wultanlc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wudxvnvs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2mecroxpx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2onbrhbxp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rivjmizo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2yscrkyew.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lfvvryud.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mvhbimxc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2glrzkeqw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qmtdpbfu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2gyvhtqzr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zpezzfly.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2wxzokysl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2flzzhecx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mzfrwzyx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2oteukcok.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ogfvdkpc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xvjgtkmm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qmyalkno.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ygbddzcp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nyhnovzs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bxjyygmx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2mmnvhkiy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2oknxiciz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2abfolmyn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnwxlsf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jlvomabs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qtjmqbdt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2woawirae.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gizltupj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zkhvlxoz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rnsbwaft.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zgtstwqb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vglkxojs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eoftnpsg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fqaiiqkb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mztrirfc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vbijdreq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2copcnhsu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2afpiseyi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2guevbuxa.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2csslcmyz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ndybpxzq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2eykamfbj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2lvmmtqvz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tlwckzdm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2oqtuvmah.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jdvdynsm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ptynmkip.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vrbwbcjk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2sbybwziv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2nelrlrqs.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rahximes.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ntztfyys.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kmxtgqoo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2qtnsniph.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2slydcamg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ouezbwoc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2whtfvfxv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sqtubwwy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sexinycr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2tertzzdy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vebsqngx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wmncbfvm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rlmbargx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pwxxdlyk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2iiyszpuv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2voiaxzxx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xutxuqxr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lrztxzjv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2jtwakgza.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jwasnqzn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ijjlybhn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cfntlzuf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tsjfqslc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mayuemtz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2praencdx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nwqflsig.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wddqlouh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2guzfgcmc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ftaqmiep.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hpbkiify.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2avcnwpho.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qmtdonxn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vedzxwig.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2onqzdkvl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pzvkvdun.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2msewemio.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lesqjrhu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rimumxpq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uhprsxqu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2txgwjscx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2waxuobjo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iuwpthds.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2srwvomel.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ifkhfnvy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wyudcvhx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mygdakit.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yyetcqqx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wulwrfjf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xvpfgbwr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ajzwvece.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ftegvquw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2plgsoiyb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dglawvjh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ifmartje.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fzwwhdgt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ilevvuxz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nyfcxavw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2whfbkcqy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2yzviephf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhwacfhw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fgebxqyh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qrjtaadb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wgwvggju.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jaichlbm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2igzuxoqv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ldbxvwto.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wjhrwqji.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2iowmvivl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fokmqkgv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2locannfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpttxikj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2lynporgw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ogycoojf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hckehyos.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yqvridgq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2obscacki.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tbpgrpqh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2skdtuoxs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ysbaoiwq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2chxtjgyd.html


<!-- 参考信息 -->