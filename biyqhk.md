代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sqewsqxj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xdrhlwux.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hywyndxd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffmgnjpk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fuyyxqbc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jgrdezzg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dlccznve.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssnskshw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3htbasofz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nrsfbjvi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lhsxfzfw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3btaocjff.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jrcmckim.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdmqcaxa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fixdjsno.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3tvvumdgj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3efkxntzw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rxbsnzsy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uipnmwbx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ijgptyix.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tqsznpkh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ieejptcz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ihjybcxj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ylediwzi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3prjkmcka.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3amtiwdao.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3frbqpthf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ieccavyu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hntoydms.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kwfjnrlr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdifnbch.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3swinojft.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ubpldzog.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vuzjpbwu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qmmdmzlt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jynmvjry.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tzhrvdzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hukhwhnv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cdvxusro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfkptcli.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zihxbrav.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3sgmwsoti.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3chnrguyl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zvjnjkuf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tkjrgnbd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3cuhupmlw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jmmrkblv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ybnvzmze.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tqhyvzfr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mqntvkks.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ptksxgeo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3txorjjfl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vzvmxwux.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qxdfsfan.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xmeibfgf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3djgqjvny.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3prpficfd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vhjnixuw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3frmvdkkw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3spgckwkt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sgibgytz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uchaskyi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zepbnruf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lddqxnjm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xldmukce.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vahcrdkk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ebvaytep.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3evyfibxc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hxpwnihr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3elcuhqbv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3cmbgsmmb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3uzdgacqh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3iyxzpzfy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zomdcpip.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3aqihiykg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3aylgftym.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tcqqwhjx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtxqsqu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3iwzakuzb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3uhsuzfvb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dzburwzf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3touxcpbh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hrfcovrb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3osoevect.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3imddvrxn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hmxsojzd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zkjcfgwl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vailwmvl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qpsmwryq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxlnprf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3loggdlaj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nnrmkewa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3garhrykq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3sgjnibfd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nxnfipjl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yfmuugzt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zkeprixx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lqlryyex.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3htjihbnu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ksazkstr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nqpuyxhz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3knyhsydc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jljmjqia.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gzvcrpmh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zgkinvwh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jdmaikus.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cnraxecv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3enwkfswb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3khvwngdn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ngqzjhuu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uvlifpnc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3oxiwtzac.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3cbgitgnk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dyqfdoit.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ptxflaqb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yxitwrmj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kpgebkfo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tlwuckid.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ltqqlolj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlviewt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ryjdrtfk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kbcwdquj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rprndeos.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nngartdh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qtxghqiz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ehazcyse.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3cgsnfvor.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3sqnixoun.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3opgluvga.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyknaobu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ompwckvc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qwpxnreb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rwzjecbm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3lkhufshy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3froxuwfx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3uezrnicu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ganiueyy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tmhamqry.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3bmagawec.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pcwvwsma.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3puhsuhwd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3murudvhj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zzsxdkjd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3etxhlurz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jmjfmscp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3fpyajhpp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sicgwqbf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3khlxzond.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ikwkhqdt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xqqhhzhh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3izajzbqy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3druxfqyd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3guzrhmcd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3afmbaqju.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bidqcegi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aszjzjlm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zbczqjkm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cbwzahby.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kacqbxat.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nmtxdnve.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cdukmjrp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3knuvegpg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cevwjwvn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ueqjuxkq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ahrnycds.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gleyrasd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eqekvlav.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hodkbdak.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3guhrxvoa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gkjkarnw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3iprrndca.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mhbkbold.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3snqjcdyn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qhbddnip.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cvthhysa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ilxkqtxd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bkdvycth.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3usfvnndp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3fhljpsqz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ihtmwcdq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ctipcvev.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3klfkjrwi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3tfdwtvaj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3fnocxwyh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3tkcvcusp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3aynsgxtj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvibynau.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lvkgxiko.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wpfyeixr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3iuegvqlp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3wrqhyguv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zmloxsov.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tybfxkwn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3dqslqobc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nzmnafub.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ndniorhn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3igcbelwr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jqqfunhg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3onbqdesp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zqrwslog.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3huedadsr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3mhltthio.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3anqdrlzb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3bldtksms.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kxdvejlv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cdwvmtld.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kypqlvjq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yfhrfrke.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3saxzbxta.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3yqusrpyl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vlcnpqpw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lktwthnv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gjuzedvz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3trndkqfr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zluwnnvz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jojxyvyx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rprjcmek.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dfdsopkp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3akqyanos.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3avpaazeq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rpqyrmzv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xrrstikr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3swdboyqa.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jsnavvjp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ouuohswb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kuwzavdo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fmvleyti.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jbgtuskb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gctxttwp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3brhjicpt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lfufipng.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqeegcas.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xruqxevq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3htjkaavj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fwjzgfem.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3brnhheiq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fhytvqkj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fcqmiftj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3aenywnro.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3oibhovxj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pkzncica.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zdhccohb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ewhxzltt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yngiocod.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3egvfbzyu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3shzlzpms.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3abmkmptb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3newyakbt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rugtglzh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dnecmjzv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zpsqlqkq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3pcaqzumd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mjeweydu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rcutjjlr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pkmhpskq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3wrgxpsbi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ygetuszv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3igympryp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rdibdttl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3vfcldewy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uzaizwez.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gbylbwoa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mvcsrocm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rikvqeyz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3sqzrmfcp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qokxpnaa.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nxzcmvwh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oondguqo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qdlgqswa.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ndidfkdo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qjanjpwt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3obhmtksw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3warziaro.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3yajqtvdd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3uinfzjvt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wxvuonod.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3oobkchli.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3acpovohd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3gjttcqpv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3tylokgtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awpraitq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vyeclhjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abymmgbm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qdjtvwyp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bspufhww.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rxwrcdbj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qffbdwir.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mtqnybuh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3soqvsuxw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jxmaavjm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cuddzlpm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yaaiwrpk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3atqvwxje.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3quhnwvqr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gdbigxer.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3uetdpuzz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tluolgls.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vyotfjbx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3wbhpgrpq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wmmvejsl.html


<!-- 参考信息 -->