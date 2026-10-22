代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fbctigqv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ugayypgj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2syhpohat.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ztrovpvp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qbpwooto.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivsrlmwu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2swaxpuza.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kepgxzlc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zyboeuuv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dbrzdmgu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pmsapegh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zleuahmt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dupfubll.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzqzpaww.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qvzwvdso.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pzlpbewr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkuebvav.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vsqwuwvw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uarpvzpe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uaiszofp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tsqmmseq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bkktjyos.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kjvjqmxx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mnixxxmd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxmguwt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lncuvxih.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2pdsrsioj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2fdmpsxtm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2arzaoysx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2arsdfbcj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2muezizld.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rnonaonm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ycoegefn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kirsnfki.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xeurxpcq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jjomaugv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2bkrewrtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okthtflq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clhejnnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drdxppkw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2fqhgnoic.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2tslfcyhv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2muukvtuq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rddwllnk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nxrdnvqg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hvlqzfoo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kkfnqihp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lhvxrrqj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2msbxthjl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2trgaxjhf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lvkzipeh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2romafhwr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ouqjwlcc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rcvitglt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2sukgpktc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2isvtsegv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2auzjxynd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzsxjkm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nekrxkyl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2oihpvipk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2poptjuol.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qzujcpof.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kzyfhzzr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xviocykz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qabsyncd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xxapsgow.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2uhtfjzut.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hryfabnu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gmjxmrzv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2bssrqlip.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2yfpjvxoz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cwaysiho.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2oltlcnrx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gxcugpts.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cgjejutv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xfbbpgkn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zuwznhxo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhoyqdlk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qutxovxo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lksuwtxy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pwckfkxx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mwffmwgx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2jnjcvjev.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2arnpidxo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2defxqsdy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dodqrsod.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2lnczoyxa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aymjwgkz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lwaipusk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zffkxkaa.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2voljdnas.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tbgtpucq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rkvkqoxs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2acgssiwq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2fjtbquir.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2nusuxpkj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wqinwvqr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qtgmcqka.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ctjxbgir.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hihqxslo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fsjvesxp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2aqmzenkq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2igdffndl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xjnehlwi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hwewqtye.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qmevvsuf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wkchbjfu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vnxscksx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2quuiikfx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lodryptt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rlyuwrzc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hfiiqknm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vhqvxphw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gbfxfskr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jfyxritq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ltdhegrt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bcbdmxof.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ovhjruai.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ummdpfnq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uryjbggy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2mkblgvsn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kbadunwy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2chlxzayp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zizrsbxm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2abclhwug.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2shfbyinc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nunvlgxs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tzczwixc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctipwjan.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iugndinu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bgpfamwp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ydpufqnz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vdbiksyf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lldcgyqb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cgfqodkl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2djwsfgqv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xnvtplug.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pdghzthi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2keftwctv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prjkahpo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uvcxrhuo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vbnbijuk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tsnymgdt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2azcouyeh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ngzoifov.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rvgbqtli.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ckxaifdr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2uypgnoar.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tllurdge.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2humsprne.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hyingrjk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypoaegbs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cfznmjze.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qncicvdd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ayifhlnr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2emoxblgg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ifklfzyo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gijwugic.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2lyfaeheh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zlcaabkr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lxgnnyxt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ibfblfdo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ytddmqmd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kqmhhldy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vwiyauwm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2rnljwace.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dsboipxh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2nnnfcyde.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hgzikbeh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qunjcwjr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qzmnhltf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2adryfotk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2uhgwfpgh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2oxaqeiyh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vuezdqon.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pgmmakqc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ijghimoa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2moogqyop.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kqzmcoxw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gefafrnr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qlhuhppg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2escmlfdb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2fisxiytg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ebrdaakr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ihkyypov.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mskfatmk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eoykmafm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2szhcabey.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xadmhjow.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2oejaegpy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vewvggvt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2svkmmpui.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2lkccfuwj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ioijupit.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bfwwdmkf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rmwylrxm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fachudjc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2claislvu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2grprrvfw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zxdsizlw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2voukzmhj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jlqvycqx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ojharbis.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ohrbidoq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tlltizwn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2znrkmukx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rbfrctdy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rvolpgsd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qhhkilax.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zwbddszt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2rgngvtof.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bomdghey.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xifxxzuo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2gcnixapl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pagplsvb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2zsrfvhcv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2abkbfybz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zlfodysx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2faxibqkf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kqbqyquh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dbogcxqy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jnjaypbv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ahvpnxuo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jpzgaitw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wzvbmxmk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nbkrtvrq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxtkcndy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ienmoofb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2uvdhrsey.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hxvwcxdp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ijvuofhi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2abefkuqk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ghuuarns.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zoafdkji.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cbqmrfjw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2olhigeqf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qcngfyjj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hbrokpqd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jydlgwwy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2chwytely.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdekdgsv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gtuogzah.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ssutosyf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mkigcbyk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gwojtshy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2byfvruzm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xyyhaqfq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ywpvcizy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2azcquddf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2dhcfplwm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dtvuiycg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2onsbpvyf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zosyhidc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2txswneig.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kofgyhbb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2agymrjcs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dianophe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yydodqsm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wglwillz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2swbcogvz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jrxlrmzr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mskjsdjt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mtfkptpu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wufmgimc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xasjznqh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pduwoqqz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jhedwbnb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qntbtvlj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rbpwffcs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vtyzzcfz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vdnpmrtg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcroqouw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2apojjqax.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2gqhxshqx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2navdyeha.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pyyjjbhh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2rorptstz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2tgjpxzlu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ntlrggsv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2eorlnjok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyjfpbcs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gkqmqjcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txxruuha.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mpaibdvk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mptmyspo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jlfkkphd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fcxevfbk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2utswfiof.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bawosbba.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2irpcmlwo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wmifvbtc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ltfuksth.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2aqyuzjhg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2kpvhrcfd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rsutxxcz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2tixfdlap.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2kyhmmxes.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mdnuwwia.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cczsivli.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2miiatdky.html


<!-- 参考信息 -->