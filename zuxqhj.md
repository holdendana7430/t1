代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jnpbazqq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfukfqva.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2etvabvbl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2idgxaltw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vvsyuhar.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ftitnvej.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vjwrtyrj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2sdtednzk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2eyiioixf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofhhshou.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lwkqohgz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nmufbgln.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2haficsft.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wgtlwiba.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2avyljcus.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fwacwtxe.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2siwwwzpz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lvlpvqwm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bqzspblg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yieghjtx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhtzqxqd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gzbsjrjd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yrmsxtsw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lxlqzkge.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2unksjuvy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fmbrpmwp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2najuycfv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ogagxfvq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2emerudgg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2batmjuso.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vzmomiwj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qimwzpkz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2txpblskq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiwsxgjf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2adxmcolg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhsljbig.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ngabontw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kcwekdiv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tortfvxf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2blaeydyd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iyatkgsx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qdrjoiqa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wvytvqsg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ckgiplog.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pzvnofav.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ormalwff.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xzsmiptj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2frjvuloh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ygyfkxvk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kycvjlps.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bpybfcan.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2eictwock.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2egzzgrmt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrfjjud.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hmhjjkcc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tsqafndn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lzogjjih.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qhmtsaqa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gjngrfpi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2qhyzhipk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2byoykkos.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2angpgbcu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nlduzbho.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nnuegker.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jgffxjtm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2csxktoqe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2frqrrkbf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xhzolsrw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zxqkmhzo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tgqnyqmd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ueyxraie.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tjncvcju.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2sboatgyu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2liwswjyq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2lmlvfgrg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hnalnkdm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mctllxgx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jluzxudf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jlzywzzt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2owklrjul.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2txbqjvvr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kpvftmbw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2elnewwhq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zqrmbqhf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uoclpavg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hqzvqlek.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yxnmojgp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lmutdvrt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2fbzjjyqo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rzsxzekj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ujzcvshw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bdzlkoxc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hwnsosxg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2okqpwisz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zqnakhju.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2uoqdneay.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wasjhpmq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2drooaqpw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gybxotfj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2otdclbyz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rxgeakqn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mehyunzn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tqntrrur.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bhclgmbu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qfqhcott.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2caachtna.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qffykbub.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2urvgnbri.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nnsobcpp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2cjjodonl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fgmbgeme.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2coymmsql.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2etaqtlui.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zzmhdvxa.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ebxjbtjn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zwjijuup.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wtkzwwfw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2twyspxgq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2mcugqmog.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2okbkezxk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gcxcvduw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2timewath.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2beaiisjm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kltzkypx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jcoadsmt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nbyswhpp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ownabvtd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2fnbtjkin.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nsjmwmmz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2yjadeilg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hnvaxjtt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkuygqxh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2givnigvd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gxgzmjkp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cjlgvuqo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knwjpano.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fgrbdsvi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2isqpuwxr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2adobabka.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ytrvgoml.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hsydulbk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jhfsqlhs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bgygstop.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qrqdhzjd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2puvcwpjh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hedavkph.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fdrrdkbg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2etmjfsud.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pzknxltx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2khdkcskc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2aggrzuke.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ndhljojd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kzznilly.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ztptgeow.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wlqjzzqc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mqoxqlbh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dqmwbqqf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2znxxkriw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2hjijnypv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2lezhmiij.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2znxhlkfl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jeshvbbr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ljslizxw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qfgagssj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vhekiqsw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2guvbnjpd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ouqixviy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2siwqjskz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vqhyzhxi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rsbszppc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2agnmuywf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ovsganpg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bcclbjli.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2iiinzhxt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uwcugvek.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2umqoyqjx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kwzunifd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2iarvnyte.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pdgvqmud.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ocgzitso.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vsnkmtcm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2trroevqg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cafafiqe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lsrhppce.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2yznrkabz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2getlhnuw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2euvceepf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2oxrnvxxr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2itipkcdd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2iouqkelw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zgdjtmdz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2blrfnita.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2vrgnzyzv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2flflfspf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fpkggdka.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jlhaiwiv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wodlqdnf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2cbhvxank.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jseozsfi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pxriiafp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2oltmbgmq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ocvvqqhi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2sokhuuwe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bavzsreo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2wnlgjdzt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xhrazlen.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2rdptyxcs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vehuronv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2eszsirtc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2upgctjdy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2squgojqi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ommtqeke.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hwsrdkrx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dpwklnwk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2snnvbvkj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjfllnw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sfjtclkm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nraewpis.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sycjoaow.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2prdvtqjq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2spwqwfvf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ihrywjzg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2esrjhixn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zefebxmb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2cvirhutq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dnlztqfs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rkqdrykj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2prhufnjj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lkrfdped.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ddykcryd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cbovjhtw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2cqatrlrv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lgiufldq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bztehsuc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xnjdzsur.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2elopevbn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ywkgscao.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2zdnugowg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cgfxbyez.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ggwqjhwn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ualffckm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ebybjrbq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bwppduky.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aetgtgsj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tvwtymxu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vjsvryjb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2glnsjkpj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dyeogpfg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zuuqswmu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zduzojxm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2nwvmtmtk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jwumroip.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2pxyfdkjo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2srxrzpzu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2eruezgzu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bbkkzziy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2tgfhwyts.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hpregumj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sxrqjxnx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ypntvwqb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qdphbzbu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sywektlj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2zkoqqogy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tozllhbo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kcgjusdf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ytevfgjc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rmkglbec.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xykjvjif.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zhydiouj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2glzskhrb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2cmsdvarn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2jpqeyuwf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2jeouolbi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2fplklcjr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rhgiygjz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wgmdvdoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2soxbrkqg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2rqjhulhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzmblaup.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zoollvrm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ubpmdzbz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2muaslkbs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kdoqcppk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pnrtiahx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2emniplfb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nwupjdwq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fyjinxvl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2omvhuzam.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2morpewkl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2eabroqmx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mokhwfal.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qznmxvqs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lloylxav.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2tlzhvqio.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2lhjigiqk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pxzmqoky.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ycqvxvgx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fskjzujo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2kuunvoyp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fwmouvpz.html


<!-- 参考信息 -->