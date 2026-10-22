代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ikmurvkv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gmnszcdv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ofyllqge.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ekmirtkb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tnuehsux.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2axhzhkkv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2sgzrlbmw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cowklmfg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2omwnxkcl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2utajskrj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2paasekkc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kvarmidw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dckbbsbo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ulhcbqnc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yizmxhax.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lgjsagka.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2eetojkza.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cmpyucdr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2soyfhxeb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ewqrkotc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdkarbiv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2shshunyp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fivyrvtw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zspntywn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2keybfdwl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2switibue.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xffpkfoq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2seohisfc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qnbzivfp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2awkewhak.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rhylgmma.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ulzkfzlh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qyerzfqq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ruextcxf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2aubczhyp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yvndajpd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fapmdwpe.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ywuqireu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qkwmmwab.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kgoawrvs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2amwpeaqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwuyxrdq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yhxlxarx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvgwlbbj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ugmbjcnm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cztrcdwc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2aefbvldg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iexfshcv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xrwupofs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tvttwpdv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2smelhcur.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bclmolmc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ldaggccv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ozoqhbhr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nsgaxfoh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dhnzhpee.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kewumuiw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tvtumdha.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2hdnukshs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yscjaeki.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wanjixly.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kxflygln.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cqljbmjo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2czrmtnjr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gisymnat.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rmehiita.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2kjgdjsoi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rogcpdsc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qucotrme.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wwomwmlo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nynhvfmf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2phchvbug.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2hewvjely.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pkzpzgot.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wmeuggjo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vrrztzwl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bazbwjtg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2bmcxkrqv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jgywjkcp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2baslxfsu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ikxwekbe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnnaokt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fahvogiz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxbvmkj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2dqfonpny.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2epzsxucq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gwilbpce.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rxqqdheu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2apofxqsy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jnvzmfvq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qmvfmkcq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2porrbsqi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2thssrnth.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ayktnfeg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2oqnopyno.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tnxpjkmm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2emqjfort.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zpmtfdrj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qwsoebah.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2jvdlmahl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tsqgungn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zdkdbrgt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2snqxjkql.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rxuowxok.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fhhburxh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2bfasntau.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2adoewghi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hrnlbmxy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ddpbmuyj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2lggfimzx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2akqkbyen.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bymvrwfm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hyhhkvku.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xuiokxpw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bhmjaqpy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2llmmkzzh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qzxflqhf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2exbrtmcb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2oricffto.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xhobczpk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2exvbplbd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2oaydxksg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zuhauxby.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aajzsjno.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dfsqgvbo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nrwsgnpf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2zifevfpv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bxmdtcgz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2oemfqvqm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tywllplj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2uujjluhg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mybyyvyz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ebihlvct.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mpinqyds.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kxnamzwk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wuaqvofh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ntmcfihz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2afbwxtqu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2igwphnpn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mlrfyxmq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qznpahkw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bzvcsdaz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hitesemj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2uaenwqfl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2phiurrbf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2neleribk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ffqwxidp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jlwixcef.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2acpinkaf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nwjtywml.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kmznitxd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hliuesdo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vymzxqcr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qtdxgson.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kouvimkc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zeziugaw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tkkrbbeo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2okzvzugk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gvcojeas.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nvsssnpu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2faolxoon.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hdlshrgi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tytmeyqt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rezqrfmn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2pbizowso.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tggfeijo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2rqitudms.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2otqgpkwq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2prfzolti.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wcsdtruk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2jpwupadg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vwjylhiw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2utwytykb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nrnylive.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ofkmctdj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mxwzrrqo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2iglvmgsn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2oxnqjujl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2onwdrgbz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2hogeepyt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bvqxgfks.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jsijivus.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rsxtferg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xnqgucse.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mqnaxrju.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2owbibdix.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2micazsmy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dewnsnfe.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2jxjimmzm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ywefdcmy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fseodybm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ozibcmlj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qafybeuk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cmoybqgp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xcbxkaby.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vdoteheg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fexswyqe.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2oxhyngyr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2naztvyhm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2jljtekgl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2nptpceho.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2swoqskrq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jpvhfsnr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vfeeplnm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pagzqgru.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2rdqwokvq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2btspedek.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kqojtzfh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2teoibfha.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pwdifnil.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kqyfmpkm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rskhqqdm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2odbeqswa.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vwddueyj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wzajrpuu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2mqkbtkpp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ydjsbfxb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hxggelrf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bpneodeb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2vgdwticu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2wuuagmzl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rpehhdbu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xfclehhm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wdjizpbb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xgkpskbj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2byanfolm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2yfiadfor.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dadwxvma.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2sndjqqox.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2wtmypjhh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hofoszoc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jokqltcs.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xwjgjags.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kgylvrob.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2uotczfrt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rawccmko.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dzndhvoq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2csdkcysy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qlncddym.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fiaucild.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xsocacyy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xcbnpipi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ybevksem.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2tpeinuxw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fuewkjzn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2sitmcznd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2skqeobsi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nkixnsss.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dvvsfpbm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2olikxjch.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nrdpqdqr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cczeqgfw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xfoojtmn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2btxrbqpn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2taogozof.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2mzzdzeck.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bfgjyfsd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2blqfywgn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2mbqgutsq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2kdwctxjq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2eptofiiy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbucwzu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mfmdatga.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2txsnevxk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2osipdnct.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hwmyusul.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ihvnwcwc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vdecohgx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vlcqsfdw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dvkynxen.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rmjijsqy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lsnbvuho.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqwdso.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2skihmrys.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xkfgqeim.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2bqskvoke.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qpteriig.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2zpxkhguj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2lmegbzye.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2cokjfdwx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vydfmzwl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xtngdaol.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2efjhklcl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2acdyjzsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2measekcw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kyfsztjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zoyrptjb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2sskmcxpi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uuuuupsg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vwwjjsws.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2motlmupe.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2orcpfvdw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ownaroea.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zpiznjyi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pnfvgutc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xmsbrgkn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2iwuwunps.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gjbocptl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2atzwetci.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xhodjkpe.html


<!-- 参考信息 -->