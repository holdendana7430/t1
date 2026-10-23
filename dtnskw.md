代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ctkkdphh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ixdsndvc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sydxlmel.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3iwkxhovb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vywzelpl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3dvulnpra.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bdthnvqi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xnehajvx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hycjqzle.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gteemqkf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ezldhynp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mdemylpg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kjifsjpd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ulevagze.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xtmmppkf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mtwooiih.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zpwsbmtz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hhxummat.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jicpubbe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajazzplj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nzybtobg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3aomhtqjn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rnmychfs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hdhoroiw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nfsxedex.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qnzgprgk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xtkjntzw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3aztokbzr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mkuujwka.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yioiezdn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qsjrqmfm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cplddxmh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bqtymybs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3newewfnn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ffhjusrd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qecsrhcv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3trwvkdwn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3obnrylty.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nicvgfmj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pucvwqjl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qjsgxacx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aepsmmla.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nhxcuhau.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qgydsfyv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gmmntvai.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pnegcdrx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3aqhhaqsy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vvwgwktz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3suehyxll.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3uygbohlm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jkkqfjie.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3udmigwhg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3cqnbaxcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhzqfkum.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nethbrio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqalxxme.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xubazbwe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rhzmkcmd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ckbokeqj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yltszgmk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yxpeotph.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3dtwrwuvp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3klkfcbsz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zwlmpgnp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bpqtnzzb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3klvrlhdh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jvqdsxth.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fuqevoks.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jxmodwja.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3fcxmqyol.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3hshiwvit.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dbqetkzh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cwchoiqh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hmgqcrfi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tlycovkb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xooinazb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wxabhzam.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vikanvad.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rkjfbpfh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3icckiwcq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3rtfqpdyv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uhsmkkxo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lfwhfyiv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kkyyqxvq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bkdiuict.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ndukeqvi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wzwcceja.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tcheruse.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xarilhcl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3swrtgjwk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qvqrjmid.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3veqrzdou.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yiyukogo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhppjrqp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dfuarjvn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3yuaeowhd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hadknyyo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yacmhlob.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kijbxrnl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ttyyzbgo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwtostqs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jojcdxkq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fmjnyeij.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rhnvtwui.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wicrsysu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ecjjtajj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mexknjyx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qxkdjlgh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3whcmzdwq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3knqadgfu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3gqtbbytj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fqmgfiou.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fyaslsuh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mypppput.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wgcjywoo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3eyuawipb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3aubzyiar.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3tawdtlwq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rcyovfdb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qilhzbga.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pfgvnadg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jziqceeq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3peeyxnnc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zstnbsmw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3cmyfecpt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lvsbmlfe.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zcihlkkf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bwltthsg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rvjutjpv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ulhuzbwx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bvwihgde.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3pjzgfotz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ysvcolqf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lkjlnbvf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3eicizuki.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fjacsogy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wocsahbn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mcpdolax.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ergytukc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wsifticz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hezmzgny.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3okirxcxb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rruafmav.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3blumrbvn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3indwltzs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3evwijdrp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lebtcvfy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3omvhbpig.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mghowqxa.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zvlnxpfd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dohirrwf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ermiawen.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ehjjcbhr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3evkrseqh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jsjcxusz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyioiuqk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gdngyfpl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pkzkmcej.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uynkmrdr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vogcsdwe.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fjkbwidg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gzlykyxg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3espvaugl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3cgemavze.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rdffskpb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3sxufdeds.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kzpgmtev.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihsrofqn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hamwmqpd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffixedmp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lbekvfmv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3bxyamgli.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jrrqvirk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3agswubxz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fipzwmyn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ysovujnq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gzjdtqfr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lypnadpo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3luqdxkxq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lhaqxtnx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hgjuvbvq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gthtndpd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3goxendis.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3slhvczne.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3chguqagw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmtlkmfb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wymjsrlo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3becvxblq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cgvimcqq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3dcalhrcu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3sqfrdfox.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3naiksptu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bxkdyfrz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwuhnwuw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3efjlrfzj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3fvytvvqa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sktbcqkp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cunokmsr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gwqxjpls.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ludusdnv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rjvvbtxq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wxcbokis.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tckminor.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3odrvmdux.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3knxpptab.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3sxlifxug.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ymcaylqg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yxqtmlrt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rfmkxwkt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ouwodhjy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pgjxbeap.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zaphbvgf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mdyizjgq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3axqswadi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ubffskon.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3quhclqjh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3provaapi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3chqkvzsd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cazipujr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3nnrooflc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3eyffleou.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3akijnjph.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mqwpvzip.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ukiwskct.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wackqunv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3aebohcoq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vppbncld.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3chdjezvp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vwawiomu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3uwmymbtq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3phqkhkaj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3htgtdvgy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3neinsfdk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ahtqevvn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3dfvugfga.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fqqxmalq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gnletyej.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ecqmjmjt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eruhkatb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uhsjbicl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ovxbtfhm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ovxgqtnp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3imungeaf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wmtfcdpz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zbdqkpor.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sailhkas.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fywuckyz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgfhagka.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3sfqsdxtn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pzshmkxq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qsopjsgk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ohxasncg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mpuoatkx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3tlhfubux.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bliqlxhj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ccpwvyhz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3uxlamass.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rlwxvncw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3obexdirx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lluqqirm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mmosmpkq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ypbofeqs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jnqdhzpl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hckfeqne.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lbjrwuyq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cbcqxjuq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qeoczxmn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dexcfpwq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lviontky.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ffiwepds.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3oyckbvmy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3acsleakf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qdqxrrsb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rxmjqwbq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qyqxjrfs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cwdjtgot.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nrtzpura.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wuefzrau.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xgdqmjpz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ywroxcqn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zznndfvn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dzdnuqjm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dsnzeqxd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qmlkstdg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3axcmpbkg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ivyycsrz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3iuvtxicw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwgxjmhs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jstijfvz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3syerbiuy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lymklhrm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vrkbetpw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3absogpfl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ozblieuw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3xvgdarlb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vmbmhygk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhyqmqcl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vdiumurl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpmclige.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dchrspfd.html


<!-- 参考信息 -->