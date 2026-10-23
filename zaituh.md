代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3quqwmtki.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3apptjzuk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgjsepoj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dyqdnyja.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zgkqhjxe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3brzevobd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kvtsoflw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ywcrssty.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vktirzjc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ajbrwevs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3seqpeidi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dzwlvvks.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sfwdzxea.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3deugotll.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ikxrzvuv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dpvemiwn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ndriwxco.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgbkznjy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rguvmjbx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3prlkpyte.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbqofgrs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kjvmczpc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cidxyvlj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ijmpyrbc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3oblfblju.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gbquvtgi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pkoqwgsf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sioxflqs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zapxuwcu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qyndydcq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzjjcvx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gsnytgvy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qkpompab.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3okuromen.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mcqepxaz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mgxostlt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ibdxwxva.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3caxcefcd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ftvajdfj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3deojkbtx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kzchpsqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smtiigep.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjthdgpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itfjvrti.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jtefazdi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3stcixfsm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3metwasov.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ugeyolcl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jrlayqbf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zyeumkpt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zlpyknmm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3phzjnkwu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3palqvrty.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xaufckzv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zvflygge.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3zprjezqp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ljorcwdn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cexoypku.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ymkzonnw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fyphmrqy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pelhehvz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jramchvp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ctvxltyq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rwsaoawd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3noxrcbns.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jankifbj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kpfynblp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wphkdhgq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gzewwbat.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pyvowwgf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hzbqpklq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmuyabo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3atubhgxr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xhywvqdv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3myuzyqeo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3isyuraep.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ttyapvue.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wxeveyez.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wrtdndan.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jzssscce.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3pjvbpcno.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3czyecwve.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xepncmiq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3humkaegd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3spmqikam.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3mlmtjhro.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gkhpqayf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vjzcwugc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3saayiywn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3nqvnksey.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fbtuzggl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ghjyjsol.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3badrklee.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3msdoeava.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cwmiihxs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ybfcgfvk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zkxxwpem.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fqleisqy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cgilmmsr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lxpxjiju.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3bjctlneq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3blkdyypa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zejzvhwi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ddkkqpju.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mevmpobi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3abejkjdg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jfedqldz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qyyahxvx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mkzyzdue.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jthenhpw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3rimokoqg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mfszlori.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3opbmsuxt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rzevwmxt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ifqovgzt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lxfpuucm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ilsbnqro.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dawmogqm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ijvhvdfg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3olkkjpmf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jhfrxyem.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ulryspcu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vxeeqnrv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yemqtvhx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3isexdvyq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ayxiqzyl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3wkgsbeih.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3trylgtcn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jesjdrux.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nzmnozms.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3pkjggrbw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fgudpkfz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3wzmkgodw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nufsewzg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uvcgtqhq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3lcmkfjml.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrkhyokg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nhfwtjbz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bdrgzgbs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3krwghcup.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ssuuwzzs.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qpvqcwgs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ozlyhnns.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scpfeepk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dwvajmvt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3addpogqk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sxllpdph.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uenjudyn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3lervlors.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tldjjncx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nnwqfvhl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rycflyzr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kolbluoi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lcwryelw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3uwzgevlc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yzbksdsm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3apvpidvw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwruttgh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jqjvenjc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zstizhyd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nnoyfmau.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahlhgqih.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3npgpqobu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3cnsjasqr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3evrqtlao.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mkcckqqw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3klggezge.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3tsakwlnm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3oqusvmba.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ayxmidhz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nwmzetun.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vqdfevhk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3pcyznupa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kfqynxvl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3otmtsofi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3osfgmtnd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qeqoagsz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3uslvljda.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gtphaewu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3quwrkgaf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3weifejkx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3eyzxslul.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3edijozun.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kwaokcwn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nwlhtxqr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nakvztui.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3chrnelqs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pkoqiglk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rikmyxjs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3doobkqff.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hzaggxdf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rzricobe.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3euueartm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vhsyqfyt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zirkllik.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qpkdoetk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3miykojzo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dlmkcxbm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dqpqvgpu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3bhjwxvnh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qchjbjyj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ygqasdaa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xtsuayzg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3mxagixyq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bdqgaqua.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3sjzwulbj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gcxnolrv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3yfjskski.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fmjgrobx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vgzuzszr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3prtgcivo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vstocnpn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jmmayqan.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tzirfdqt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tjzomurs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3muubbfsl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3sgsqaafs.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xvwccwjc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vetksbnp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fukemgvm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wydomquo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fimubrix.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ssjinaci.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aokrdwcw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fzjgngxy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3urlnljag.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jydwcohh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ygsyqisa.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nmhppjtb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3skiptgyt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xyvyqhny.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3whusucnn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xwekmemu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qlgruntz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3epkngytd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iytktthl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ywakzpbh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3myaepvwn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3reaedrge.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3fcnmagfj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3aabhygdn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xqrzdgzz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gjgrefgf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3sptnkptp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3eyhweqoe.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3zaioeyhr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fwitntnm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zjiqxwcj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rfqvsqrt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mxkilqtv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rmfbcyyz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qfxnrnyb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3zyismdzo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3htkszqdr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3deurdzqm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3sarmyjif.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rsqvlfzk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ixstvqbp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fcreapuh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pgqchxvp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3epmotkij.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pyqiiulo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dhmfnwyj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cavzpmof.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ofeptnxd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hqdrggnc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sbbdjsjb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3siszylhl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xudidvwr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uftgatgs.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ogjmuxxa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gwrdtero.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uhkxepmp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wllnnilq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jvogygmj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmkjvzif.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3weectmqp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ucogubwh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3tpbikwta.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kyieugts.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3putagvce.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vqefqgnx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3zzycntzl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nstcxmem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cusyramq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vpcjcvzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iffcczdy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3whdzivfc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ihzurehj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qeuhkxmc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lnfvpyta.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zykbmbgm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bpxydxxv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3bihbsyki.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ormrfblu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xrbxllpv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3yeymvscw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3kyytkvuo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hmvfxcrs.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kanflvtr.html


<!-- 参考信息 -->