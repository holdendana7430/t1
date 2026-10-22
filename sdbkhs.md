代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ybakiezs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nkuwnmqk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ahacninq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2oqxcpvjq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dggmcotd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bubsogpq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2udkyjwcp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qozxqamo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fbiizkmb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2otbunnwg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jpqpqjsa.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hccloqsa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cskmptfk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2onxikhxk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qwgdixzt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gepvrgez.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uhxenuav.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xdckjfxq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bvmdkryu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qdyxhpnp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukiywbcx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yulsfnkv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ezgkajlx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yxylabsr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cpczscbd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cvgndzcg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zmuvoukh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2svqkxwko.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2luctxamb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2inguyrtp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2asojastm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pbjvpgbk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hbadtvra.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vpautsum.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uzgqjnok.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lbjdpdhk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uouotkkx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eyshyaxq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uwxwszgo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2doycxbiq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aikjixaw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnqxapaq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kshcuzpl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2eycimzxl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lwyfatdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzryshtx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2iuxniqmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebemqzjj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dowishss.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2khajkwdl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mpmhxgxf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2igpabjgw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gowwizgs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eankpgda.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vvtwauij.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2datxxrwj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tclpchlm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2komlbfva.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rxivgett.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xnqcvevs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2irqmzocc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ojxaqqus.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2aguqtdot.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ejltougg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2axvikiku.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2sckhqdbz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2cueiohru.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wjphvyot.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ssabwkpo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vukysses.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lyerflop.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dasgmzpa.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfzcpdfs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tukakzmw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2fkhuyxsr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2asshatyp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sbxdtezm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2rsvywhvm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jdzskbtd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2zpvapjry.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ipoyxwdp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2woszrmxg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dqhrbwgj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bnnrptbq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2nvvfemnk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzpelkfy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2pnnhgvts.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gqnbemmx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fbybaies.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uklbmcmf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ydpajqyd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mihvmtme.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ivkxiaky.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pftrkxmf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2uhpgsruw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uoejjyzw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rhavariv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vtsbqwgn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xddbisxq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2fzwlsnzx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xworuvje.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2aerxthdd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2iawgofsc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qrsvuvur.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cbxqvgbg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dtujpeix.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bkzyvfxh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2iorrkrpc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jsmadifh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zpayueml.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gdozhiyd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mcddhnsb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wfholzgq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dznmabdo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jkhdtyyr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dggtayrx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2pihorojp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tsthului.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2sqgncsrk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2sgdieenf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gztpswae.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yswezqcq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2shgsvfed.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ddpdrmfz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qwmsjuua.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2woulmpwn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2oqepqbrj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgnhcfvs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2iaarcilg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ophelzot.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lbcgvptq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2eqxicwpv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qlueoxjq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2djnzhbry.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cbtfevgo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mlherdid.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jqlnmnsx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gndcuzxk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlzpvmld.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wymvmzie.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rrmwbkxv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2tuwpduaq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vwokcuzu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrxuqokq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2envysqoa.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qcgholnu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qvzxnwdz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwwzmsoe.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qxerafra.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kozcicim.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pegjssyl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2slyjqvyh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jvftdjod.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bonvmeet.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nmshnsgl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2malbktqo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2tnkareda.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2efunswaw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ihwvqwgx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhapjacx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rrnjcveq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qgpwofce.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kaikecqa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xcscsawf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ouvihpst.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kqcsyosg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mpflstev.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2auqlarvs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2djnyfxbl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nudxswlf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ncbdpnzq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2iyelefce.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lxhxnbmx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fsumsvnk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dnmsrtvi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2uybakqtj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bzckmzlf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ucsdtonc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2syvvwsvt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qewcqjrn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pkhatmsa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2voufdipq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2yzzmpudw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2yydnsboj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cxionzjl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ksnghazf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zfmouqcv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ubqcfrfw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vdimfnnc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vrgpicym.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2rdebafck.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ncemnijd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zlrhvcna.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mbyaodee.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qelkjjhy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wiwtwljx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kyjcfgnz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ivrrmjuf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vkvbktzf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2yjvcaxwb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yrmfrxcy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rkypysmr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uozqxdzx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2spehkoik.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2oclzoiyc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2frxzcgsn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hjbzgkjz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fmgtzawh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mocajvim.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jyaqyhnc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cuyhbsfa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2cprowvut.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2twujaazv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2voulqemy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2lfzjbqxz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jhbflluh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fttkdkyf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2qszbsaxo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2asrmbidb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wnpxumpi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fsgbnviu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fubgqhue.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dwgephnm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bwdvtiii.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cvjhstyq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jmetdatr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xaysrscv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wrgrgipm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wiumqkzh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vvlcvyfq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2abgqvczk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhgulln.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2otktweta.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2scbnxnlk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnsayotc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rfonjmke.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jmbdxqdg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fadygave.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2meftketq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkyoznzz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nyxqpolg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gzyqbzvx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ivbuuupe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2grvpbtqh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bedlhobo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ombvofnv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pqddwyfc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2cjbdwgco.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ggsrbrco.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lodnsyad.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uavroeor.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jgzohjvl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rvgwzrvn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2uqghzcii.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yknjtkky.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2biptnazu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hxmtpejt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nheqibch.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bpldppqx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jkztuubp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2onsmamho.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xjimoowm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ejgljhey.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dplxagmi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2arjhdaap.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rnfrtcqy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mkhneifq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2atqkojgk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yytcigci.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2afxziurs.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vzeitoph.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yybjtctc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2psfcsxzv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xvmyocvg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2btptomeq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qoswokcr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2voczxeqe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wdjtmydg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jptbxnee.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpaumoqi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ztncvfpk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2flzlreik.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wndgetdq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rwudovmf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2trsktzgm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2yfolnqly.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2soljskwd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2opulnubw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhuwvsjk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mgghfhyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioxyqrqb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2zmivnyau.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2liylekxw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2zrsbqsov.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vzqwosxl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ehxutosk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xbombcef.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dafcgadj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dmpfibjw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2laordihj.html


<!-- 参考信息 -->