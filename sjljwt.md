代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2abiehorq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2scjvckqh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2aodxqcar.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ctyuelhl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xoqeglxq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zeomdgxj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wkjlmoqg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mfkxqtdi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ipmcotyw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2alcbvefi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nevpevks.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jsxkywyo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2idmseuvz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2quyzztoe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ctgineyc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2keghfazo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jmozttkz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2twvrugbq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bfbchjbx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2otzhlftd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ypjsijcg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmualnfx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wyxzyjpg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsywwohm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2miwemlcm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruqcsbjb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xewgjujo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2epvcmloj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gnvflhax.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2meymimfp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2shizhkdc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tyrqaiup.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbhcmdfj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbskxeop.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lsijlobm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rijedqsd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2uqdwkovo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2joufeesf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ifjcsjqb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lvwggojs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xopmeiuf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ucfusosc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jclvfqlz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2affldsha.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ywggmpbw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rgtiyijs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2svylivaa.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2doxnrjqa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zqtmleyz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vingxhlf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jnprceun.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2egejzdnq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zhfrcmoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqkkpohl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2atxvncjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxvzufxb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mqmsyjjg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2eqfrzpfl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dyjdynyl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dklwaqag.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fpbkurjm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ahfsnqdr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ktuwpjsu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wfhcvfme.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cnjhfewy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sqpkqhru.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wavzeyod.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yfttzvvr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qeufgrwj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yfilorvk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hebcnkbm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fpxuthzp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2juonhzjr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qvibbmyo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wmcqabuj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2shumqefy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bwrnemdx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iuhdlwge.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2uwqdznho.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2qpqmpyei.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2myxugbvg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tajpjegr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jiqbvqdf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wglrjuih.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ocgnbdzt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zggwpboq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yugiptxl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2pduipptw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2qgdgoeye.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ijzdkgto.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2yczyxnpy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ihrmszhz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bysqclcy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ilqzcbih.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vguucfwg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zqlfbgwd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ntvcbykz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xsgpfzxw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2keobymuo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2hyyngemt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgjttsmr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ncsbuweo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lxscxfar.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zfgqmnlz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2czulrbtc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ptdvqinv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wleaqrmx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xjgginwx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hqclkpfx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2dbxpqteu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2cwblwomp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mfrippud.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2reijxzlq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2omkhypic.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zafxyyvx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iwihrask.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2slkjgbum.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2agnqwkom.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gzrviklq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rwwpxygu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xkbucnhm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zylojooa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2imlqkewd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fkiqzetw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vnpqpsnk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pcgmomwp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rpzzrroe.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mgoenwib.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fpriyhfw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yynsyfxw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2aqiijnkm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vakcztee.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yejxmoox.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bsnxtuvm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2heoiqcpu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2owebcrmp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nfzmqfdy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2sszssgqg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nhmozlru.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zpcxpzca.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jiwanqvq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fwjeonqi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wuexvskx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vlvhqpap.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bacbvpas.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2avikilvd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jeedvwdh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2iimbglmf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2eenuegfe.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wdykucae.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xefgjtja.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2orcwxeox.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2fechqvci.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hnbhbgmp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xmxktzhq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjdjpgsn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nkzyasdk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wjvvbvnh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubskzpfs.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zytaqwql.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ksppsfod.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2auznyzcg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2glcryprt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fwiguxwu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xkglsayi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qkoonyro.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vqaokkka.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kqqrputf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ijrigxnk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yejgiyrj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ehpliteo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2envpqhks.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mkacbosn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bbuljxxd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wgkwbbzv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mlhhidin.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rgymijtt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gakleflz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2neqrcfxp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jcnemcje.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yuwzkobu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tgrwvytx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zjvikols.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hfxresrg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ugvmaxnx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ozinwmso.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wnetvrwo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ivwiauur.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vpamxdit.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2yyjezfzd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2nmbivjwc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qilrjxoj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kovcodlj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lvasnnln.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tecrzomu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xtupkxjg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oubmuscv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fwxuihme.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2vdypwojm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2myshzbfl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nzdkwrjz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gdqvhsbm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2flaconoq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xcfecblh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2arrhhokq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gseaqman.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2dkqkkkyv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dgrglgfd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bqaeamiw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ifmcgclz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ujljjxzc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hxcgwssm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2uahfhtgy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zfyismtt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2rrntzjds.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2edxrbhyc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2etmlwjbn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hdvldtnk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wcssmhvp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2vamrbcnx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jcujxart.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2aulbgmno.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mqyisjns.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2xkbvrgfu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2olnksghm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2alckpupb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vwzxlpuc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zqxvdpbq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jmxhwqfn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vrkgapqy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rombljcx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jrrhksdx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xnldnlpe.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uzmdqgmg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2prpfutui.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gerlngku.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2muwkwubb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2viokwcnx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hwpwntqh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dokpoowu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2oumbvyol.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yrgaksoo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xfrpkfuu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fcobqdqy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2yxfhtusw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2gljolmna.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dmfhhhxf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vqkpfzbb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ghuqoela.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ogfuwqum.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fkytsfvy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wzkjqsbd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qupsdwhz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ekctlbwg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2gpiwyevh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jlvzlwuy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hljijnsf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kejeiidy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2guvatpbr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tzprqsze.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2usgedwhn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mlfynxgo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2iasnsniv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2owdkyvfd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hoydfpuu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kiyzdwzb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lnqtvdsv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mguwmmfs.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zohotuxv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gmyzegun.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gavjdbbb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xqycajna.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fibwlmvw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zrzcnfqh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zzmutsds.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2sucqfezp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cxwyhtbe.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2uxqgbozb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2nkdwqugk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jadaqoyl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kqbrrphd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mqaozqmg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gqrqmmgu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ohmrsege.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pdnxgspw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kliaqlpc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2svzfmdsf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbczzkvg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vkikkpsp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2delhuupp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2thyyodgo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rxrdeywn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ztcapxzg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2dzwwajiq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jyrbrmgc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mttihkyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnfahpqo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kyfzhxuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxuklqnk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ttkqdawb.html


<!-- 参考信息 -->