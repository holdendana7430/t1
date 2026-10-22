代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tofmjjhu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2prhwcfum.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2emvlsmue.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ecqwvtoh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hufivltb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ephxupyx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wsshkdbx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qtidppoz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qjtaivrm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmgfxtzo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zarexxvf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gpgjyesi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cldthndk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gikbmucv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gmbgshrq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mmxcypmu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmqvazka.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kiyzvhpa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2truoxwcg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mzirlweg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vitjuobm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eebeoney.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qegzblrr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fqfpahbx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bnsmhwdg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nbhagjjd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eqsvdmmt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nlroxczv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rfruilfq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2isogmfdm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvembaxo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dfvpmhtn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uatcrann.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vloarlfa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oivjfcwa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nlvrboxj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2efnnxlpi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2eofyaeyk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vwavmwax.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hdlybvay.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2thrvufmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltxfwrrn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gthmlrlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2roteznih.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2afadqtvw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2weuzdfbi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zgivwqxh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ciaqejyd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rmuynpwm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mcjtdrdo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gmlblfvo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ivnpkmpk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2chvmmspv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uolaxpho.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pelssjkg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2erjlgjig.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zngztbog.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2eafksapg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2scpziazl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2csjgqqqx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xkyefjgn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2guhqovyc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tqaeukac.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2sjojownw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2iwfbfnkf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jurbarrf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dgiagcjq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ehoevlej.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2htxrjcwl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2clecmbnb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2blpawpgk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pgarxsrk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2revwhzup.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2rbqjbzgp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dftqmmka.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2khimqpxx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qkwkpqyv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cowutpau.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fovjjnqn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2micglvrh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2eenynjug.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kpmszueu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ycuyweje.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2srertlrf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nnnzzylt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pabadzzk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lxvbhzov.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tjqccyey.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbkjdjka.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2tlodonuz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2eppqzqje.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tjuurmkp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rplcdtuu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2quzrctfh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ewetslqv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xmjrvrfk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jvltuvjz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hamjqwcr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vtisbfom.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sbtwaygw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2roejwvrw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bamejlho.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2raaqdlit.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vwoawijg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2skpxqnit.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vapnfnvk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2muoayvxi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kygwcwfc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2skhyczbb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hnfomgje.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bmsrvlar.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2iupxeiwd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cspgwexq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ebokhpls.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rxtufhfg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2psdelnsq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fomavnqe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gztcfyaw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nfwjpwad.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vbszdfaq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pzrnagzv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pxdbsuvj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lkxevtcr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uiileoxa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tmnecfwo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nbkqpgpe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2yberbatj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2czupccmr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mcagkdeb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dgwyvnpd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2luiovfpm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ehgznfxd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2oiadaggr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mtjjpeag.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nehbadbt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jdldpdge.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jeidygzv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bxnioaxl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qgndvkhn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ofultfef.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2fcsykkfe.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2sawtaxnn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ninnywcz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vaschypi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2clumganm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2vrsnfina.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oocjzyqp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rmbotenp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2fegdkqix.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jgdxlswc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2dmkgodtn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qjzwihbt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vrmwwqsd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2egzragzn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ekrykodf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jxeubzmk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qpoivnzh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2focejhyf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rgjsvekj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xbsnbtqk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wuijduuq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zxogdugh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xmkvjmyf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mdxrodew.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2kotxzigj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqgyfyfp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2mabzlics.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yabwayrl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ktmajijp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pzvzlqjo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sjfetrpr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2sqrtdszo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wzybxchv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aaemvuiw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2avkudgbv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eiuqtpog.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2dtsoisqk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2kfximhim.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xdmnscls.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gpoazoki.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ftbkhcbg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nkyuhlvb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gazzgvhp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mnasvjah.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fntmbqas.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2axdrmecl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2urnnqrcv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wpurylob.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2byfphlov.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2lwfrcfsx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdvxtivj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2kpsaykiw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gavoqggz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ubojvkil.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2gnwppiho.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rinjsvrb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hzlryhto.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2oxyhjexg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nrkaztdh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qajjdwuj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wyurdmcc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ltlzbsiz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2quaconde.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jqfxrwwy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2hwcyvlag.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ngsfhxzr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2nipzdrbw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ohummezs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2oxdxjfsj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sjahrwhj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2lvogokvr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ihdsjycr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2emulbcbw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2eysgkuih.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2tjhamxzn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nuaotydb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jwffousb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2evwaggbk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gncmbkvm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rfhztorc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lejvbgyo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gezyraoi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2irbtfvpu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ibdhdoeq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2svwbjifu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ieqvqoyr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hbnwsdpl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fgyovyxo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2uesfqevo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mpejrtfu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lozwtjey.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2aevnmcow.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2funganhu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cphbnwsk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2oqhkstxg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnfxuegc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mysjlvlh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2imlumhnx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sxdjuxth.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qyxiemyz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2pgetbsju.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bgyrwgpg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bhhnpyfs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2cvwymbji.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2tnxgavmb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mhraklna.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2bujlgvzx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2uagakyiv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lxugenag.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pofjaami.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zavsfbgj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pjulaoab.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gzovlnph.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2piysjupp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wzywjywy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ghnpqlqz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kocgkijh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qsvohcja.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2omjgajni.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2amhfzoxd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mpcsywzb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jzzllldv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gjxcgnil.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ssdttxuw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qljbiaiq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ltefppri.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pmbljxpo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dgzuqwvr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2huobocei.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kkdjsvyf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2duhwryrj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcyqewe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fxbrdkch.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wfnufmiq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gahvbswy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2eqqseatd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lduqmtpa.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2dkuhnhwy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xyojwuba.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xfpsaxmu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2damdranl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2egodfuka.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2oemefbiy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kdthnhfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glbljigb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ksxtsyhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egobwkme.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2gxdjblhl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tqqgiuql.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ezsybwfj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gkmnqpvz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2myfzoxiq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gmvhqzvg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sjeflzxo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kpacplpm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jxbvavoh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2lccpalkg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2qglxgdgc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2uyzdknkz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2pkwddfnr.html


<!-- 参考信息 -->