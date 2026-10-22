代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zypwvmbr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ustnrhhq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dfmqhbnz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dwxfigiq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rrmrddwj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mpinpjhd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2uqxcglao.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vihgsgyw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2myxgompz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hdikross.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lstodsyz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sequwlji.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kmrwybay.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2drmtdrbt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qppbziax.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvlcbozl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pwxdjjnp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbvvkahu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pbiplfah.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nukvgwfo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gbdzgzqc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lanwuwff.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lraqslxr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lkrhrvfz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvwummnr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jayflovn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhdodfmg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2lncmnuhi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dwctqabe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pblqgsrp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gwxjvdwd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zkttxvmf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2fjxvttvk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pkwflmba.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kkdwykni.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uyctegui.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfxgctkz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qmzvssvu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wijauauf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ryixafwx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fbrgbtib.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fmfqmmrt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hwkcqrme.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2raognyol.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2njuhwyqk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2uocaybwz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2igxlyzdt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ohifnejk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gsspmjtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byasoihj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrxrqhzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cenempxl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ptrhylqn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xfdgvywm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rhenbrgu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hiuwwcce.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sicjioxr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gqigpefb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ygwyhbtk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2snonymll.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ovkkwsgs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dvyrrwhh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2feiirubk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mcbqgjad.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lxwcnzfy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2htlfvgps.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vrbqxvni.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hfnkfabw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lzuasehh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2oraxvvtq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zqpdjeef.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2krxbnkhi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ecrzvhui.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pmmubief.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2fbryajqt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2csbbmdpk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jyfibptl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wkwsuxqf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2khemwwma.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jlgfebew.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cepubzkw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ypiqovqj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kuabcmff.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2nxaqvxfv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kqoafucc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2swkuznxy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fqolwilk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2prtlraao.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xksxntsh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2laoiutat.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2sdkphppa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pmquloaq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2orwroskp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2eotidevt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kxktqlpe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2fahotaeh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kadtakqd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2clxiticl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qiuboweb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hzntezlz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gyosthnd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2errvwbcf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2agyxwvyg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ksjkuzmt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2punfwyuv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ygwarqsv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fsottfva.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ibbavioj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wgivnvvg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2djjjedsq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ubovnett.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rornsqos.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eouoodfg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hqfwsrln.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xqkpgcfy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xuzjjwvd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2umreorke.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dwqctekx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2epvdiywg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kthlktsq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lumrggju.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2spyvotjh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qydbhbqa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qbkhvsaa.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2puatuuko.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ldktaymu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qsbyqcpu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2aneooouc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hiptlwae.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2sixtnfuv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ztomkjyx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjbbrtx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nbvvmuru.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2riyngqgo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hnlyfiua.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2igfiqhbm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ndqtynnk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2qjmqvcnx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2lfwaitau.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wqnslwoj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2thxwyeak.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rnauwsek.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2vhonvbpl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hdchsxuq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2cvgrgdev.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zdezpphd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2nmgzycuf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bbmdwxlc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nxusmvuu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lekqvjej.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xdprzqcn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yxdegllk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gqcbdfca.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mzdcayqk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwjbpfbb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fkhrzpsw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bhophwbj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rehytbud.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ssnrzpvt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2dtclbwxd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fjjerisd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iuaolhif.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kuvlcupu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bajdpyzh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rtqoqvaq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2eyrdnpoy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dpqagjgm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2cnpcapgx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2umznolzg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pztryiqo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zaqgquyy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lnuyuyah.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xrxsqvjo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2azwerlrn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jezwbokf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rwofsglo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rqwaezpk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2uaemhjtd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ldebuabz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2szkvyqqb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2lbxayvfk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wsszjazq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2fqhkpjpy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qyxgpkdb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tvcarbkn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hlpbqshs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jedfqici.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ptrgqfox.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bgrbwawk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ybrsvksi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qcaxghyq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lsipbwvi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nuvwkuxt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mjfszhwv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ezyruwwh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xvshezec.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ptvbxyzo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ymvwfxew.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cswbuixm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gsrwtlgp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2oxfxtaqu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qiwcwrgp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2furegtxf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2txnbvvfn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2tjbvrlth.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qrhlmfbe.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tkfayvsf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2aplybeil.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2styxmrjv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jsmejckz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2medkfjes.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ofgibwfv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rlakgall.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2giafipgm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tmfxiakw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2zlrnwgqk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2aarumcps.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bvztvazs.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fhvqloqh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fmtwccti.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2wxjazwlb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2uoihwazu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sxqmwmop.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nkgixiuu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kredqhwu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mpnczhfz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2nuvfdffy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rshjanmg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2frobauiy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2omotkoew.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2mbuhbdzp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehsswixp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2byogfdrd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hjlwtigu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ndpjtpzt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhitmlqb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vahdqmit.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gkdpaisp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ffevvdxm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zgoctita.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2cocbwlru.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zcmywzpw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2arhbkoqu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2odizdcbt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2uduabciq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nxvugwxo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jkpogybz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hnvpdtjq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2uoofzuby.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hpnfcmpm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2hpxondet.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gwcfdxee.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gktmexoq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2zhphhxtr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mdlbtnnu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2pnyufppz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ayjrnzos.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bnnpwynr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2exhfvmtt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tyhhbykf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fnvtuazw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zulltnkr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iqklbrum.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2szhyddgk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2brdnidkp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mxvrjmna.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wgqsinfh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fjcmwyem.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wzrzfopa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2euosbucl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2muuicldq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2lqgvfexz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2psfybczy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zvtwrkzo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2sarvnuzl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uoldnmoz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xvcfypit.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gnpulseq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lwenwnwl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2islthyrx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oivzqchw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oipvyyej.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2tlhkggdn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nrqtnswx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uahpdvzy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pshggwjf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zfcvzotg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mxnkldrj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2jknzhbtp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2hoqgmpou.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ljwdicfr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fxxomjok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdyqnpes.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ggqvwpxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhayzarc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2scwvtdpa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2idgstydy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2disibvbu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2svvjqeyc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2iwuxhvqb.html


<!-- 参考信息 -->