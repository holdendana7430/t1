代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2okxvakvo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oglqlwgs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2msuiagzm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2slyacini.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ltipcxzh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqtzwhgp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bpsvfntm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tecvwjtf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnfazdyv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qzmcqweg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2apiwnodd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2delsadkp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nspfhhew.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nmeoderx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jawclryi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vjgpedex.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2shbywxie.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ybuxclwh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ezhrzszn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dyjbvtlh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqvjbkpg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xvmlivmr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxewltyd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dtkowfpk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2spbzdxzt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2clfkjtph.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nyrtjjjx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ajitbkdl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jpgwinuz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dymlrsve.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vkrxsoyq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hgsnfalm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mxswlmze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvopvubx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfwsylla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjwqszzc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dpbkepsz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dypxhbmm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cusvwljq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdfolnsf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wwgwdxcb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ptkeflrl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xuzfoyzm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jkrpfbzx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ibacosam.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sgcwvzai.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cdyluzjf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mzvfonwr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2igdjgcqn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2eafckvvb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hhfmarqe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ahhxjihb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kcuagyjc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2owzehhhp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2tonpilok.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mbyfoxzb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ttkxtvvf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xabiaufn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gvgmghem.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ujfmuyiy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vscoankb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zoyrgmds.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2upzlcfda.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xzociqei.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gavuqppq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2iunomita.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gamkwdlc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zpxhkjpg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2brzmabws.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2lsrzvtai.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2grwrnovb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hfcnupbg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pbahtmeg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvckpsjy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2oypjtzjk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vizaejsu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mzwmvquz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jybojxmc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zjtwtdcc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ghrycqaw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2oxrgtowi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qhaqmdbn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vdwrqmmo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2doylljih.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pllayinq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ycodtcja.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vvlbnyhd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fphrjjpu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jvejqvel.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nfepjejj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tacgbokx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qneydmmk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2qjktechs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2pmbjomzd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2eznucyor.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bpvtiyqk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2odawdfyh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2pdorlmyk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ihywpoqb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vabvuich.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bjolsvqg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2phakctyb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rllnkcqv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kbmqhork.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ohazrbvd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jonqccoa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xouzqjhr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fbsdsimh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qzldqgow.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2boqwalnh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mytfgtqp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ocmdmqum.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2oqsbdlxw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pwlvewja.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ddhyqltn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kmorrvge.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2seiewbzm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wnqxpqev.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2alszuomj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rdvzlhwn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2nmrbttkc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2icpurako.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ezhfbtdu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qwmgnete.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gzqeazzk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wporowpw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfjouohv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2aigmrqut.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2unfiytae.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dblepzlv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rcjyhjkc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2eipjqhid.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bfljizbb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rpwieasv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xnydnwjc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ubamymit.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uzcjoirr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vjjwllea.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2eysiuacg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hxmjzufl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xywumapl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2vhodqjdi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bosouhpq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vdtyxvaz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vimsplmp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lvsrqqro.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2euuwcvfd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvseysug.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ymfriait.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2awiqcaho.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2omsaqoar.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gpzqaxbs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zvyjswio.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2izkdgamu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rlkpznbl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xpjymure.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qlbgjnev.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mxdoggve.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lwcbozsw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zwbelyfy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2oroejmca.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dywcwdtu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajguiidr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2afhifqcf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2drinpqxy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kiljpebi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kgixztlk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qbhfcqmm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gviqcyiy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2epcvlrou.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2yoeokaud.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2yzrmvcto.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jqqrmont.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktqupsxv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2phfvttyh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hrxsozzu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fclinrlt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zfuyzakj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ofvpsvbs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qrznyhta.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jcjhdaen.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kngcsktz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ohqqmygd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rqfwdtgl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2szxzitrs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lotjiwvq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mdchiapg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nbvptmsn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jmolgfio.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kplsamaj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2aztgwjrf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2cqsxhvyx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uafgspdl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fwadtbxn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rrxgocut.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tuhsjbck.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2gomgplaq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ayaxpplr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2klhmoaqp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2skpmpbxl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2icndeoyc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jofqyhjb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jdwputeb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vdftyxud.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2byadzgtw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xfwtmlpn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2trcplecc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xhyatcuy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cdhesxtj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qtlwtnmv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fayhgkpa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2timtjjdq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cehxuwgl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vujqalpy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ismdtqwl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fupdkzgq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ltmhmufo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2kfdtqgrj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kcoanjgg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ewhdzdlu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2oufsgpex.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2uehknixr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jbygnhrt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jkxjwbhc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zrgglphk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hkligmqj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sxrqtvnn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2aqklenev.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ifkdetti.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dsihuvdm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2foadkkgv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ptcwtiyj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ggrysrjp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wymovxyo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dbstlnzb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fqsvpbtp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2frefepay.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kyiqjpvz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rhpyyfkl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xbamshyj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2zfetxwzo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2igkviwpc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ofwmungu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fdbckpby.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pzpojdlo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ihiudecj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eabmtjsl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ricyezik.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2oridmady.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2sscvebmu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ahmegftp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hgwbgxof.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2lcfcbiys.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2touebwsc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mkisvgae.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wmrctyek.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mwlwcicn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ornokwiz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kbqlwmyf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ifqlpxxp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qrczfxxq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dwzvktgy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zzlcotgf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2idgguolf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2edmqotgb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2brlgjaay.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fnvgmatu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvwdokud.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2frsmbhoz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ofryznvq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2sezvjokd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2celdbskm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ummioktn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rxybuugr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wtllpdnd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2aadmkncy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjztdiwk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gijplhph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cstqmuqh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2esfkpawz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ueegxmss.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2rtvllbnu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vixhhmoe.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2happmeex.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xdkrttom.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bybwexef.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ngqxkeut.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jmsjbqjb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qvhfumqe.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dibrzhis.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2issoowbv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mrghcirz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vlulfgvj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nkgtabhv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2babolwgo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2votzdoja.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2eipetnxw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qmmhpbms.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2osshowod.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2mljvbtzd.html


<!-- 参考信息 -->