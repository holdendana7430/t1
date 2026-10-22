代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mtwqzxnc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2efcqepvn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nedqiiln.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2impdlunb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uqshdmig.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rhqearvi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ljdeplds.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2epjprots.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnwicomx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2psreceld.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gkjvajtm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qctmzzok.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2sgxfzxqw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2slmyftvb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2karjejfp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qpyobkrx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aukwpfjx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qjtmzmcj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xbepgvzf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2txutvape.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2efmvxikp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wycojknr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmapvrt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lzcguwzk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ijwgbyhh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kknwfiaj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xrvqmiil.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jqjpevqd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wkfqmhmc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2btxdhuxl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dwnqebdl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qpzzzwqo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mptxaihe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iuttmvgn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wtcracul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anxgrqwe.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2whtplngg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vdecxbue.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ehnnhrik.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pmebfpbu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mhyfnttl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tlvrpozq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xqmvxidl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rjxwahbh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kknztxpg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2esahnekm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jmnmnynj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pbpuhexy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2yedoryzw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qcnocwqy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lrxcmxna.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2pgrizegu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2exmjoamh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2upigzwld.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kpvmpeqw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ktbsnrhl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2egpvpzce.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybuwdnrg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qlzftnqz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fffimfeu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uwlqcjvs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vitbuhao.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xnlyanms.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jefgspzg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zvaoynwc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rvnaemxe.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2doioabak.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2eyjdpmow.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ybczdmtd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jklffnbv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kerwsaih.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vhiknwkn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qqagdtvy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lpteflqi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2txtghgkj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hggiugir.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hvmospnq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dyybkhtq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vsplqujw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2piadissx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wmdkslhq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gjpflhcj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2pdtsatzc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcprqip.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gnznjrln.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ayouhulf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xnnjxivx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fgmutnom.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2reyonyog.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2eedzvuyo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2dwznewcl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lpgcvqmm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fgvwnqjk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wnxagooa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2coxzfnum.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmelqlr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2pbbgeflo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uxxgqbwt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2kgdjfzng.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cpygtwyz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bqwrzeuz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2cjchblay.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ssajwysc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2lqkpfqpu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ytosxzov.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2tqgjqhhe.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dyzlhdin.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2envzkdex.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2pwznxdvt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tqklgxnj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2syozmeyt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kozfeqlo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lbabokwn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bzoikjwa.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ocrfpxyv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aeaedcwp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pnbxbsob.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kmifoizj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2egrjakpu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qfugboxs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bprmdqhk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2quzpgjqa.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fiobxcur.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vkwedfny.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2yzqlyttc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ifuahxyp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mkbuhvlx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hacrhiov.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bpehqyss.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2trlcreje.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ymxqxuro.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2isibrotw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rhdljjau.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zjueyikx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yedqutad.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2csldlwai.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uznwqbna.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ycwfhhei.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nngpfvzp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wnmemmib.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cgoxuipd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2iqqpqpbq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tmwqsoze.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2opicsioh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kyoifejz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tfhyszfs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gfyknvsp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wkdapzte.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mxkrfejp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2knehxxbt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2eoebtbgz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2buxhxcaq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dxqxigog.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gckgbpqu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2iagezksx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2blaltwdi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vugxiouu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrywxglh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xdnjetru.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qzgkiwis.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2gmrhrcmn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2kwdtqdup.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gyankxam.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2cfqmlozm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qqkvbqsc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cshmzxyn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2psywufvu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2atcluynl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tabtqswe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cvmsifjf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2eaeyxbfk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kzehyiwm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2agnwzaql.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xhfkdrmj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tzabbmil.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nkfxtvzd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2thbrystw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xuvhnccg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2etppewuz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gijhdudi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tevoqiws.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pguywcwh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fcjalvhj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vkrdlkvc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mjnfixfn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nkojqhjn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vajqqjlq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xaeaatdc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2sumqsphi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ydamswni.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ziwnknlu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2agytywks.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2drmfdzxi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2gbwqxmfj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wffrxhng.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hkxuuifo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rwbooogs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hlwgzqef.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nxorzopz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2jboufnky.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xfzjikhv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fberrkpj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2yxurnicn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uqmcvsud.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rzkshqkd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jjrlmwkn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ktoumwpx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2uwyxgybt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mdvvyyry.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2utfzjsjq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2onccvwko.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cpzxgvwv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lhnnxcok.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tatkhcyi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tudpikhx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vhlwkpws.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oksxelda.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lfhoebab.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2nbmfdzuc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cwqmsthu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pawdviwt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2uhdddpwd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnbbysyc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2plxejkox.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2fxbmobjt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rpgtgvjl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ilnkoujw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2axspwkkw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zonmledo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kouvpoiu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xdgelrqv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mcxuneps.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2irhjosss.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wefpyxrb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jwwathig.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bzaajyjp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2efzzdhrb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wovclxjg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2yndilrql.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2iouoykrj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2oesmtrww.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jzaalvkd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vpzdnyqa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2imgrnlvr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xjdicgml.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tdtppeqo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hjvfeang.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kdniopol.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vycxlewa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fyhchzlw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ouszxvtn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gwqqyktf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fxxjdxlp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmcejff.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kmtrrzmu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jmzekkko.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zxbscrja.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jlolqlfz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2uimcprwh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zsoovpib.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2pozsrprq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wtwutges.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mdhjhipy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jnyaqcng.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2coecvqyp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xldaioio.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fqajjrhu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtqoplfv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mbgofltx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ggpzbpya.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dwybtqbc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2doxvkugr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cyxfclae.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qajjvldy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tzkwkmac.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2aaylhmgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xncksuqu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ulhtrvjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srtucntl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kujubrok.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2smelwwkd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vzbettbj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2oshvajyb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qxfgzohy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2aagzerpq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mlilawny.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wevoiedy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kzbgxfnf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2egofgfuj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2chkahkbt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nsazsrre.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2fkuhqisr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vcbzdgka.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bvhxhwqx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jphhhzrc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gpoilxqv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wbjixklq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2viatjsul.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vnyqqady.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2lphpqarh.html


<!-- 参考信息 -->