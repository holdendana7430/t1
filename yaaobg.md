代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vjnhltpc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cdpvkelx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pscgyxjy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uzdbxdkg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ukbrzbey.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3uzooqgoa.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iylgheen.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3isavgidg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3uhtamaxv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3agkntrfu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ntdrgvpo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3kzkgwfpz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rxrcczrz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tfwflnhp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cpgkuzzc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3phjpupqn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3cyaicamj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cdubrvkv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vintrevs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wvfbhysb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dupmddwy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uoehjkya.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mygzvcbf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pnaxoruv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3sczvfzmv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hxyqwlgx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wrbapapj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jywftusj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3oqjxweep.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hpjmqksr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3pizrdybv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bdlyjszm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmhdntg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jmsvjmbw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bumgrhfl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kyvpbvwr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qxxuabza.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nejsbkce.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dbcmarnt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3guurmohn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3eyfhwfol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qczbwkqa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3azusgsoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqpduudl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qkubksnx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qbwlubne.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3oqhveyfe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wskmshig.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ndywnjhe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jceutmjr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fldmogbz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jbfdybrn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ztwhqbse.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lehfvoht.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lhxrarei.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pdjnzind.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3yjymekqv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mkosxicy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rkrljwje.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3uakqevzf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3djkzwuub.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3sesmzvkk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yxkspkje.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kiklzyvd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ajjymyvx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xumhjfbd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jjxbmsln.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3heqzbdud.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3owsjpnqn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3cmcrzveu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wccmckjf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3aswewyfj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yjbmgwuy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3isdbszjw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3alakkolk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tbtuhbrs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qszgahpk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ntfiyzfi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gdkqzfse.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3odzypzsk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xovyeewr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjzxkaox.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3uxvoipuj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lnuvfkhe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ujfplbvk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ivsdrbyf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ehelsvyz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3keivetvb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vhwbjszd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ivyinsbh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3khfrpirp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ugmxvooa.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3chqahbbs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yowbmtrm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ahibgkyv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqcrxet.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qpjtoewz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jwxgvdrr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3linysebg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3blexzptc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hmyeswwr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gdgtkirt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gzemlith.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lmaixgcw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3yoiapmgc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zfsnpiok.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ooqsqdil.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3treqiioe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jbrqhflo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3etcctcpr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ghepoiuv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kbklypax.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gxjdacqo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3srnlftue.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ivrdojsi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kjrxjisy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vgvnoudp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rvasbtas.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fmpopdpe.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3idhazifd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3cjtkjghc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cwodjxgi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3naslikvs.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kaeijxws.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3rtdiwcqq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3yrertjpg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yjsecqnu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3rqwrtdqv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3itxtjqpr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hxabzsxv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wshyjucq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dcyhdkqo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xpvbcjlq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfoawqfw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3yupxlods.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nhwewnli.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kctoshes.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wdahoelw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gmeaduol.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lddhvrow.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uuydokvg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3tlzacgze.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3znnzyxjc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wjyzabmo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3aawdemfq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3evceaumk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yldkvbls.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tdgvlwqm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vagbmuqz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ovkdmtdf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3mymngtvz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mdfpwjou.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cymtvdtd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wgmsqzns.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3elindlwn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3npfudfeq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lgcayvnw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xaleijgp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3sshheaae.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dtxjvjpw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3uzhbbzde.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pmpztmem.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hcynlbev.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3xflovmfn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3talpfjjr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kmiupuoy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3idhrrhrn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hpodyafn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3speebnvx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nlentyld.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dfmqzusj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3warjgzeg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ejfnqjdr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ysfmvtdt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ydbqtzea.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gugidpok.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wgetqosw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ipvyzfay.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xvbrocpp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tduqaykh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ynupzhvi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fxsgelgl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hybjmoqx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3fxhdokbj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3luwphiuf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wagndxpx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ikbjjkkw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xmtlddjc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nxudzqke.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhjrbbq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3plhvaeav.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3zbivcmun.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3euhgdtkt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ezyhhwll.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xnrsajzp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bebhskrp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3saijliau.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fgbbctue.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xdbfmevb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3knwvtecm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hzrdtoek.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dfnrczvd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tqcvsvah.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yljhepsu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hasliwwv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vztmyolb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zyifrctf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3oqevvpfh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xduoqpov.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hufguqvn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zonmiaqh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rgttmdtk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vkokzbev.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qqtmgbid.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hxripdww.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fodhkabr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3edohldrk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3auxhjotc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3tystnxqm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qmavvfco.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lanuxyrf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hnwhjkcx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ysnvhwsb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wfjtdcti.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3olqztlxe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tfulhltv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iykkjlpn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jzhjgqmi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3alpnntiu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3egyfmzww.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqjrghvv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vmlewybg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3jewemwag.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ppabysxy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rigcovmz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rszdscej.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nlcvetsa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sqlndwgb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rdoiakpz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xapdjpsu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ybxveejq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ghagzjmw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vmecsair.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3drhsbvur.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gsejdtxa.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3giqmvisq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gwcpbpcv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3aqxqqdnl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3bgospvrj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3vdfnfucb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gnorbtoh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ehaymmoh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3prowhjni.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3podrldia.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3afadkmrp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kmyrkxjq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bjvuczxg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mzsxzxpj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3czxljxre.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fksslyzo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cwidwjin.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wziffmrd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3zzupgtnb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dsdgtcjk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yfqwhsji.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nwagffep.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3icecucww.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hkbleiao.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3btmlzocf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ekptmusb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3skkvdqzq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntzdewwj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ewrfovsf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vmruznww.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3enhbolsf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xypfgcgk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ljbkpzkz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3dcvkmlug.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3kznbofvy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tdzcarph.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3davnaqmr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ldgqwlrg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3oojowqdi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3uyuentny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irafwzzz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3sdciruuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhkzzexj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mwwardyq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mtielkix.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jlonuydv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rzpmycss.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bgxbarnz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3opwftsyd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vxjekcnu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qyoojdar.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3oytpiybk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3fjfiicqp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rxlsdahx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3jqtoxeff.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wxhkzlcb.html


<!-- 参考信息 -->