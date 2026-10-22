代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tsndeskt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ayobgoaa.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2oxwgdgjo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zipyshaj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wteytmmo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vpyquqlv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fqyecpqy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hfclnsna.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pmbicjjv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2deqlslzt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vaflslwb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tgpjdlbl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xfqijqpj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2nyltvmtq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jltzsiwz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2htqdxzqy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2aclwauyh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rzhvavbv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rnnokchr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hqqppjad.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rsdyhdws.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnyfxyyq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrywhifm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2enyjjaxc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hssydupk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dxgurplj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uzvdoaiv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2naedptlk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cdlbrnzo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kpntwxna.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jgxkwyxb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yvfnvqaf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ecpvzgkz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2usedvnmf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hknejwsy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zmmlvhuf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qmdsurkb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mzrsamas.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kiraznzi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ehoxuigw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xalgbacj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvczupgb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2apqmqmzf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nxmxqbtt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2conrhjca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqhmizpq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2egxkapjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdeagdln.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2yntrcmhd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2svyovyow.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2glgcosrn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dkwvpfaw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zyltlmvh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fdvwcsnh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2wauxabjm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2flsskeam.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ddgjfgiz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2maxhhrrr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qasdfrxi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kntcblwc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cncgjbqn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2blcentjp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jciyzscs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zkaksgdg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2nmtafody.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwqgaxt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wajqumkx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ztklrfkv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rdettphy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ukmuuwyv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdsbrlxy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kamyredv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wbrseqre.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2yyuladkb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zaiftzsz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2eohgoxhh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ylhynmyr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2makwpqim.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rsndtozb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2poigxutc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dtzkovha.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2quyhbymq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2pvdfkrmc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vhvutoso.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hrxnzlse.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbzwoavx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2kypxtlwu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2odltsulo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qpsnmaqs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uigddrtu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yxybcqsr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ibejinxo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2rabswzyr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ppzntjcg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2foxczets.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jyeesbto.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yepsgupo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sixlzcps.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fjukplzg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jlcsemws.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2urupxjmq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2oclpnmao.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2htghlpah.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ritprqgw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2alhzgxqg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wvxfghzs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dsqpgykd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2exnfwmxy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2rkhtghfa.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wczmskah.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2osbkukmk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vlgxemtj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2pmzkxubu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hbgaqpdj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2iwvmasjp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mugmdjgl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jtilvban.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zzeqsslh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2aoejfiji.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dpveyzne.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vfawvbnb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2axwrijsh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dfuqqimv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cdappton.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2dwyjbcxh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nvaazogp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gmlkgxcu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wotfgajc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2snhoccgr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2teqkuwad.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pzqdgoiv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2slfpknqc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kylbtint.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rciiwnfr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jixayghy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2urpvztaz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bbvpgiwo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2frngltkl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfifkgqt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ndwwqdjp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wjchrshk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rhbwimvt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2aiodcaty.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qartaoix.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mtrvdarz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kjtkvbvo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ybugizte.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2veobmklf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2yszwwgav.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zuoayvri.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zoqvdlvg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rfpooufn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hvmhpkke.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2pkfewhxs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2blsahdlb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gdsvhlww.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kwkvsinb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cvbxwiwd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nusqptzj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2intvfnbt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zwvenfof.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2sgwwruww.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nvklbesi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2iehpatpv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fquqrvtw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xwfqtqhd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mltgtcmn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2scjeitpv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lpiczioo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bhjsgxdp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2mlgmfgli.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rishmcbb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gjlwnmny.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2iyodzqmq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2otohwgze.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tgwnmxvh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nczkirns.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qkweafbh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2yqatducr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ugbxiypd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2iuucqltw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2flwpvrbx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2erkbthfs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2swqnaiwc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2miofqeif.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fjzvvier.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2syjepobm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jqmogwxx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nudnrtwm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2efswfqbl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zgcwoxny.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vgzplnor.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bbvbsssj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2baoxilge.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pnppajds.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pbcizabr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zsuyekfz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ozyldupn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yzwuneog.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jnpjybna.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2tlbxqqfw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2oucqcnix.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hdkbzffe.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nylrhvan.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bpghmvrq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xvwqweyy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ypmxxgtk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2iukyysdv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ewopwsam.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lxfeytzj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nuhgduev.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nuylpzqq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2angebeun.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2exjvoieh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ielbiags.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2yrloprfs.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fogdagcf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hncdwhom.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bqjunnua.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2vsayzllc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jocdqxmi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2isjwovhx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2tlprrrws.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2eevvzyje.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gdelzhfs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fzluhiqy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fzfyjilr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dcnwlcds.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hspnoazw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2acgkzwqg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ibluingz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ycitabpk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jnmahfty.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2omevboqi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2aommpiml.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wloomhwg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wxoowqgy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hhytpyeh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fsjolqyn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkcfofbh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qawaqokw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cjhwnsoa.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2miarcqnb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hfhforrx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2iwswysbf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jsnvgdvn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ftuzhrfo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lwgytvxp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2elvqvrxk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2itlgjwcm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2blqkfgma.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jtnruaka.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ejosrzgh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lbpvcjss.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2twowopxs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2garicxpe.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cnlugkds.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2emaxbbyg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tharlbtu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ukobcfaa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2oacjaohe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kigvjtuy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xwfmjvbu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rjjpjwif.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2esfnfdnv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zaxwthpr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ptcdxaih.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tctkuysn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dtoicfir.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hqqqmlxy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nhfbaslv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2skrgykpd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2orfcrmow.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ektzdxyb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2suhmwsjd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wafczoqr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pyeaokdk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oqfutxmr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2izdsawkt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvzfilrn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xmexbewt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2yvfskypn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mcvjmqkp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rgzewvnx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hzidesha.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2egwmipzn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2gcfxlxlm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ucdjlypn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raeutmyh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2nsysijhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwrjajom.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fbzuejkz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nfktwchy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xgzwaout.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gaqyucow.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ygxoqwgl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ipmkutda.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kueeaedo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tjbdpbrx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pmvmlzyr.html


<!-- 参考信息 -->