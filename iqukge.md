代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cenkyqfc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2krdlcbow.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fekobaap.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gstnvgmw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zysjwokn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkqrmmcs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mwgnpkyf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtfugyef.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pghipbfm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pzsksbzs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dlctzocj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pkjxibds.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qxinllow.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2atrsxgrq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2msvptojq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fdxtanpp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jegvicqj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kotblsmx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wbnumvex.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qyockgrh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lgqtxddz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iilhsdub.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gjeqvxlq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gdvpkyyx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2nuvnmdxe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bonqvuou.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntzaerii.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2isexalxb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ewptwdti.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uxjzykkh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lfxsnsue.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zsexobmd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rugfowqf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zdkktwgr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tqtnapua.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ylletswb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vhsecmll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttudxbnn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wouorvwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xduddgae.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2evdtspzg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vnlwpfld.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tipyoyfs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ybgygdax.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rsxqeneb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2alclhthq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zpcjqgho.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2swhfiqmu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2mlhaxtbj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ictdpcad.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rpfvygqc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lamakbsn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2yteyuabr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jcinkptn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2nxultupo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2sqroibrj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sijoblkh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvjzjyc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2mvacxwlw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2irmkkdbl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jkziigrq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkmyehvk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gjukyklx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hfekzidx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifvefjfp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzfvjmt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2moabmrfa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hopifrqt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bfivfbpk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vdboujtj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2eysgrzir.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bvkvvqjj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ftngdtqp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2oshzqreq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wayrrkki.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ktcjvqvs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2siytdpnt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwismfce.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lmkujdxg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uubsgvrw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vdbosgyc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mqtytsqb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2iuxyakuc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2heduqxuf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2bczwhenz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qotskimd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zlwuviqb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2whtilruh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hscageyd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pncogogf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fcjmpbwf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ezsgxjge.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qsyoagca.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2nxayfska.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2okugssjd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ksurlkag.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nfujkkzg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zwyzqwyf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qnzieaub.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wwkdxnja.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mqhcemtj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lcopvhez.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pblghabd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2javqboyj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2eruhbrpo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uooizacq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jjsgskae.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2iwtodypd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cxgllwhw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mlacpbge.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fqpepfvy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjrrmss.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wzxjemop.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2oogzhvta.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2arggistj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tgbvecxo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ildaammm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zncyygjc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2tlssodxq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bazbyvrr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vkzoxcmj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2bhgevqkk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2whljcuwv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2omwjqhtn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2oxghszsq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2osffziae.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2asidiluf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gcozoehw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2owllofqg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2frbmafsr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tteuwbqv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nuyotqax.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rpprbios.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2stiolrvy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2akifaxxv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jhuyrsob.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wwfnzwnf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nfzgpzin.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uqkcuurg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xwastyga.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gtjpppjz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2oxkdlezj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dftzlwyj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nuisgksn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gthpjhdj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bdbruogz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jukaqdqq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2omihjvoz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iqfwyjda.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kvhherce.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vkgwombr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2engmsslw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ilblyomi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2dpmillzk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2kqnjtwwd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2atjilsnu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2nmrlrvoa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lswaflqy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2swqiptut.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2amufvxft.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2toxxrnqc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uurmogdk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2uuvksitx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yecpwhnf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2uvelabzh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2tizhjqjs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rguqwrqz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tfhwapix.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cukyusvy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fbuqtqcb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lwubdviw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dabyejlc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gphtfptw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hjjcvbaj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kpaxamnh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vpgaqvka.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cafjxsmy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ytzfzqrq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wgazqjdr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fkmgdune.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zjilrsaz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zirbniud.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2lnslluif.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2otaykxxa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ycmnnsjw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gwphmohc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mwquptyp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2skrpujmf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xmlcjsum.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ejxffrqb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2cqkdvxjb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ahymasug.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2tulfisel.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2efvwmwmi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hqzqsati.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2oesclxmb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bgvemrfo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ntmvuwpl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ssfaozik.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2uzpdhdwl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2szhigbsm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vopisiqp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xjbiwozf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2sctwukqn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xaekcipr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2etvmuhpe.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2talbzujb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dfvrwuah.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2eqqnfinp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2huqjvtqq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zwuxgtcb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lrleqdbm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ydhcdbcl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dbodqnav.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2gwdrbzgl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dlvvyepu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ifwtgolu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mnuceuok.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2auboszci.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xtyrqamu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ofibexiw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2zvefonsq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tvoespjl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vyiigwzu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgxehnlx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qpeofyma.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2unfimnqj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kazlhmqf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zbqdsbgl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jnjidczv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xfnkfrob.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ssbknofv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qwspyark.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2luhhxzxv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qcqzliea.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2esigscks.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2foyevxgl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gxvolvlf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2tbpqumgs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lqqnavnz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2apogvhis.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2cixqcmir.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2oniopmxp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wejwbitm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2bufohvxy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dewpraee.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jxljeqyb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kiwnfqhf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qwozxstf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dsrcixww.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2efvkuezp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ihjaeihp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ydnjjrtd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhzoqay.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wubnffwc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ergeyjmm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2unoouqqe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2blhyhgmw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zryiuans.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2inhtbnpx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jmqwfhwx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2qzxyfbit.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2itibulwa.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ntxkzdlp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rhptypum.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2igjcskhe.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2neqnfouu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2urfgsjkx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2agovxcwi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2foeshehh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rueoyakq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2pahozzkf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tmuayxcw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ubltmjlk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2bzcaiacz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2paiqncje.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2boyqoofc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2yzstxhos.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jfpgmuoa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2kbfcwpii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ropeszds.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2rrxhnhiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sknqcped.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yozdnckg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mhgbunak.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2mqwrgglw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kuinwsmz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xviqyyyf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qnzbtmop.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rplxzvyg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gzfzspqx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ogjbxhhf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xfubehae.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jiupfgzv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ywrlqjee.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2cnodgtsp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pueqrihf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2voovcdjr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2jfrvjckf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kdgnlvmo.html


<!-- 参考信息 -->